---
title: Ressourcentyp teamsTab
description: 'Eine TeamsTab ist eine Registerkarte, hat fixiert an einen Kanal innerhalb eines Teams (angeschlossen). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2db59065f139e2e704c3394f7afb82cba91c33fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509287"
---
# <a name="teamstab-resource-type"></a>Ressourcentyp teamsTab

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen). 

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Registerkarten](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Listen Registerkarten fixiert zu einem Kanal.|
|[Erste Registerkarte](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Liest eine Registerkarte an einen Kanal fixiert.|
|[Registerkarte hinzufügen](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Fügt (Pins) einer Registerkarte zu einem Kanal.|
|[Registerkarte entfernen](../api/teamstab-delete.md) | Keine | Entfernt (löst) einer Registerkarte aus einem Kanal.|
|[Registerkarte "Aktualisieren"](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Aktualisiert die Registerkarte Eigenschaften.|


## <a name="properties"></a>Eigenschaften

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|  id              |   string                  |  Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.     |
|  displayName            |   string                  |  Der Name der Registerkarte.     |
|  name            |   string                  |  (Veraltet) Der Name der Registerkarte.     |
|  teamsAppId           |   string             |  App-Definition-Bezeichner der Registerkarte. Dieser Wert kann nach der Erstellung der Registerkarte geändert werden.     |
|  sortOrderIndex  |   int                     |  Index der Reihenfolge für die Sortierung von Registerkarten verwendet werden soll.     |
|  webUrl          |   string                  |  Deep-Link-Url der Registerkarte-Instanz. Schreibgeschützt.     |
|  Konfiguration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.     |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Die Anwendung, die auf der Registerkarte verknüpft ist. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a>Siehe auch

[Konfigurieren der integrierten Registerkartentypen](/graph/teams-configuring-builtin-tabs)
