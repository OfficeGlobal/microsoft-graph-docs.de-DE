---
title: Ressourcentyp attributeMappingParameterSchema
description: Beschreibt einen einzelnen Parameter in einer AttributeMappingFunctionSchema verwendet.
localization_priority: Normal
ms.openlocfilehash: 083f89ebc5a74e6fd58a33925b2bfa46801b7961
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892169"
---
# <a name="attributemappingparameterschema-resource-type"></a>Ressourcentyp attributeMappingParameterSchema

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Beschreibt einen einzelnen Parameter in einer [AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)verwendet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Boolean                   |Der angegebene Parameter kann mehrere Male bereitgestellt werden (beispielsweise Eingabe mehrere Zeichenfolgen der `Concatenate(string,string,...)` Funktion). |
|name                        |String                    |Name des Parameters. |
|erforderlich                    |Boolean                   |`true`Wenn der Parameter erforderlich ist. andernfalls `false`. |
|type                        |Zeichenfolge                    |Mögliche Werte: `Boolean`, `Binary`, `Reference`, `Integer`, `String`. Der Standardwert lautet `String`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
