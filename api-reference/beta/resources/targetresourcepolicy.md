---
title: Ressourcentyp targetResourcePolicy
description: 'Gibt die Richtlinie, die von der Aktivität Audit betroffen war. Die Ressource TargetResource abgeleitet.   '
localization_priority: Normal
ms.openlocfilehash: 355e6ac11741a2aa7aeb780bdac4b7be373092af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813139"
---
# <a name="targetresourcepolicy-resource-type"></a>Ressourcentyp targetResourcePolicy
Gibt die Richtlinie, die von der Aktivität Audit betroffen war. Die Ressource [TargetResource](targetresource.md) abgeleitet.   



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|policyType|String|Gibt den Namen der Richtlinie, die geändert oder wurde gezielt für Änderung|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
