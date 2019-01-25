---
title: Attributdefinition Ressourcentyp
description: Beschreibt ein Attribut eines Objekts an.
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514341"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="c3ece-103">Attributdefinition Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c3ece-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3ece-104">Beschreibt ein Attribut eines Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c3ece-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="c3ece-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3ece-105">Properties</span></span>

| <span data-ttu-id="c3ece-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3ece-106">Property</span></span>      | <span data-ttu-id="c3ece-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c3ece-107">Type</span></span>      | <span data-ttu-id="c3ece-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3ece-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c3ece-109">Anchor</span><span class="sxs-lookup"><span data-stu-id="c3ece-109">anchor</span></span>         |<span data-ttu-id="c3ece-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c3ece-110">Boolean</span></span>    | <span data-ttu-id="c3ece-111">`true`Wenn das Attribut als Anker für das Objekt verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c3ece-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="c3ece-112">Anchor Attribute benötigen einen eindeutigen Wert, der ein Objekt identifiziert und unveränderlich sein müssen.</span><span class="sxs-lookup"><span data-stu-id="c3ece-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="c3ece-113">Der Standardwert lautet `false`.</span><span class="sxs-lookup"><span data-stu-id="c3ece-113">Default is `false`.</span></span> <span data-ttu-id="c3ece-114">Eine und nur ein einziges die Attribute des Objekts muss als Verankerung Unterstützung der Synchronisierung festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c3ece-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="c3ece-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="c3ece-115">caseExact</span></span>      |<span data-ttu-id="c3ece-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c3ece-116">Boolean</span></span>    |<span data-ttu-id="c3ece-117">`true`Wenn der Wert dieses Attributs wie die Groß-/Kleinschreibung beachtet behandelt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c3ece-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="c3ece-118">Diese Einstellung wirkt sich auf wie das Synchronisierungsmodul Änderungen für das Attribut erkennt.</span><span class="sxs-lookup"><span data-stu-id="c3ece-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="c3ece-119">$metadata</span><span class="sxs-lookup"><span data-stu-id="c3ece-119">metadata</span></span>       |[<span data-ttu-id="c3ece-120">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="c3ece-120">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="c3ece-121">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c3ece-121">Additional extension properties.</span></span> <span data-ttu-id="c3ece-122">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="c3ece-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c3ece-123">Mehrwertig</span><span class="sxs-lookup"><span data-stu-id="c3ece-123">multivalued</span></span>    |<span data-ttu-id="c3ece-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c3ece-124">Boolean</span></span>    |<span data-ttu-id="c3ece-125">`true`Wenn ein Attribut mehrere Werte zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c3ece-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="c3ece-126">Der Standardwert lautet `false`.</span><span class="sxs-lookup"><span data-stu-id="c3ece-126">Default is `false`.</span></span>|
|<span data-ttu-id="c3ece-127">Veränderlichkeit</span><span class="sxs-lookup"><span data-stu-id="c3ece-127">mutability</span></span>     |<span data-ttu-id="c3ece-128">String</span><span class="sxs-lookup"><span data-stu-id="c3ece-128">String</span></span>     |<span data-ttu-id="c3ece-129">Ein Attribut Veränderlichkeit.</span><span class="sxs-lookup"><span data-stu-id="c3ece-129">An attribute's mutability.</span></span> <span data-ttu-id="c3ece-130">Mögliche Werte: sind `ReadWrite`, `ReadOnly`, `Immutable` und `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="c3ece-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="c3ece-131">Der Standardwert lautet `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="c3ece-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="c3ece-132">name</span><span class="sxs-lookup"><span data-stu-id="c3ece-132">name</span></span>           |<span data-ttu-id="c3ece-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3ece-133">String</span></span>     |<span data-ttu-id="c3ece-134">Name des Attributs.</span><span class="sxs-lookup"><span data-stu-id="c3ece-134">Name of the attribute.</span></span> <span data-ttu-id="c3ece-135">Muss innerhalb der Objektdefinition eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="c3ece-135">Must be unique within the object definition.</span></span> <span data-ttu-id="c3ece-136">Lässt keine NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="c3ece-136">Not nullable.</span></span>|
|<span data-ttu-id="c3ece-137">erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3ece-137">required</span></span>       |<span data-ttu-id="c3ece-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c3ece-138">Boolean</span></span>    |<span data-ttu-id="c3ece-139">`true`Wenn das Attribut erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c3ece-139">`true` if attribute is required.</span></span> <span data-ttu-id="c3ece-140">Objekt kann nicht erstellt werden, wenn die erforderlichen Attribute fehlen.</span><span class="sxs-lookup"><span data-stu-id="c3ece-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="c3ece-141">Wenn das required-Attribut während der Synchronisierung keinen Wert aufweist, wird der Standardwert verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c3ece-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="c3ece-142">Wenn der Standardwert nicht festgelegt wurde, wird die Synchronisierung einen Fehler aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="c3ece-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="c3ece-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="c3ece-143">referencedObjects</span></span>|[<span data-ttu-id="c3ece-144">referencedObject</span><span class="sxs-lookup"><span data-stu-id="c3ece-144">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="c3ece-145">Für Attribute mit `reference` eingeben, Listen die Objekte verwiesen wird (beispielsweise die `manager` Attribut würde auflisten `User` als das referenzierte Objekt).</span><span class="sxs-lookup"><span data-stu-id="c3ece-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="c3ece-146">type</span><span class="sxs-lookup"><span data-stu-id="c3ece-146">type</span></span>           |<span data-ttu-id="c3ece-147">String</span><span class="sxs-lookup"><span data-stu-id="c3ece-147">String</span></span>     |<span data-ttu-id="c3ece-148">Attributtyp Wert.</span><span class="sxs-lookup"><span data-stu-id="c3ece-148">Attribute value type.</span></span> <span data-ttu-id="c3ece-149">Mögliche Werte: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="c3ece-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="c3ece-150">Der Standardwert lautet `String`.</span><span class="sxs-lookup"><span data-stu-id="c3ece-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3ece-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3ece-151">JSON representation</span></span>

<span data-ttu-id="c3ece-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c3ece-152">The following is a JSON representation of the resource.</span></span>

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
