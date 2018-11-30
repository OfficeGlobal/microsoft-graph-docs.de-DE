---
title: settingValue-Ressourcentyp
description: Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020091"
---
# <a name="settingvalue-resource-type"></a>settingValue-Ressourcentyp

Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.

### <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|name|Zeichenfolge| Name der Einstellung (entsprechend der [groupSettingTemplate](groupsettingtemplate.md)-Definition). |
|Wert|Zeichenfolge| Wert der Einstellung. |

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->