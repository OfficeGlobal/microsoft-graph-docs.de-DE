---
title: Ressourcentyp teamGuestSettings
description: Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.
localization_priority: Normal
ms.openlocfilehash: 15644f3761329589a4d770e777ae5fd63751e6be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851541"
---
# <a name="teamguestsettings-resource-type"></a>Ressourcentyp teamGuestSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.|
|allowDeleteChannels|Boolean|Bei Festlegung auf "true" Gäste Kanäle löschen kann.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
