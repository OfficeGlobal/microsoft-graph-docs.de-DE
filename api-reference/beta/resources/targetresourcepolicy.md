---
title: Ressourcentyp targetResourcePolicy
description: 'Gibt die Richtlinie, die von der Aktivität Audit betroffen war. Die Ressource TargetResource abgeleitet.   '
ms.openlocfilehash: 20486c535d0df4b3745f5cfc3414b320a9374075
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063422"
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