---
title: Ressourcentyp teamMemberSettings
description: Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.
localization_priority: Normal
ms.openlocfilehash: 85f8794ea3564174c75f38228f3891bcd264df2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851380"
---
# <a name="teammembersettings-resource-type"></a>Ressourcentyp teamMemberSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.|
|allowDeleteChannels|Boolean|Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.|
|allowAddRemoveApps|Boolean|Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.|
|allowCreateUpdateRemoveTabs|Boolean|Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten. |
|allowCreateUpdateRemoveConnectors|Boolean|Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.|

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
