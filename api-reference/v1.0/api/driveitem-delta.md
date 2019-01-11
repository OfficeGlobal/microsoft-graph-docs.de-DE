---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Synchronisieren der Inhalte eines Laufwerks
localization_priority: Priority
ms.openlocfilehash: edf47b1ab6ecd910a5ad2dbc2e87454963a12555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815988"
---
# <a name="track-changes-for-a-drive"></a>Laufwerksänderungen nachverfolgen

Mit dieser Methode kann Ihre App Änderungen nachverfolgen, die im Laufe der Zeit an Laufwerken sowie deren untergeordneten Elementen vorgenommen werden.

Die App ruft zunächst `delta` ohne Parameter auf. Der Dienst startet dann eine Enumeration der Laufwerkshierarchie und gibt Seiten mit Elementen sowie entweder einen `@odata.nextLink` oder einen `@odata.deltaLink` zurück, wie unten beschrieben. Die App sollte die Aufrufe solange mit dem `@odata.nextLink` fortführen, bis kein `@odata.nextLink` mehr zurückgegeben wird oder bis eine Antwort mit einem leeren Satz an Änderungen zurückgegeben wird.

Sobald alle Änderungen empfangen wurden, können Sie sie auf den lokalen Zustand anwenden. Wenn Sie zu einem späteren Zeitpunkt nochmals auf Änderungen prüfen möchten, rufen Sie erneut `delta` auf, mit dem `@odata.deltaLink` aus der vorherigen Antwort.

Gelöschte Elemente werden mit dem [`deleted`Facet](../resources/deleted.md) zurückgegeben. Elemente, für die diese Eigenschaft gesetzt ist, sollten Sie aus Ihrem lokalen Zustand entfernen. 

**Hinweis:** Löschen Sie Ordner nur lokal, wenn sie nach der Synchronisierung aller Änderungen leer sind.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a>Funktionsparameter

| Parameter   | Typ  | Beschreibung                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| token  | string | Optional. Wenn Sie nicht angegeben ist, zählt aktuellen Status der Hierarchie. Wenn `latest`, gibt eine leere Antwort mit dem neuesten Delta-Token. Wenn eine frühere Delta-Token gibt neuen Status seit Token zurück.

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$select`, `$expand` und `$top` zur Anpassung der Antwort.

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von Ressourcen des Typs [DriveItem](../resources/driveitem.md) im Antworttext zurück.

Zusätzlich zu der Sammlung von DriveItems enthält die Antwort außerdem eine der folgenden Eigenschaften:

| Name                 | Wert  | Beschreibung                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **@odata.nextLink**  | url    | Eine URL zum Abrufen der nächsten verfügbaren Seite von Änderungen, sofern weitere Änderungen im aktuellen Satz vorhanden sind                                        |
| **@odata.deltaLink** | url    | Eine URL, die anstelle eines **@odata.nextLink** zurückgegeben wird, sobald alle aktuellen Änderungen zurückgegeben wurden. Sie wird verwendet, um zu einem späteren Zeitpunkt den nächsten Satz von Änderungen zu lesen.  |

## <a name="example-initial-request"></a>Beispiel (ursprüngliche Anforderung)

Hier sehen Sie ein Beispiel für einen Aufruf dieser API zur Ermittlung Ihres lokalen Zustands.

### <a name="request"></a>Anforderung

Unten ein Beispiel für eine ursprüngliche Anforderung:

<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

Diese Antwort enthält die erste Seite von Änderungen. Die Eigenschaft **@odata.nextLink** gibt an, dass im aktuellen Satz von Elementen weitere Elemente verfügbar sind. Die App sollte nun solange den URL-Wert von **@odata.nextLink** anfordern, bis alle Seiten von Elementen abgerufen wurden.

## <a name="example-last-page-in-a-set"></a>Beispiel (letzte Seite in einem Satz)

Unten sehen Sie ein Beispiel für einen Aufruf dieser API zur Aktualisierung Ihres lokalen Zustands.

### <a name="request"></a>Anforderung

Hier sehen Sie ein Beispiel für eine Anforderung nach der ursprünglichen Anforderung:

<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

Diese Antwort gibt an, dass im Zeitraum zwischen der ursprünglichen Anforderung und dieser Anforderung zur Aktualisierung des lokalen Zustands das Element `folder2` gelöscht wurde und das Element `file.txt` entweder hinzugefügt oder geändert wurde.

Die letzte Seite mit Elementen enthält die Eigenschaft **@odata.deltaLink**. Sie spezifiziert die URL, über die zu einem späteren Zeitpunkt Änderungen abgerufen werden können, die bis dahin an dem jetzt aktuellen Elementsatz vorgenommen wurden.

Es kann passieren, dass der Dienst für ein Token keine Änderungsliste zurückgeben kann. (Das ist beispielsweise der Fall, wenn ein Client nach einer längeren Verbindungsunterbrechung versucht, ein altes Token wiederzuverwenden, oder wenn sich der Zustand eines Servers geändert hat und daher ein neues Token erforderlich ist.) In solchen Fällen gibt der Dienst einen Fehler des Typs `HTTP 410 Gone` zurück. Die Fehlerantwort enthält einen der unten aufgeführten Fehlercodes und einen Header `Location` mit einem neuen „nextLink“, der eine vollständig neue „delta“-Enumeration startet. Vergleichen Sie nach Abschluss der vollständigen Enumeration die zurückgegebenen Elemente mit Ihrem lokalen Zustand, und befolgen Sie diese Anweisungen:

| Fehlertyp                       | Anweisungen                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | Ersetzen Sie alle lokalen Elemente durch die Serverversion (einschließlich gelöschter Elemente), wenn Sie sicher sind, dass der Dienst bei der letzten Synchronisierung mit den lokalen Änderungen aktualisiert wurde. Laden Sie alle lokalen Änderungen hoch, die dem Server noch nicht bekannt sind. |
| `resyncChangesUploadDifferences` | Laden Sie alle lokalen Elemente hoch, die der Dienst nicht zurückgegeben hat, und laden Sie alle Dateien hoch, die sich von der Version auf dem Server unterscheiden (wobei Sie beide Kopien beibehalten, wenn Sie nicht sicher sind, welche die aktuelle ist).                                       |

## <a name="retrieving-the-current-deltalink"></a>Abrufen des aktuellen deltaLink

In einigen Fällen kann es sinnvoll sein, den aktuellen Wert von DeltaLink anzufordern, ohne zunächst die bereits auf dem Laufwerk vorhandenen Elemente aufzulisten.

Dies kann hilfreich sein, wenn die App nur über Änderungen informiert werden möchte und vorhandene Elemente keine Rolle spielen.
Rufen Sie zum Abrufen des aktuellen deltaLink `delta` mit dem Abfragezeichenfolgenparameter `?token=latest` auf.

**Hinweis: Wenn Sie versuchen, eine vollständige lokale Darstellung der Elemente in einem Ordner oder Laufwerk zu verwalten, müssen Sie `delta` für die erste Enumeration verwenden. Andere Methoden, z. B. Auslagerung über die `children`-Sammlung eines Ordners, geben nicht unbedingt jedes einzelne Element zurück, wenn während der Enumeration ein Schreibvorgang ausgeführt wird. Die Verwendung von `delta` ist die einzige Möglichkeit sicherzustellen, dass Sie alle erforderlichen Daten gelesen haben.**

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a>Bemerkungen

* Der „delta“-Feed zeigt den aktuellen Zustand jedes Elements, nicht jede Änderung. Wenn ein Element beispielsweise zweimal umbenannt wurde, wird es nur einmal angezeigt, mit seinem neuesten Namen.
* Ein Element kann mehrmals in einem „delta“-Feed aufgeführt werden, aus jeweils unterschiedlichen Gründen. Verwenden Sie das letzte Vorkommen in der Auflistung.
* Die Eigenschaft `parentReference` von Elementen enthält keinen Wert für **path**. Der Grund: Wenn ein Ordner umbenannt wird, gibt **delta** keine Nachfolger dieses Ordners zurück. **Bei Verwendung von „delta“ sollten Sie Elemente immer anhand ihrer ID nachverfolgen.**
* In OneDrive for Business und SharePoint wird `delta` nur für den Ordner `root` unterstützt, für andere Ordner auf einem Laufwerk jedoch nicht.

* Delta gibt keine der folgenden „DriveItem“-Eigenschaften zurück:
  * **cTag**
  * **lastModifiedBy**
  * **size**

## <a name="error-responses"></a>Fehlerantworten

Zusätzlich zu den vorstehend beschriebenen Fehlern bei der erneuten Synchronisierung finden Sie unter [Fehlerantworten] [ error-response] weitere Informationen darüber, wie Fehler zurückgegeben werden.

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes"
} -->
