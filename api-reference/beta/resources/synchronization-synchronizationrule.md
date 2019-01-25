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
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="4d82e-103">Ressourcentyp synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="4d82e-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d82e-104">Definiert, wie die Synchronisierung für das Synchronisierungsmodul, einschließlich der zu synchronisierender Objekte und in welche Richtung ausgeführt werden sollen, wie Objekte in das Zielverzeichnis Objekte aus dem Quellverzeichnis zugeordnet werden soll und wie Attribute sollte transformiert werden, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.</span><span class="sxs-lookup"><span data-stu-id="4d82e-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="4d82e-105">**Hinweis:** Synchronisierungsregeln Definieren der Synchronisierung in einer Richtung - vom Quellverzeichnis in das Zielverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4d82e-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="4d82e-106">Die Quell- und Ziel-Verzeichnisse werden als Teil der Regeleigenschaften definiert.</span><span class="sxs-lookup"><span data-stu-id="4d82e-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="4d82e-107">Synchronisierungsregeln werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4d82e-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d82e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d82e-108">Properties</span></span>

| <span data-ttu-id="4d82e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d82e-109">Property</span></span>      | <span data-ttu-id="4d82e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4d82e-110">Type</span></span>      | <span data-ttu-id="4d82e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d82e-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4d82e-112">bearbeitet werden</span><span class="sxs-lookup"><span data-stu-id="4d82e-112">editable</span></span>       |<span data-ttu-id="4d82e-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4d82e-113">Boolean</span></span>    |<span data-ttu-id="4d82e-114">`true`Wenn die Synchronisierung Regel angepasst werden kann. `false` Wenn diese Regel schreibgeschützt ist und nicht geändert werden sollte.</span><span class="sxs-lookup"><span data-stu-id="4d82e-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="4d82e-115">id</span><span class="sxs-lookup"><span data-stu-id="4d82e-115">id</span></span>             |<span data-ttu-id="4d82e-116">String</span><span class="sxs-lookup"><span data-stu-id="4d82e-116">String</span></span>     |<span data-ttu-id="4d82e-117">Kennung für die Synchronisierung Regel.</span><span class="sxs-lookup"><span data-stu-id="4d82e-117">Synchronization rule identifier.</span></span> <span data-ttu-id="4d82e-118">Einen der Bezeichner vom Synchronisierungsmodul erkannt muss werden.</span><span class="sxs-lookup"><span data-stu-id="4d82e-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="4d82e-119">Unterstützt die Regel, die in der Synchronisierung-Vorlage, die von der API zurückgegebenen IDs gefunden werden können.</span><span class="sxs-lookup"><span data-stu-id="4d82e-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="4d82e-120">$metadata</span><span class="sxs-lookup"><span data-stu-id="4d82e-120">metadata</span></span>       |<span data-ttu-id="4d82e-121">[StringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4d82e-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="4d82e-122">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4d82e-122">Additional extension properties.</span></span> <span data-ttu-id="4d82e-123">Wenn vom Supportteam explizit angewiesen, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="4d82e-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4d82e-124">name</span><span class="sxs-lookup"><span data-stu-id="4d82e-124">name</span></span>           |<span data-ttu-id="4d82e-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d82e-125">String</span></span>     |<span data-ttu-id="4d82e-126">Lesbare Name der Regel Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="4d82e-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="4d82e-127">Lässt keine NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="4d82e-127">Not nullable.</span></span>|
|<span data-ttu-id="4d82e-128">objectMappings</span><span class="sxs-lookup"><span data-stu-id="4d82e-128">objectMappings</span></span> |<span data-ttu-id="4d82e-129">[ObjectMapping](synchronization-objectmapping.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4d82e-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="4d82e-130">Auflistung von Objekt Zuordnungen von der Regel unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d82e-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="4d82e-131">Weist das Synchronisierungsmodul welche Objekte synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4d82e-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="4d82e-132">Priorität</span><span class="sxs-lookup"><span data-stu-id="4d82e-132">priority</span></span>       |<span data-ttu-id="4d82e-133">Ganze Zahl</span><span class="sxs-lookup"><span data-stu-id="4d82e-133">Integer</span></span>    |<span data-ttu-id="4d82e-134">Priorität relativ zu anderen Regeln in der [SynchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="4d82e-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="4d82e-135">Regeln mit der niedrigsten Prioritätsnummer werden zuerst verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="4d82e-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="4d82e-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="4d82e-136">sourceDirectoryName</span></span>       |<span data-ttu-id="4d82e-137">String</span><span class="sxs-lookup"><span data-stu-id="4d82e-137">String</span></span>    |<span data-ttu-id="4d82e-138">Name der Source-Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4d82e-138">Name of the source directory.</span></span> <span data-ttu-id="4d82e-139">Muss eine der Definitionen in [SynchronizationSchema](synchronization-synchronizationschema.md)Verzeichnis übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="4d82e-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="4d82e-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="4d82e-140">targetDirectoryName</span></span>       |<span data-ttu-id="4d82e-141">String</span><span class="sxs-lookup"><span data-stu-id="4d82e-141">String</span></span>    |<span data-ttu-id="4d82e-142">Der Name des Zielverzeichnisses.</span><span class="sxs-lookup"><span data-stu-id="4d82e-142">Name of the target directory.</span></span> <span data-ttu-id="4d82e-143">Muss eine der Definitionen in [SynchronizationSchema](synchronization-synchronizationschema.md)Verzeichnis übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="4d82e-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d82e-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d82e-144">JSON representation</span></span>

<span data-ttu-id="4d82e-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d82e-145">The following is a JSON representation of the resource.</span></span>

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
