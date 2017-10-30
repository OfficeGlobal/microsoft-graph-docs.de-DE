---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.topic: conceptual
ms.openlocfilehash: 963d2b71b879c285a43378d07c1bfd755f150b9f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="working-with-long-running-actions-beta"></a>Arbeiten mit langen Aktionen (Beta)

> **Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Abfrage einiger API-Antworten kann unbestimmte Zeit dauern.
Anstatt zu warten, bis der Vorgang abgeschlossen ist und Sie eine Antwort erhalten, können Sie das lange ausgeführte Aktionsmuster von Microsoft Graph verwenden.
Bei der Verwendung dieses Musters verfügt die App über eine Wartezeit für die Abfrage von Statusupdates für lange ausgeführte Aktionen, wobei Anforderungen nicht auf den Abschluss der Aktion warten müssen.

Das allgemeine Muster umfasst die folgenden Schritte:

1. Die App fordert eine lange ausgeführte Aktion über die API an. Die API akzeptiert die Aktion und gibt eine `202 Accepted`-Antwort zusammen mit einem Speicherortheader für die API-URL zum Abrufen von Statusberichten zur Aktion zurück.
2. Die App fordert die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md)-Antwort mit dem Fortschritt der lange ausgeführten Aktion.
3. Die lange ausgeführte Aktion wird abgeschlossen. 
4. Ihre App fordert erneut die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md)-Antwort über den Abschluss der lange ausgeführten Aktion.

## <a name="initial-action-request"></a>Anfängliche Aktionsanforderung

Lassen Sie uns die einzelnen Schritte für ein Beispiel eines [DriveItem Copy](../api-reference/beta/api/driveitem_copy.md)-Szenarios durchgehen.
In diesem Szenario fordert eine App das Kopieren eines Ordners mit einer großen Menge enthaltener Daten an.
Das Abschließen dieser Anforderung wird wahrscheinlich einige Sekunden dauern, da die Datenmenge groß ist.

<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```

Die API antwortet, dass die Aktion akzeptiert wurde, und gibt die URL zum Abrufen des Status der lange ausgeführten Aktion zurück.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

**Hinweis:** Die zurückgegebene URL des Speicherorts befindet sich möglicherweise nicht auf dem Microsoft Graph-API-Endpunkt.

In vielen Fällen ist dies das Ende der Anforderung, da der Kopiervorgang abgeschlossen wird, ohne dass die App weitere Aufgaben ausführt.
Wenn die App jedoch den Status des Kopiervorgangs anzeigen oder sicherstellen muss, dass dieser ohne Fehler abgeschlossen wird, kann sie dazu die Überwachungs-URL verwenden.

## <a name="retrieve-a-status-report-from-the-monitor-url"></a>Abrufen eines Statusberichts von der Überwachungs-URL

Um den Status des Kopiervorgang zu überprüfen, stellt die App eine Anforderung an die URL, die in der vorherigen Antwort bereitgestellt wurde.
*Hinweis:* Diese Anforderung erfordert keine Authentifizierung, da die URL kurzlebig und einzigartig für den ursprünglichen Aufrufer ist. 

<!-- { "blockType": "request", "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

Der Dienst gibt eine Antwort mit der Information zurück, dass die lang ausgeführte Aktion noch nicht abgeschlossen ist:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

Diese Information kann verwendet werden, um den Benutzer über den Fortschritt des Kopiervorgangs zu informieren.
Die App kann die Überwachungs-URL weiterhin abfragen, um Statusupdates anzufordern und den Fortschritt der Aktion nachzuverfolgen.

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a>Abrufen eines Statusberichts zum Abschluss von der Überwachungs-URL

Nach einigen Sekunden ist der Kopiervorgang abgeschlossen.
Wenn die App nun die Überwachungs-URL abfragt, ist die Antwort eine Weiterleitung zum Endergebnis der Aktion.

<!-- { "blockType": "request", "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

Wenn die Aktion ausgeführt wurde, gibt die Antwort des Überwachungsdienstes die resourceId für die Ergebnisse zurück.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a>Abrufen der Ergebnisse des abgeschlossenen Vorgangs

Nachdem der Auftrag abgeschlossen wurde, gibt die Überwachungs-URL die Ressourcen-ID des Ergebnisses zurück, in diesem Fall die neue Kopie des ursprünglichen Elements.
Sie können dieses neue Element mithilfe der Ressourcen-ID ansprechen. Beispiel:

<!-- { "blockType": "request", "name": "lro-copy-item-example-complete", "scopes": "files.readwrite" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a>Unterstützte Ressourcen

Lange ausgeführte Aktionen werden für die folgenden API-Methoden API unterstützt:

| **Ressource** | **API** |
|:------ | :------ |
| DriveItem | [Copy](../api-reference/beta/api/driveitem_copy.md) |

## <a name="prerequisites"></a>Voraussetzungen

Die gleichen [Berechtigungen](./permissions_reference.md), die für die Ausführung einer lange ausgeführten Aktion erforderlich sind, sind ebenfalls erforderlich, um den Status einer lange ausgeführten Aktion abzufragen.




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "tocPath": "Concepts/Long running actions"
} -->