---
title: Ressourcentyp synchronizationRule
description: Definiert, wie die Synchronisierung für das Synchronisierungsmodul, einschließlich der zu synchronisierender Objekte und in welche Richtung ausgeführt werden sollen, wie Objekte in das Zielverzeichnis Objekte aus dem Quellverzeichnis zugeordnet werden soll und wie Attribute sollte transformiert werden, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517925"
---
# <a name="synchronizationrule-resource-type"></a>Ressourcentyp synchronizationRule

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Definiert, wie die Synchronisierung für das Synchronisierungsmodul, einschließlich der zu synchronisierender Objekte und in welche Richtung ausgeführt werden sollen, wie Objekte in das Zielverzeichnis Objekte aus dem Quellverzeichnis zugeordnet werden soll und wie Attribute sollte transformiert werden, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.

>**Hinweis:** Synchronisierungsregeln Definieren der Synchronisierung in einer Richtung - vom Quellverzeichnis in das Zielverzeichnis. Die Quell- und Ziel-Verzeichnisse werden als Teil der Regeleigenschaften definiert.

Synchronisierungsregeln werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung    |
|:--------------|:----------|:---------------|
|bearbeitet werden       |Boolescher Wert    |`true`Wenn die Synchronisierung Regel angepasst werden kann. `false` Wenn diese Regel schreibgeschützt ist und nicht geändert werden sollte.|
|id             |String     |Kennung für die Synchronisierung Regel. Einen der Bezeichner vom Synchronisierungsmodul erkannt muss werden. Unterstützt die Regel, die in der Synchronisierung-Vorlage, die von der API zurückgegebenen IDs gefunden werden können.|
|$metadata       |[StringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) -Auflistung |Zusätzliche Erweiterungseigenschaften. Wenn vom Supportteam explizit angewiesen, sollte Metadatenwerte nicht geändert werden.|
|name           |Zeichenfolge     |Lesbare Name der Regel Synchronisierung. Lässt keine NULL-Werte zu.|
|objectMappings |[ObjectMapping](synchronization-objectmapping.md) -Auflistung    |Auflistung von Objekt Zuordnungen von der Regel unterstützt. Weist das Synchronisierungsmodul welche Objekte synchronisiert werden sollen.|
|Priorität       |Ganze Zahl    |Priorität relativ zu anderen Regeln in der [SynchronizationSchema](synchronization-synchronizationschema.md). Regeln mit der niedrigsten Prioritätsnummer werden zuerst verarbeitet werden.|
|sourceDirectoryName       |String    |Name der Source-Verzeichnis. Muss eine der Definitionen in [SynchronizationSchema](synchronization-synchronizationschema.md)Verzeichnis übereinstimmen.|
|targetDirectoryName       |String    |Der Name des Zielverzeichnisses. Muss eine der Definitionen in [SynchronizationSchema](synchronization-synchronizationschema.md)Verzeichnis übereinstimmen.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
