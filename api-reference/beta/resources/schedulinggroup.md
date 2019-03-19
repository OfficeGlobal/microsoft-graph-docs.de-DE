---
title: schedulingGroup-Ressourcentyp
description: Eine logische Gruppierung von Mitgliedern im Zeitplan (in der Regel anhand der Rolle).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657868"
---
# <a name="schedulinggroup-resource-type"></a>schedulingGroup-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine logische Gruppierung von Benutzern in einem [Zeitplan](schedule.md) (in der Regel anhand der Rolle). 

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[schedulingGroup erstellen](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | Ein neues `schedulingGroup` erstellen.|
|[schedulingGroup auflisten](../api/schedule-list-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md)-Auflistung | Abrufen der Liste von `schedulingGroups` in einem Zeitplan.|
|[schedulingGroup abrufen](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | Abrufen eines `schedulingGroup` anhand der ID.|
|[schedulingGroup ersetzen](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | Ein `schedulingGroup` ersetzen.|
|[schedulingGroup löschen](../api/schedulinggroup-delete.md) | Keine | `schedulingGroup` als inaktiv markieren.|

## <a name="properties"></a>Eigenschaften
|Name          |Typ           |Beschreibung                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |ID des `schedulingGroup`.|
| displayName   | `string`      | Der Anzeigename für das `schedulingGroup`. Erforderlich. |
| isActive          |`bool`      | Gibt an, ob `schedulingGroup` beim Erstellen neuer Entitäten oder beim Aktualisieren vorhandener Entitäten verwendet werden kann. Erforderlich. |
| UserIds       | `collection(string)`    |  Die Liste der Benutzer-IDs, die ein Mitglied von `schedulingGroup` sind. Erforderlich. |
| createdDateTime       |`DateTimeOffset`        |Der Zeitstempel, mit dem dieses `schedulingGroup` zuerst erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |Der Zeitstempel, mit dem dieses `schedulingGroup` zuletzt aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: '2014-01-01T00:00:00Z'. |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Die Identität, die dieses `schedulingGroup` zuletzt aktualisiert hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
