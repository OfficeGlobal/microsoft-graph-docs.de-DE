---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515195"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="98494-103">Ressourcentyp filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="98494-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98494-104">Beschreibt einen Operator, der in einem [Filter](synchronization-filter.md)verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="98494-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="98494-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="98494-105">Properties</span></span>

| <span data-ttu-id="98494-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98494-106">Property</span></span>                   | <span data-ttu-id="98494-107">Typ</span><span class="sxs-lookup"><span data-stu-id="98494-107">Type</span></span>                      | <span data-ttu-id="98494-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98494-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="98494-109">Stelligkeit</span><span class="sxs-lookup"><span data-stu-id="98494-109">arity</span></span>                       |<span data-ttu-id="98494-110">String</span><span class="sxs-lookup"><span data-stu-id="98494-110">String</span></span>          |<span data-ttu-id="98494-111">Stelligkeit des Operators.</span><span class="sxs-lookup"><span data-stu-id="98494-111">Arity of the operator.</span></span> <span data-ttu-id="98494-112">Mögliche Werte sind: `Binary` und `Unary`.</span><span class="sxs-lookup"><span data-stu-id="98494-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="98494-113">Der Standardwert ist `Binary`.</span><span class="sxs-lookup"><span data-stu-id="98494-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="98494-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="98494-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="98494-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="98494-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="98494-116">Mögliche Werte sind: `All` und `Any`.</span><span class="sxs-lookup"><span data-stu-id="98494-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="98494-117">Gilt nur für mehrwertige Attribute.</span><span class="sxs-lookup"><span data-stu-id="98494-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="98494-118">`All`bedeutet, dass alle Werte, die die Bedingung erfüllen müssen.</span><span class="sxs-lookup"><span data-stu-id="98494-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="98494-119">`Any`bedeutet, dass mindestens ein Wert hat, um die Bedingung zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="98494-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="98494-120">Der Standardwert ist `All`.</span><span class="sxs-lookup"><span data-stu-id="98494-120">The default is `All`.</span></span>|
|<span data-ttu-id="98494-121">name</span><span class="sxs-lookup"><span data-stu-id="98494-121">name</span></span>                        |<span data-ttu-id="98494-122">String</span><span class="sxs-lookup"><span data-stu-id="98494-122">String</span></span>                     |<span data-ttu-id="98494-123">Name des Operators.</span><span class="sxs-lookup"><span data-stu-id="98494-123">Operator name.</span></span> |
|<span data-ttu-id="98494-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="98494-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="98494-125">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="98494-125">String collection</span></span>         |<span data-ttu-id="98494-126">Attribut Typen, die vom Operator unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98494-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="98494-127">Mögliche Werte sind: `Boolean`, `Binary`, `Reference`, `Integer` und `String`.</span><span class="sxs-lookup"><span data-stu-id="98494-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98494-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="98494-128">JSON representation</span></span>

<span data-ttu-id="98494-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="98494-129">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
