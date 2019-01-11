---
title: Ressourcentyp stringKeyAttributeMappingSourceValuePair
description: Stellt ein Schlüssel-Wert-Paar, in denen der Schlüssel ist eine Zeichenfolge und der Wert ist AttributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: 24695cc64fd3c240d5416a7b37e9a5d373e5a88a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805089"
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
