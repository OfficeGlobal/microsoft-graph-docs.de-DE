---
title: Ressourcentyp attributeMappingSource
description: 'Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt. Beispielsweise kann ein einfaches Wert aus einem gegebenen Attribut für das Quellobjekt sein oder einen komplexeren Ausdruck Zeichenfolge Verkettung/Extraction/Ersatz von basierend auf verschiedene Attribute für Datenquellen sind möglich. '
localization_priority: Normal
ms.openlocfilehash: a7c1493f27f34230d4305fe95b2d2f03a5ad25e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825011"
---
# <a name="attributemappingsource-resource-type"></a>Ressourcentyp attributeMappingSource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt. Beispielsweise kann ein einfaches Wert aus einem gegebenen Attribut für das Quellobjekt sein oder einen komplexeren Ausdruck Zeichenfolge Verkettung/Extraction/Ersatz von basierend auf verschiedene Attribute für Datenquellen sind möglich. 

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ                      | Beschreibung               |
|:----------------------|:--------------------------|:--------------------------|
|Ausdruck             |String                     |Entsprechende Ausdruck Darstellung dieses **AttributeMappingSource** -Objekts.|
|name                   |String                     |Name-Parameter der Zuordnungsquelle. Je nach der Wert der **Type** -Eigenschaft kann dies der Name der Funktion, die den Namen der Source-Attribut oder einen konstanten Wert geeignet sein. |
|parameters             |[StringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) -Auflistung | Wenn dieses Objekt eine Funktion darstellt, werden Funktionsparameter aufgelistet. Parameter bestehen aus **AttributeMappingSource** Objekte selbst komplexe Ausdrücke zulassen. **Typ** ist nicht `Function`, wird diese Eigenschaft Array Null/leer sein. |
|type                   | String                    |Der Typ des in diesem Attribut Zuordnungsquelle. Mögliche Werte sind: `Attribute`, `Constant` und `Function`. Der Standardwert lautet `Attribute`.| 

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a>Beispiele für JSON

Einfache-Attribut zum Zuordnen

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

Extrahieren von ersten 8 Zeichen aus dem Ausdruck

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
