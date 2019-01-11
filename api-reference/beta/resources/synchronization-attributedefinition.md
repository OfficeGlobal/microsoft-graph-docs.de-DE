---
title: Attributdefinition Ressourcentyp
description: Beschreibt ein Attribut eines Objekts an.
localization_priority: Normal
ms.openlocfilehash: 63b7f67808ab6695b30f5464d72aed2814e46c5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829680"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="c44ab-103">Attributdefinition Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c44ab-103">attributeDefinition resource type</span></span>

> <span data-ttu-id="c44ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c44ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c44ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c44ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c44ab-106">Beschreibt ein Attribut eines Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c44ab-106">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="c44ab-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c44ab-107">Properties</span></span>

| <span data-ttu-id="c44ab-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c44ab-108">Property</span></span>      | <span data-ttu-id="c44ab-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c44ab-109">Type</span></span>      | <span data-ttu-id="c44ab-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c44ab-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c44ab-111">Anker</span><span class="sxs-lookup"><span data-stu-id="c44ab-111">anchor</span></span>         |<span data-ttu-id="c44ab-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c44ab-112">Boolean</span></span>    | <span data-ttu-id="c44ab-113">`true`Wenn das Attribut als Anker für das Objekt verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c44ab-113">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="c44ab-114">Anchor Attribute benötigen einen eindeutigen Wert, der ein Objekt identifiziert und unveränderlich sein müssen.</span><span class="sxs-lookup"><span data-stu-id="c44ab-114">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="c44ab-115">Der Standardwert lautet `false`.</span><span class="sxs-lookup"><span data-stu-id="c44ab-115">Default is `false`.</span></span> <span data-ttu-id="c44ab-116">Eine und nur ein einziges die Attribute des Objekts muss als Verankerung Unterstützung der Synchronisierung festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c44ab-116">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="c44ab-117">caseExact</span><span class="sxs-lookup"><span data-stu-id="c44ab-117">caseExact</span></span>      |<span data-ttu-id="c44ab-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c44ab-118">Boolean</span></span>    |<span data-ttu-id="c44ab-119">`true`Wenn der Wert dieses Attributs wie die Groß-/Kleinschreibung beachtet behandelt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c44ab-119">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="c44ab-120">Diese Einstellung wirkt sich auf wie das Synchronisierungsmodul Änderungen für das Attribut erkennt.</span><span class="sxs-lookup"><span data-stu-id="c44ab-120">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="c44ab-121">Metadaten</span><span class="sxs-lookup"><span data-stu-id="c44ab-121">metadata</span></span>       |[<span data-ttu-id="c44ab-122">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="c44ab-122">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="c44ab-123">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c44ab-123">Additional extension properties.</span></span> <span data-ttu-id="c44ab-124">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="c44ab-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c44ab-125">mehrwertige</span><span class="sxs-lookup"><span data-stu-id="c44ab-125">multivalued</span></span>    |<span data-ttu-id="c44ab-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c44ab-126">Boolean</span></span>    |<span data-ttu-id="c44ab-127">`true`Wenn ein Attribut mehrere Werte zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c44ab-127">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="c44ab-128">Der Standardwert lautet `false`.</span><span class="sxs-lookup"><span data-stu-id="c44ab-128">Default is `false`.</span></span>|
|<span data-ttu-id="c44ab-129">Veränderlichkeit</span><span class="sxs-lookup"><span data-stu-id="c44ab-129">mutability</span></span>     |<span data-ttu-id="c44ab-130">String</span><span class="sxs-lookup"><span data-stu-id="c44ab-130">String</span></span>     |<span data-ttu-id="c44ab-131">Ein Attribut Veränderlichkeit.</span><span class="sxs-lookup"><span data-stu-id="c44ab-131">An attribute's mutability.</span></span> <span data-ttu-id="c44ab-132">Mögliche Werte sind: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="c44ab-132">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="c44ab-133">Der Standardwert lautet `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="c44ab-133">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="c44ab-134">name</span><span class="sxs-lookup"><span data-stu-id="c44ab-134">name</span></span>           |<span data-ttu-id="c44ab-135">String</span><span class="sxs-lookup"><span data-stu-id="c44ab-135">String</span></span>     |<span data-ttu-id="c44ab-136">Name des Attributs.</span><span class="sxs-lookup"><span data-stu-id="c44ab-136">Name of the attribute.</span></span> <span data-ttu-id="c44ab-137">Muss innerhalb der Objektdefinition eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="c44ab-137">Must be unique within the object definition.</span></span> <span data-ttu-id="c44ab-138">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="c44ab-138">Not nullable.</span></span>|
|<span data-ttu-id="c44ab-139">erforderlich</span><span class="sxs-lookup"><span data-stu-id="c44ab-139">required</span></span>       |<span data-ttu-id="c44ab-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c44ab-140">Boolean</span></span>    |<span data-ttu-id="c44ab-141">`true`Wenn das Attribut erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c44ab-141">`true` if attribute is required.</span></span> <span data-ttu-id="c44ab-142">Objekt kann nicht erstellt werden, wenn die erforderlichen Attribute fehlen.</span><span class="sxs-lookup"><span data-stu-id="c44ab-142">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="c44ab-143">Wenn das required-Attribut während der Synchronisierung keinen Wert aufweist, wird der Standardwert verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c44ab-143">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="c44ab-144">Wenn der Standardwert nicht festgelegt wurde, wird die Synchronisierung einen Fehler aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="c44ab-144">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="c44ab-145">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="c44ab-145">referencedObjects</span></span>|[<span data-ttu-id="c44ab-146">referencedObject</span><span class="sxs-lookup"><span data-stu-id="c44ab-146">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="c44ab-147">Für Attribute mit `reference` eingeben, Listen die Objekte verwiesen wird (beispielsweise die `manager` Attribut würde auflisten `User` als das referenzierte Objekt).</span><span class="sxs-lookup"><span data-stu-id="c44ab-147">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="c44ab-148">type</span><span class="sxs-lookup"><span data-stu-id="c44ab-148">type</span></span>           |<span data-ttu-id="c44ab-149">String</span><span class="sxs-lookup"><span data-stu-id="c44ab-149">String</span></span>     |<span data-ttu-id="c44ab-150">Attributtyp Wert.</span><span class="sxs-lookup"><span data-stu-id="c44ab-150">Attribute value type.</span></span> <span data-ttu-id="c44ab-151">Mögliche Werte: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="c44ab-151">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="c44ab-152">Der Standardwert lautet `String`.</span><span class="sxs-lookup"><span data-stu-id="c44ab-152">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c44ab-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c44ab-153">JSON representation</span></span>

<span data-ttu-id="c44ab-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c44ab-154">The following is a JSON representation of the resource.</span></span>

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
