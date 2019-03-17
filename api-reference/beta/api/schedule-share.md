---
title: 'Zeitplan: Freigeben'
description: Teilen Sie einen Zeit Planzeitraum mit Schedule-Elementen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eaa2eae082c2b50f39b4a3ac2547ca5b0135381f
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657721"
---
# <a name="schedule-share"></a>Zeitplan: Freigeben

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Teilen Sie einen Zeit [Plan](../resources/schedule.md) Zeitraum mit Schedule-Elementen.
Erstellen Sie die Auflistungen von [Shift](../resources/shift.md) -und [timeOff](../resources/timeoff.md) -Elementen im angegebenen Zeitintervall [](../resources/schedule.md) des Zeitplans, die von den angegebenen Teammitgliedern angezeigt werden, einschließlich Mitarbeiter und Manager.
Jede [Shift](../resources/shift.md) -und [timeOff](../resources/timeoff.md) -Instanz in einem [Zeitplan](../resources/schedule.md) unterstützt eine Entwurfsversion und eine freigegebene Version des Elements. Die Entwurfsversion kann nur von Managern angezeigt werden, und die freigegebene Version kann von Mitarbeitern und Managern angezeigt werden. Für jede [Shift](../resources/shift.md) -und [timeOff](../resources/timeoff.md) -Instanz im angegebenen Zeitintervall aktualisiert die Freigabe Aktion die freigegebene Version aus der Entwurfsversion, sodass Mitarbeiter neben Managern auch die aktuellen Informationen zu dem Element anzeigen können. Der Parameter **notifyTeam** gibt weiter an, welche Mitarbeiter das Element anzeigen können.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

> **Hinweis**: Diese API unterstützt Administratorberechtigungen. Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

|Parameter                   |Typ           |Beschreibung  |
|-----------------------|-------------------|--------------|
| notifyTeam            |`Boolean`             |Gibt an, ob das gesamte Team eine sichtbare Benachrichtigung über diese Aktion erhalten soll, oder nur Mitarbeiter, denen eine Schicht zugewiesen wurde, die freigegeben wurde. Erforderlich.       |
| startDateTime         |`DateTimeOffset`   |Die Startzeit für die Freigabe von Schichten im Zeitplan. Erforderlich.   |
| endDateTime           |`DateTimeOffset`   | Die Endzeit für die Freigabe von Schichten für den Zeitplan bis.   |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
