---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059369"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="02953-103">Ressourcentyp filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="02953-103">filterOperatorSchema resource type</span></span>

> <span data-ttu-id="02953-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02953-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02953-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02953-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02953-106">Beschreibt einen Operator, der in einem [Filter](synchronization-filter.md)verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="02953-106">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="02953-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02953-107">Properties</span></span>

| <span data-ttu-id="02953-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02953-108">Property</span></span>                   | <span data-ttu-id="02953-109">Typ</span><span class="sxs-lookup"><span data-stu-id="02953-109">Type</span></span>                      | <span data-ttu-id="02953-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02953-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="02953-111">Stelligkeit</span><span class="sxs-lookup"><span data-stu-id="02953-111">arity</span></span>                       |<span data-ttu-id="02953-112">String</span><span class="sxs-lookup"><span data-stu-id="02953-112">String</span></span>          |<span data-ttu-id="02953-113">Stelligkeit des Operators.</span><span class="sxs-lookup"><span data-stu-id="02953-113">Arity of the operator.</span></span> <span data-ttu-id="02953-114">Mögliche Werte sind: `Binary` und `Unary`.</span><span class="sxs-lookup"><span data-stu-id="02953-114">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="02953-115">Der Standardwert ist `Binary`.</span><span class="sxs-lookup"><span data-stu-id="02953-115">The default is `Binary`.</span></span>|
|<span data-ttu-id="02953-116">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="02953-116">multivaluedComparisonType</span></span>   |<span data-ttu-id="02953-117">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="02953-117">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="02953-118">Mögliche Werte sind: `All` und `Any`.</span><span class="sxs-lookup"><span data-stu-id="02953-118">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="02953-119">Gilt nur für mehrwertige Attribute.</span><span class="sxs-lookup"><span data-stu-id="02953-119">Applies only to multivalued attributes.</span></span> <span data-ttu-id="02953-120">`All`bedeutet, dass alle Werte, die die Bedingung erfüllen müssen.</span><span class="sxs-lookup"><span data-stu-id="02953-120">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="02953-121">`Any`bedeutet, dass mindestens ein Wert hat, um die Bedingung zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="02953-121">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="02953-122">Der Standardwert ist `All`.</span><span class="sxs-lookup"><span data-stu-id="02953-122">The default is `All`.</span></span>|
|<span data-ttu-id="02953-123">name</span><span class="sxs-lookup"><span data-stu-id="02953-123">name</span></span>                        |<span data-ttu-id="02953-124">String</span><span class="sxs-lookup"><span data-stu-id="02953-124">String</span></span>                     |<span data-ttu-id="02953-125">Name des Operators.</span><span class="sxs-lookup"><span data-stu-id="02953-125">Operator name.</span></span> |
|<span data-ttu-id="02953-126">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="02953-126">supportedAttributeTypes</span></span>     |<span data-ttu-id="02953-127">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="02953-127">String collection</span></span>         |<span data-ttu-id="02953-128">Attribut Typen, die vom Operator unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02953-128">Attribute types supported by the operator.</span></span> <span data-ttu-id="02953-129">Mögliche Werte sind: `Boolean`, `Binary`, `Reference`, `Integer` und `String`.</span><span class="sxs-lookup"><span data-stu-id="02953-129">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02953-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02953-130">JSON representation</span></span>

<span data-ttu-id="02953-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02953-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->