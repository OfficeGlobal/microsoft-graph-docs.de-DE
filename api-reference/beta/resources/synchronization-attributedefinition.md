---
title: Attributdefinition Ressourcentyp
description: Beschreibt ein Attribut eines Objekts an.
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643916"
---
# <a name="attributedefinition-resource-type"></a>Attributdefinition Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt ein Attribut eines Objekts an.

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung    |
|:--------------|:----------|:---------------|
|Anker         |Boolean    | `true`Wenn das Attribut als Anker für das Objekt verwendet werden soll. Anchor Attribute benötigen einen eindeutigen Wert, der ein Objekt identifiziert und unveränderlich sein müssen. Der Standardwert lautet `false`. Eine und nur ein einziges die Attribute des Objekts muss als Verankerung Unterstützung der Synchronisierung festgelegt werden. |
|caseExact      |Boolean    |`true`Wenn der Wert dieses Attributs wie die Groß-/Kleinschreibung beachtet behandelt werden soll. Diese Einstellung wirkt sich auf wie das Synchronisierungsmodul Änderungen für das Attribut erkennt.|
|Metadaten       |[metadataEntry](../resources/synchronization-metadataentry.md)    |Zusätzliche Erweiterungseigenschaften. Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.|
|mehrwertige    |Boolean    |`true`Wenn ein Attribut mehrere Werte zulässig sind. Der Standardwert lautet `false`.|
|Veränderlichkeit     |String     |Ein Attribut Veränderlichkeit. Mögliche Werte sind: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`. Der Standardwert lautet `ReadWrite`.|
|name           |String     |Name des Attributs. Muss innerhalb der Objektdefinition eindeutig sein. Lässt keine Nullwerte zu.|
|erforderlich       |Boolean    |`true`Wenn das Attribut erforderlich ist. Objekt kann nicht erstellt werden, wenn die erforderlichen Attribute fehlen. Wenn das required-Attribut während der Synchronisierung keinen Wert aufweist, wird der Standardwert verwendet werden. Wenn der Standardwert nicht festgelegt wurde, wird die Synchronisierung einen Fehler aufgezeichnet.|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) |Für Attribute mit `reference` eingeben, Listen die Objekte verwiesen wird (beispielsweise die `manager` Attribut würde auflisten `User` als das referenzierte Objekt).|
|type           |String     |Attributtyp Wert. Mögliche Werte: `String`, `Integer`, `Reference`, `Binary`, `Boolean`. Der Standardwert lautet `String`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
