---
title: Ressourcentyp attributeMappingFunctionSchema
description: Beschreibt eine Funktion, die in eine Zuordnung Attribut verwendet werden kann, während der Synchronisierung Werte umgewandelt.
localization_priority: Normal
ms.openlocfilehash: 7273534d281d8ea5eaf3709b530776295cd9c767
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822162"
---
# <a name="attributemappingfunctionschema-resource-type"></a>Ressourcentyp attributeMappingFunctionSchema

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Beschreibt eine Funktion, die in eine [Zuordnung zwischen Attributen](synchronization-attributemapping.md) verwendet werden kann, während der Synchronisierung Werte umgewandelt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | [AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung|Liste unterstützt Attribut Zuordnungsfunktionen.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:-------------------------|:---------------|
|name                        |Zeichenfolge                    |Name des Operators. |
|parameters                  |[AttributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) -Auflistung  |Auflistung von Funktionsparametern.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
