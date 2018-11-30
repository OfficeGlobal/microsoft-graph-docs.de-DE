---
title: Ressourcentyp stringKeyAttributeMappingSourceValuePair
description: Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist AttributeMappingSource.
ms.openlocfilehash: 875c593ae652ce763f420d29e5dd4e5e2601bc88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065195"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>Ressourcentyp stringKeyAttributeMappingSourceValuePair

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist [AttributeMappingSource](synchronization-attributemappingsource.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Key|String|Der Name des Parameters.|
|Wert|[attributeMappingSource](synchronization-attributemappingsource.md)|Der Wert des Parameters.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
