---
title: Outlooktask aktualisieren
description: Schreibbare Eigenschaften einer Outlook-Aufgabe zu ändern.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526886"
---
# <a name="update-outlooktask"></a>Outlooktask aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Schreibbare Eigenschaften einer Outlook-Aufgabe zu ändern.

Die Eigenschaft **CompletedDateTime** kann mit der Aktion **Complete** oder explizit mit einer PATCH-Operation gesetzt werden. Wenn Sie PATCH für die Einstellung von **CompletedDateTime** verwenden, stellen Sie sicher, dass Sie **Status** ebenfalls auf `completed` einstellen.

Standardmäßig wird dieses Vorgangs (und die POST, GET und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben. Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.

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
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Prefer: outlook.timezone | Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist. Optional.|

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|assignedTo|String|Der Name der Person, die die Aufgabe zugewiesen wurde.|
|body|[itemBody](../resources/itembody.md)|Der Hauptteil der Aufgabe, die in der Regel Informationen zum Vorgang enthält. Beachten Sie, dass nur HTML-Typ unterstützt wird.|
|categories|Zeichenfolgenauflistung|Die Kategorien, die dem Vorgang zugeordnet.|
|changeKey|String|Die Version des Vorgangs.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, dass der Vorgang abgeschlossen wurde.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung die Aufgabe. Standardmäßig ist es in UTC. Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen. Wert der Eigenschaft verwendet die ISO 8601-Format. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, die die Aufgabe fertig gestellt werden.|
|hasAttachments|Boolescher Wert|Legen Sie auf true zurück, wenn der Vorgang Anlagen hat.|
|Wichtigkeit|string|Die Wichtigkeit des Ereignisses. Mögliche Werte sind: `low`, `normal` und `high`.|
|isReminderOn|Boolean|Legen Sie auf true zurück, wenn eine Warnung festgelegt ist, um die Benutzer über die Aufgabe zu erinnern.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten die Aufgabe Änderung. Standardmäßig ist es in UTC. Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen. Wert der Eigenschaft um ISO 8601-Format verwendet und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|owner|String|Der Name der Person, die die Aufgabe erstellt.|
|parentFolderId|String|Der eindeutige Bezeichner für die Aufgabe übergeordneten Ordner.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Das Serienmuster für den Vorgang.|
|ReminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Datum und Zeit für eine Erinnerung des Vorgangs erfolgt.|
|sensitivity|string|Gibt die Ebene des Datenschutzes für den Vorgang an. Mögliche Werte: sind `normal`, `personal`, `private` und `confidential`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, wenn der Vorgang zu beginnen.|
|status|string|Gibt das Bundesland oder den Fortschritt des Vorgangs. Mögliche Werte sind: `notStarted`, `inProgress`, `completed`, `waitingOnOthers` und `deferred`.|
|subject|String|Eine kurze Beschreibung oder Titel des Vorgangs.|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTask](../resources/outlooktask.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Das folgende Beispiel ändert die Eigenschaft **DueDateTime** und verwendet die `Prefer: outlook.timezone` Header die datumsspezifische Eigenschaften in der Antwort in der Eastern Standard Time (EST) Ausdrücken angeben.
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
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
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
