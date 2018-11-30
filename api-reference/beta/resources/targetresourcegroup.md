---
title: Ressourcentyp targetResourceGroup
description: 'Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war. Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061422"
---
# <a name="targetresourcegroup-resource-type"></a>Ressourcentyp targetResourceGroup
Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war. Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD 



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|groupType|String| Mögliche Werte sind: `unifiedGroups`, `azureAD` und `unknownFutureValue`.|

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