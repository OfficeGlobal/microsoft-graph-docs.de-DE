---
title: 'DirectoryObject: Delta'
description: 'Get neu erstellt, aktualisiert oder gelöscht Verzeichnisobjekten der folgenden Typen: Benutzer, Gruppe oder Organisation Kontakt in einer einzelnen Delta-Abfrage. Finden Sie unter Nachverfolgen von Änderungen für Details.'
localization_priority: Normal
ms.openlocfilehash: 823107bce56d77c4e9c29a77405ac014443f5190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854495"
---
# <a name="directoryobject-delta"></a>DirectoryObject: Delta

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Get neu erstellt, aktualisiert oder gelöscht Verzeichnisobjekten der folgenden Typen: [Benutzer](../resources/user.md), [Gruppe](../resources/group.md) und [organisatorische Kontakt](../resources/orgcontact.md)in einer einzelnen Delta-Abfrage. Einzelheiten finden Sie unter [Nachverfolgen von Änderungen](/graph/delta-query-overview) .

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.Read.All, Directory.AccessAsUser.All  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt  |
|Anwendung | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

Zum Nachverfolgen von Änderungen beginnen, stellen Sie eine Anforderung, einschließlich der Delta-Funktion für die Ressource DirectoryObjects.

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a>Abfrageparameter

Nachverfolgen von Änderungen verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe. Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben. Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.

Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.

In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.

| Abfrageparameter | Typ |Beschreibung|
|:---------------|:--------|:----------|
| $deltatoken | string | Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Benutzersammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.|
| $skiptoken | string | Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Benutzersammlung weitere Änderungen zum Nachverfolgen vorliegen. |

### <a name="odata-query-parameters"></a>OData-Abfrageparameter

Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.

- Sie können `$filter` mit den speziellen `isOf` Operator Filtern eine Teilmenge der Typen von DirectoryObject abgeleitet.
  - Sie können mehrere Ausdrücke mit kombinieren ein `or`, ermöglicht eine einzelne Delta-Abfrage mehrere Typen nachverfolgen vorhanden ist. Finden Sie im [dritten Beispiel](#request-3) für Details.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | zurückgeben = minimal <br><br>Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden. Optional. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

### <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Benutzer](../resources/directoryobject.md) -Auflistungsobjekt in der Antworttext. Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.

- Wenn ein `nextLink` URL zurückgegeben wird:
  - Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen. Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.
  - Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung. Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.

- Wenn ein `deltaLink` URL zurückgegeben wird:
  - Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll. Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.
  - Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung

Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:

- Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten. Dies schließt Eigenschaften auf null-Wert festgelegt wird.
- Wenn die Eigenschaft nicht geändert wurde, wird der alte Wert in der Antwort enthalten.
- Wenn die Eigenschaft nicht festgelegt wurde, bevor es nicht in der Antwort überhaupt eingeschlossen werden sollen.


> **Hinweis:** Mit diesem Verhalten ist die Antwort verfolgen es nicht möglich, sagen, ob eine Eigenschaft oder nicht geändert wird. Darüber hinaus meist die Antworten Delta groß sein, da sie alle Eigenschaftswerte enthalten.

#### <a name="alternative-return-only-the-changed-properties"></a>Alternative: nur die geänderten Eigenschaften zurückgeben

Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:

- Wenn die Eigenschaft geändert wurde, ist der neue Wert in der Antwort enthalten. Dies schließt Eigenschaften auf null-Wert festgelegt wird.
- Wenn die Eigenschaft nicht geändert wurde, ist die Eigenschaft nicht in allen in der Antwort enthalten. (Andere als das Standardverhalten).

> **Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta. Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.

## <a name="example"></a>Beispiel

### <a name="request-1"></a>Anforderung 1

Nachfolgend sehen Sie ein Beispiel der Anforderung. Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a>Antwort 1

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Nicht `isOf` Filter verwendet wurde, damit alle Typen von DirectoryObject abgeleitete zurückgegeben werden.

>**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a>Anforderung 2

Im nächste Beispiel wird die Verwendung des Verhaltens alternative minimale Antwort:
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a>Antwort 2

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Beachten Sie, dass nur die Eigenschaften, die tatsächlich geändert wurden zurückgegeben werden.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a>Anforderung 3

Das nächste Beispiel veranschaulicht die erste Anforderung mithilfe der `isOf` Operator herausfiltern nur Benutzer- und Entitäten:
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a>Antwort 3

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Beachten Sie, dass nur Benutzer und Gruppe Objekte zurückgegeben werden:

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

- [Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](/graph/delta-query-overview).
- [Inkrementelle Änderungen für Benutzer erhalten möchten](/graph/delta-query-users).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
