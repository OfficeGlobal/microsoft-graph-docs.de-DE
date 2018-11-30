---
title: Ressourcentyp synchronizationRule
description: Definiert, wie die Synchronisierung für das Synchronisierungsmodul, einschließlich der zu synchronisierender Objekte und in welche Richtung ausgeführt werden sollen, wie Objekte in das Zielverzeichnis Objekte aus dem Quellverzeichnis zugeordnet werden soll und wie Attribute sollte transformiert werden, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060078"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="4e221-103">Ressourcentyp synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="4e221-103">synchronizationRule resource type</span></span>

> <span data-ttu-id="4e221-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e221-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e221-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e221-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e221-106">Definiert, wie die Synchronisierung für das Synchronisierungsmodul, einschließlich der zu synchronisierender Objekte und in welche Richtung ausgeführt werden sollen, wie Objekte in das Zielverzeichnis Objekte aus dem Quellverzeichnis zugeordnet werden soll und wie Attribute sollte transformiert werden, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.</span><span class="sxs-lookup"><span data-stu-id="4e221-106">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="4e221-107">**Hinweis:** Synchronisierungsregeln Definieren der Synchronisierung in einer Richtung - vom Quellverzeichnis in das Zielverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4e221-107">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="4e221-108">Die Quell- und Ziel-Verzeichnisse werden als Teil der Regeleigenschaften definiert.</span><span class="sxs-lookup"><span data-stu-id="4e221-108">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="4e221-109">Synchronisierungsregeln werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4e221-109">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4e221-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e221-110">Properties</span></span>

| <span data-ttu-id="4e221-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e221-111">Property</span></span>      | <span data-ttu-id="4e221-112">Typ</span><span class="sxs-lookup"><span data-stu-id="4e221-112">Type</span></span>      | <span data-ttu-id="4e221-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e221-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4e221-114">bearbeitet werden</span><span class="sxs-lookup"><span data-stu-id="4e221-114">editable</span></span>       |<span data-ttu-id="4e221-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4e221-115">Boolean</span></span>    |<span data-ttu-id="4e221-116">`true`Wenn die Synchronisierung Regel angepasst werden kann. `false` Wenn diese Regel schreibgeschützt ist und nicht geändert werden sollte.</span><span class="sxs-lookup"><span data-stu-id="4e221-116">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="4e221-117">id</span><span class="sxs-lookup"><span data-stu-id="4e221-117">id</span></span>             |<span data-ttu-id="4e221-118">String</span><span class="sxs-lookup"><span data-stu-id="4e221-118">String</span></span>     |<span data-ttu-id="4e221-119">Kennung für die Synchronisierung Regel.</span><span class="sxs-lookup"><span data-stu-id="4e221-119">Synchronization rule identifier.</span></span> <span data-ttu-id="4e221-120">Einen der Bezeichner vom Synchronisierungsmodul erkannt muss werden.</span><span class="sxs-lookup"><span data-stu-id="4e221-120">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="4e221-121">Unterstützt die Regel, die in der Synchronisierung-Vorlage, die von der API zurückgegebenen IDs gefunden werden können.</span><span class="sxs-lookup"><span data-stu-id="4e221-121">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="4e221-122">Metadaten</span><span class="sxs-lookup"><span data-stu-id="4e221-122">metadata</span></span>       |<span data-ttu-id="4e221-123">[StringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4e221-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="4e221-124">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4e221-124">Additional extension properties.</span></span> <span data-ttu-id="4e221-125">Wenn vom Supportteam explizit angewiesen, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="4e221-125">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4e221-126">name</span><span class="sxs-lookup"><span data-stu-id="4e221-126">name</span></span>           |<span data-ttu-id="4e221-127">String</span><span class="sxs-lookup"><span data-stu-id="4e221-127">String</span></span>     |<span data-ttu-id="4e221-128">Lesbare Name der Regel Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="4e221-128">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="4e221-129">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4e221-129">Not nullable.</span></span>|
|<span data-ttu-id="4e221-130">objectMappings</span><span class="sxs-lookup"><span data-stu-id="4e221-130">objectMappings</span></span> |<span data-ttu-id="4e221-131">[ObjectMapping](synchronization-objectmapping.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4e221-131">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="4e221-132">Auflistung von Objekt Zuordnungen von der Regel unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e221-132">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="4e221-133">Weist das Synchronisierungsmodul welche Objekte synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4e221-133">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="4e221-134">Priorität</span><span class="sxs-lookup"><span data-stu-id="4e221-134">priority</span></span>       |<span data-ttu-id="4e221-135">Ganze Zahl</span><span class="sxs-lookup"><span data-stu-id="4e221-135">Integer</span></span>    |<span data-ttu-id="4e221-136">Priorität relativ zu anderen Regeln in der [SynchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="4e221-136">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="4e221-137">Regeln mit der niedrigsten Prioritätsnummer werden zuerst verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="4e221-137">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="4e221-138">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="4e221-138">sourceDirectoryName</span></span>       |<span data-ttu-id="4e221-139">String</span><span class="sxs-lookup"><span data-stu-id="4e221-139">String</span></span>    |<span data-ttu-id="4e221-140">Name der Source-Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4e221-140">Name of the source directory.</span></span> <span data-ttu-id="4e221-141">Muss eine der Definitionen in [SynchronizationSchema](synchronization-synchronizationschema.md)Verzeichnis übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="4e221-141">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="4e221-142">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="4e221-142">targetDirectoryName</span></span>       |<span data-ttu-id="4e221-143">String</span><span class="sxs-lookup"><span data-stu-id="4e221-143">String</span></span>    |<span data-ttu-id="4e221-144">Der Name des Zielverzeichnisses.</span><span class="sxs-lookup"><span data-stu-id="4e221-144">Name of the target directory.</span></span> <span data-ttu-id="4e221-145">Muss eine der Definitionen in [SynchronizationSchema](synchronization-synchronizationschema.md)Verzeichnis übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="4e221-145">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e221-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e221-146">JSON representation</span></span>

<span data-ttu-id="4e221-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e221-147">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->