---
title: Ressourcentyp filterOperatorSchema
description: Beschreibt einen Operator, der in einem Filter verwendet werden kann.
localization_priority: Normal
ms.openlocfilehash: 366e00b5d21efeaf67e3e799c5b1c2412a68e268
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573682"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="4b171-103">Ressourcentyp filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="4b171-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b171-104">Beschreibt einen Operator, der in einem [Filter](synchronization-filter.md)verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="4b171-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b171-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b171-105">Properties</span></span>

| <span data-ttu-id="4b171-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b171-106">Property</span></span>                   | <span data-ttu-id="4b171-107">Typ</span><span class="sxs-lookup"><span data-stu-id="4b171-107">Type</span></span>                      | <span data-ttu-id="4b171-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b171-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="4b171-109">Stelligkeit</span><span class="sxs-lookup"><span data-stu-id="4b171-109">arity</span></span>                       | <span data-ttu-id="4b171-110">microsoft.graph.scopeOperatorType</span><span class="sxs-lookup"><span data-stu-id="4b171-110">microsoft.graph.scopeOperatorType</span></span>         |<span data-ttu-id="4b171-111">Stelligkeit des Operators.</span><span class="sxs-lookup"><span data-stu-id="4b171-111">Arity of the operator.</span></span> <span data-ttu-id="4b171-112">Mögliche Werte sind: `Binary` und `Unary`.</span><span class="sxs-lookup"><span data-stu-id="4b171-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="4b171-113">Der Standardwert ist `Binary`.</span><span class="sxs-lookup"><span data-stu-id="4b171-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="4b171-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="4b171-114">multivaluedComparisonType</span></span>   | <span data-ttu-id="4b171-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="4b171-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="4b171-116">Mögliche Werte sind: `All` und `Any`.</span><span class="sxs-lookup"><span data-stu-id="4b171-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="4b171-117">Gilt nur für mehrwertige Attribute.</span><span class="sxs-lookup"><span data-stu-id="4b171-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="4b171-118">`All`bedeutet, dass alle Werte, die die Bedingung erfüllen müssen.</span><span class="sxs-lookup"><span data-stu-id="4b171-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="4b171-119">`Any`bedeutet, dass mindestens ein Wert hat, um die Bedingung zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="4b171-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="4b171-120">Der Standardwert ist `All`.</span><span class="sxs-lookup"><span data-stu-id="4b171-120">The default is `All`.</span></span>|
|<span data-ttu-id="4b171-121">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="4b171-121">supportedAttributeTypes</span></span>     | <span data-ttu-id="4b171-122">AttributeType-Auflistung</span><span class="sxs-lookup"><span data-stu-id="4b171-122">attributeType collection</span></span>         |<span data-ttu-id="4b171-123">Attribut Typen, die vom Operator unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b171-123">Attribute types supported by the operator.</span></span> <span data-ttu-id="4b171-124">Mögliche Werte sind: `Boolean`, `Binary`, `Reference`, `Integer` und `String`.</span><span class="sxs-lookup"><span data-stu-id="4b171-124">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b171-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b171-125">JSON representation</span></span>

<span data-ttu-id="4b171-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b171-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "microsoft.graph.scopeOperatorType",
  "multivaluedComparisonType": "microsoft.graph.scopeOperatorMultiValuedComparisonType",  
  "supportedAttributeTypes": ["attributeType"]
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
