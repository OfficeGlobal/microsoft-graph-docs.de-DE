---
title: Ressourcentyp modifiedProperty
description: Gibt an, die geänderten Eigenschaften mit vorherigen und neuen Wert für eine Ressource in Azure AD, die geändert wird.
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060769"
---
# <a name="modifiedproperty-resource-type"></a>Ressourcentyp modifiedProperty
Gibt an, die geänderten Eigenschaften mit vorherigen und neuen Wert für eine Ressource in Azure AD, die geändert wird.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|String|Gibt den Eigenschaftennamen des Zielattributs, die geändert wurde.|
|newValue|Zeichenfolge|Gibt den aktualisierten Wert für die Eigenschaft an.|
|oldValue|Zeichenfolge|Gibt den vorherigen Wert (vor der Aktualisierung) für die Eigenschaft.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->