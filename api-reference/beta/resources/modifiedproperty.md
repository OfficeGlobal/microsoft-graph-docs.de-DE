---
title: Ressourcentyp modifiedProperty
description: Gibt an, die geänderten Eigenschaften mit vorherigen und neuen Wert für eine Ressource in Azure AD, die geändert wird.
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844454"
---
# <a name="modifiedproperty-resource-type"></a>Ressourcentyp modifiedProperty
Gibt an, die geänderten Eigenschaften mit vorherigen und neuen Wert für eine Ressource in Azure AD, die geändert wird.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|Zeichenfolge|Gibt den Eigenschaftennamen des Zielattributs, die geändert wurde.|
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
