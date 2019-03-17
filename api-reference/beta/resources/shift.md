---
title: Schicht-Ressourcentyp
description: Eine Schicht ist eine Einheit der geplanten Arbeit im Zeitplan.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657896"
---
# <a name="shift-resource-type"></a>Schicht-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Einheit der geplanten Arbeit in einem [Zeitplan](schedule.md). 

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Schicht erstellen](../api/schedule-post-shifts.md) | [UMSCHALT](shift.md) | Erstellen Sie eine `shift`neue.|
|[Listen Verschiebungen](../api/schedule-list-shifts.md) | [Shift](shift.md) -Auflistung | Rufen Sie die Liste `shifts` der in diesem Zeitplan ab.|
|[Shift abrufen](../api/shift-get.md) | [UMSCHALT](shift.md) | Rufen Sie `shift` eine nach ID ab.|
|[UMSCHALT ersetzen](../api/shift-put.md) | [UMSCHALT](shift.md) | Ersetzen Sie `shift`a.|
|[Schicht löschen](../api/shift-delete.md) | None | Löschen Sie `shift` eine aus dem Zeitplan.|

## <a name="properties"></a>Eigenschaften
|Name          |Typ           |Beschreibung                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID des `shift`.|
| userId            |`string`      |Die ID des Benutzers, der dem `shift`zugewiesen ist. Erforderlich. |
| schedulingGroupId         |`string`      |Die ID der Planungsgruppe, `shift` in der Sie enthalten ist. Erforderlich. |
| sharedShift   |`[shiftItem](shiftitem.md)`  |Die freigegebene `shift` Version dieses, die sowohl von Mitarbeitern als auch von Managern angezeigt werden kann. Erforderlich. |
| draftShift        |`[shiftItem](shiftitem.md)`        |Die Entwurfsversion dieses `shift` , die von Managern angezeigt werden kann. Erforderlich. |
| createdDateTime       |`DateTimeOffset`        |Der Zeitstempel, für `shift` den dies zuerst erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| lastModifiedDateTime      |`DateTimeOffset`        |Der Zeitstempel, an `shift` dem dieser zuletzt aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Die Identität, die zuletzt aktualisiert `shift`hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
