---
title: Ressourcentyp targetResourceGroup
description: 'Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war. Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851184"
---
# <a name="targetresourcegroup-resource-type"></a>Ressourcentyp targetResourceGroup
Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war. Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD 



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|groupType|Zeichenfolge| Mögliche Werte sind: `unifiedGroups`, `azureAD` und `unknownFutureValue`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
