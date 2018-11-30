---
title: Attributdefinition Ressourcentyp
description: Beschreibt ein Attribut eines Objekts an.
ms.openlocfilehash: 2199f8dbe5c528cf3b1b73f007fdae3451833815
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065007"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="5703e-103">Attributdefinition Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5703e-103">attributeDefinition resource type</span></span>

> <span data-ttu-id="5703e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5703e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5703e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5703e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5703e-106">Beschreibt ein Attribut eines Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5703e-106">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="5703e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5703e-107">Properties</span></span>

| <span data-ttu-id="5703e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5703e-108">Property</span></span>      | <span data-ttu-id="5703e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5703e-109">Type</span></span>      | <span data-ttu-id="5703e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5703e-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="5703e-111">Anker</span><span class="sxs-lookup"><span data-stu-id="5703e-111">anchor</span></span>         |<span data-ttu-id="5703e-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5703e-112">Boolean</span></span>    | <span data-ttu-id="5703e-113">`true`Wenn das Attribut als Anker für das Objekt verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5703e-113">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="5703e-114">Anchor Attribute benötigen einen eindeutigen Wert, der ein Objekt identifiziert und unveränderlich sein müssen.</span><span class="sxs-lookup"><span data-stu-id="5703e-114">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="5703e-115">Der Standardwert lautet `false`.</span><span class="sxs-lookup"><span data-stu-id="5703e-115">Default is `false`.</span></span> <span data-ttu-id="5703e-116">Eine und nur ein einziges die Attribute des Objekts muss als Verankerung Unterstützung der Synchronisierung festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="5703e-116">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="5703e-117">caseExact</span><span class="sxs-lookup"><span data-stu-id="5703e-117">caseExact</span></span>      |<span data-ttu-id="5703e-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5703e-118">Boolean</span></span>    |<span data-ttu-id="5703e-119">`true`Wenn der Wert dieses Attributs wie die Groß-/Kleinschreibung beachtet behandelt werden soll.</span><span class="sxs-lookup"><span data-stu-id="5703e-119">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="5703e-120">Diese Einstellung wirkt sich auf wie das Synchronisierungsmodul Änderungen für das Attribut erkennt.</span><span class="sxs-lookup"><span data-stu-id="5703e-120">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="5703e-121">Metadaten</span><span class="sxs-lookup"><span data-stu-id="5703e-121">metadata</span></span>       |[<span data-ttu-id="5703e-122">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="5703e-122">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="5703e-123">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="5703e-123">Additional extension properties.</span></span> <span data-ttu-id="5703e-124">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="5703e-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="5703e-125">mehrwertige</span><span class="sxs-lookup"><span data-stu-id="5703e-125">multivalued</span></span>    |<span data-ttu-id="5703e-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5703e-126">Boolean</span></span>    |<span data-ttu-id="5703e-127">`true`Wenn ein Attribut mehrere Werte zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="5703e-127">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="5703e-128">Der Standardwert lautet `false`.</span><span class="sxs-lookup"><span data-stu-id="5703e-128">Default is `false`.</span></span>|
|<span data-ttu-id="5703e-129">Veränderlichkeit</span><span class="sxs-lookup"><span data-stu-id="5703e-129">mutability</span></span>     |<span data-ttu-id="5703e-130">String</span><span class="sxs-lookup"><span data-stu-id="5703e-130">String</span></span>     |<span data-ttu-id="5703e-131">Ein Attribut Veränderlichkeit.</span><span class="sxs-lookup"><span data-stu-id="5703e-131">An attribute's mutability.</span></span> <span data-ttu-id="5703e-132">Mögliche Werte sind: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="5703e-132">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="5703e-133">Der Standardwert lautet `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="5703e-133">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="5703e-134">name</span><span class="sxs-lookup"><span data-stu-id="5703e-134">name</span></span>           |<span data-ttu-id="5703e-135">String</span><span class="sxs-lookup"><span data-stu-id="5703e-135">String</span></span>     |<span data-ttu-id="5703e-136">Name des Attributs.</span><span class="sxs-lookup"><span data-stu-id="5703e-136">Name of the attribute.</span></span> <span data-ttu-id="5703e-137">Muss innerhalb der Objektdefinition eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="5703e-137">Must be unique within the object definition.</span></span> <span data-ttu-id="5703e-138">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5703e-138">Not nullable.</span></span>|
|<span data-ttu-id="5703e-139">erforderlich</span><span class="sxs-lookup"><span data-stu-id="5703e-139">required</span></span>       |<span data-ttu-id="5703e-140">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5703e-140">Boolean</span></span>    |<span data-ttu-id="5703e-141">`true`Wenn das Attribut erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5703e-141">`true` if attribute is required.</span></span> <span data-ttu-id="5703e-142">Objekt kann nicht erstellt werden, wenn die erforderlichen Attribute fehlen.</span><span class="sxs-lookup"><span data-stu-id="5703e-142">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="5703e-143">Wenn das required-Attribut während der Synchronisierung keinen Wert aufweist, wird der Standardwert verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5703e-143">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="5703e-144">Wenn der Standardwert nicht festgelegt wurde, wird die Synchronisierung einen Fehler aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="5703e-144">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="5703e-145">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="5703e-145">referencedObjects</span></span>|[<span data-ttu-id="5703e-146">referencedObject</span><span class="sxs-lookup"><span data-stu-id="5703e-146">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="5703e-147">Für Attribute mit `reference` eingeben, Listen die Objekte verwiesen wird (beispielsweise die `manager` Attribut würde auflisten `User` als das referenzierte Objekt).</span><span class="sxs-lookup"><span data-stu-id="5703e-147">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="5703e-148">Typ</span><span class="sxs-lookup"><span data-stu-id="5703e-148">type</span></span>           |<span data-ttu-id="5703e-149">String</span><span class="sxs-lookup"><span data-stu-id="5703e-149">String</span></span>     |<span data-ttu-id="5703e-150">Attributtyp Wert.</span><span class="sxs-lookup"><span data-stu-id="5703e-150">Attribute value type.</span></span> <span data-ttu-id="5703e-151">Mögliche Werte: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="5703e-151">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="5703e-152">Der Standardwert lautet `String`.</span><span class="sxs-lookup"><span data-stu-id="5703e-152">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5703e-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5703e-153">JSON representation</span></span>

<span data-ttu-id="5703e-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5703e-154">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->