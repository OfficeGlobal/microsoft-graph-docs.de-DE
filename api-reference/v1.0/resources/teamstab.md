---
title: Ressourcentyp teamsTab
description: 'Eine TeamsTab ist eine Registerkarte, hat fixiert an einen Kanal innerhalb eines Teams (angeschlossen). '
ms.openlocfilehash: 4e9773fa2e4ea6a114c1f2695906c09d84b3f043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017900"
---
# <a name="teamstab-resource-type"></a>Ressourcentyp teamsTab



Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen). 

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Registerkarten](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Listen Registerkarten fixiert zu einem Kanal.|
|[Erste Registerkarte](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Liest eine Registerkarte an einen Kanal fixiert.|
|[Registerkarte hinzufügen](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Fügt (Pins) einer Registerkarte zu einem Kanal.|
|[Registerkarte entfernen](../api/teamstab-delete.md) | Keines | Entfernt (löst) einer Registerkarte aus einem Kanal.|
|[Registerkarte "Aktualisieren"](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Aktualisiert die Registerkarte Eigenschaften.|


## <a name="properties"></a>Eigenschaften

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|  id              |   string                  |  Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.     |
|  displayName            |   string                  |  Der Name der Registerkarte.     |
|  sortOrderIndex  |   Int                     |  Index der Reihenfolge für die Sortierung von Registerkarten     |
|  webUrl          |   string                  |  Deep-Link-Url der Registerkarte-Instanz. Schreibgeschützt.     |
|  Konfiguration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.     |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Die Anwendung, die auf der Registerkarte verknüpft ist. Nach der Erstellung der Registerkarte werden nicht geändert. |

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
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Siehe auch

[Konfigurieren der integrierten Registerkartentypen](/graph/teams-configuring-builtin-tabs)
