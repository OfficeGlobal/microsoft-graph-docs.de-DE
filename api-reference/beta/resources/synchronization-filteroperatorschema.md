---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
localization_priority: Normal
ms.openlocfilehash: 0d26fb58b77369b70ab185fa8ad5214d6b6c1e71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848279"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="c13bf-103">Ressourcentyp filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="c13bf-103">filterOperatorSchema resource type</span></span>

> <span data-ttu-id="c13bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c13bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c13bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c13bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c13bf-106">Beschreibt einen Operator, der in einem [Filter](synchronization-filter.md)verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="c13bf-106">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c13bf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c13bf-107">Properties</span></span>

| <span data-ttu-id="c13bf-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c13bf-108">Property</span></span>                   | <span data-ttu-id="c13bf-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c13bf-109">Type</span></span>                      | <span data-ttu-id="c13bf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c13bf-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="c13bf-111">Stelligkeit</span><span class="sxs-lookup"><span data-stu-id="c13bf-111">arity</span></span>                       |<span data-ttu-id="c13bf-112">String</span><span class="sxs-lookup"><span data-stu-id="c13bf-112">String</span></span>          |<span data-ttu-id="c13bf-113">Stelligkeit des Operators.</span><span class="sxs-lookup"><span data-stu-id="c13bf-113">Arity of the operator.</span></span> <span data-ttu-id="c13bf-114">Mögliche Werte sind: `Binary` und `Unary`.</span><span class="sxs-lookup"><span data-stu-id="c13bf-114">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="c13bf-115">Der Standardwert ist `Binary`.</span><span class="sxs-lookup"><span data-stu-id="c13bf-115">The default is `Binary`.</span></span>|
|<span data-ttu-id="c13bf-116">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="c13bf-116">multivaluedComparisonType</span></span>   |<span data-ttu-id="c13bf-117">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="c13bf-117">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="c13bf-118">Mögliche Werte sind: `All` und `Any`.</span><span class="sxs-lookup"><span data-stu-id="c13bf-118">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="c13bf-119">Gilt nur für mehrwertige Attribute.</span><span class="sxs-lookup"><span data-stu-id="c13bf-119">Applies only to multivalued attributes.</span></span> <span data-ttu-id="c13bf-120">`All`bedeutet, dass alle Werte, die die Bedingung erfüllen müssen.</span><span class="sxs-lookup"><span data-stu-id="c13bf-120">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="c13bf-121">`Any`bedeutet, dass mindestens ein Wert hat, um die Bedingung zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="c13bf-121">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="c13bf-122">Der Standardwert ist `All`.</span><span class="sxs-lookup"><span data-stu-id="c13bf-122">The default is `All`.</span></span>|
|<span data-ttu-id="c13bf-123">name</span><span class="sxs-lookup"><span data-stu-id="c13bf-123">name</span></span>                        |<span data-ttu-id="c13bf-124">String</span><span class="sxs-lookup"><span data-stu-id="c13bf-124">String</span></span>                     |<span data-ttu-id="c13bf-125">Name des Operators.</span><span class="sxs-lookup"><span data-stu-id="c13bf-125">Operator name.</span></span> |
|<span data-ttu-id="c13bf-126">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="c13bf-126">supportedAttributeTypes</span></span>     |<span data-ttu-id="c13bf-127">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c13bf-127">String collection</span></span>         |<span data-ttu-id="c13bf-128">Attribut Typen, die vom Operator unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c13bf-128">Attribute types supported by the operator.</span></span> <span data-ttu-id="c13bf-129">Mögliche Werte sind: `Boolean`, `Binary`, `Reference`, `Integer` und `String`.</span><span class="sxs-lookup"><span data-stu-id="c13bf-129">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c13bf-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c13bf-130">JSON representation</span></span>

<span data-ttu-id="c13bf-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c13bf-131">The following is a JSON representation of the resource.</span></span>

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
