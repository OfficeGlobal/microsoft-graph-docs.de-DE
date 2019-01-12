---
title: Arbeiten mit langen Aktionen (Beta)
description: In diesem Artikel wird das Arbeiten mit lange ausgeführten Aktionen beschrieben.
localization_priority: Normal
ms.openlocfilehash: d7ee9631e9e18ae1972e2b156366c66d3d3dd455
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868054"
---
# <a name="working-with-long-running-actions-beta"></a>Arbeiten mit langen Aktionen (Beta)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Abfrage einiger API-Antworten kann unbestimmte Zeit dauern.
Anstatt zu warten, bis der Vorgang abgeschlossen ist und Sie eine Antwort erhalten, können Sie das lange ausgeführte Aktionsmuster von Microsoft Graph verwenden.
Bei der Verwendung dieses Musters verfügt die App über eine Wartezeit für die Abfrage von Statusupdates für lange ausgeführte Aktionen, wobei Anforderungen nicht auf den Abschluss der Aktion warten müssen.

Das allgemeine Muster umfasst die folgenden Schritte:

1. Die App fordert eine lange ausgeführte Aktion über die API an. Die API akzeptiert die Aktion und gibt eine `202 Accepted`-Antwort zusammen mit einem Speicherortheader für die API-URL zum Abrufen von Statusberichten zur Aktion zurück.
2. Die App fordert die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta)-Antwort mit dem Fortschritt der lange ausgeführten Aktion.
3. Die lange ausgeführte Aktion wird abgeschlossen. 
4. Ihre App fordert erneut die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta)-Antwort über den Abschluss der lange ausgeführten Aktion.

## <a name="initial-action-request"></a>Anfängliche Aktionsanforderung

Lassen Sie uns die einzelnen Schritte für ein Beispiel eines [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta)-Szenarios durchgehen.
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

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

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

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

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

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

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
| DriveItem | [Copy](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a>Voraussetzungen

Die gleichen [Berechtigungen](./permissions-reference.md), die für die Ausführung einer lange ausgeführten Aktion erforderlich sind, sind ebenfalls erforderlich, um den Status einer lange ausgeführten Aktion abzufragen.




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
