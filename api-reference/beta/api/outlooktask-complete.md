---
title: 'OutlookTask: abgeschlossen'
description: 'Führen Sie eine Outlook-Aufgabe, die die **CompletedDateTime** -Eigenschaft auf das aktuelle Datum festgelegt wird, '
ms.openlocfilehash: 732da0f3eb03f6a4674e1254586ae21b5f3334bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064372"
---
# <a name="outlooktask-complete"></a>OutlookTask: abgeschlossen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Führen Sie eine Outlook-Aufgabe, die die **CompletedDateTime** -Eigenschaft auf das aktuelle Datum und die **Status** -Eigenschaft festlegt `completed`.

Wenn Sie eine Aufgabe in einer Terminserie in der Antwort durchführen wird die Auflistung der abgeschlossenen Aufgabe in der Datenreihe und die nächste Aufgabe in der Datenreihe enthalten.

Die **CompletedDateTime** -Eigenschaft gibt das Datum an, wenn die Aufgabe abgeschlossen ist. Den Zeitbereich des **CompletedDateTime** ist standardmäßig auf Mitternacht UTC festgelegt. 

Standardmäßig wird dieses Vorgangs (und die POST-, Get- und PATCH Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben. Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Tasks.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Tasks.ReadWrite    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}/complete

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Prefer: outlook.timezone | Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist. Optional.|

## <a name="request-body"></a>Anforderungstext

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [OutlookTask](../resources/outlooktask.md) -Auflistungsobjekt in der Antworttext.

## <a name="example"></a>Beispiel
Das folgende Beispiel kennzeichnet die angegebene Aufgabe als erledigt. Es gibt Pacific Standard Time (PST) in der `Prefer: outlook.timezone` Kopfzeile.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->
```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Die **CompletedDateTime** und andere Eigenschaften datumsspezifische in der Antwort werden in PST-Datei angegeben. 

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
    {
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTIBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->