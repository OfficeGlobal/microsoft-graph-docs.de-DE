---
title: Ressourcentyp teamMemberSettings
description: Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6ffd1dba4a0aafb1364a6d3f1ee673e2381c7178
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954253"
---
# <a name="teammembersettings-resource-type"></a>Ressourcentyp teamMemberSettings



Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolescher Wert|Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.|
|allowDeleteChannels|Boolescher Wert|Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.|
|allowAddRemoveApps|Boolescher Wert|Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.|
|allowCreateUpdateRemoveTabs|Boolescher Wert|Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten. |
|allowCreateUpdateRemoveConnectors|Boolescher Wert|Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
