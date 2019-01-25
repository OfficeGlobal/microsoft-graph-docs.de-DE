---
title: Ressourcentyp attributeMappingFunctionSchema
description: Beschreibt eine Funktion, die in eine Zuordnung Attribut verwendet werden kann, während der Synchronisierung Werte umgewandelt.
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511982"
---
# <a name="attributemappingfunctionschema-resource-type"></a>Ressourcentyp attributeMappingFunctionSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt eine Funktion, die in eine [Zuordnung zwischen Attributen](synchronization-attributemapping.md) verwendet werden kann, während der Synchronisierung Werte umgewandelt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | [AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung|Liste unterstützt Attribut Zuordnungsfunktionen.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:-------------------------|:---------------|
|name                        |String                    |Name des Operators. |
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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingfunctionschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
