---
title: FilterClause Ressourcentyp
description: Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833859"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="80d8b-103">FilterClause Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="80d8b-103">filterClause resource type</span></span>

> <span data-ttu-id="80d8b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80d8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80d8b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80d8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80d8b-106">Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).</span><span class="sxs-lookup"><span data-stu-id="80d8b-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="80d8b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80d8b-107">Properties</span></span>
| <span data-ttu-id="80d8b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80d8b-108">Property</span></span>     | <span data-ttu-id="80d8b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="80d8b-109">Type</span></span>   |<span data-ttu-id="80d8b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80d8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80d8b-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="80d8b-111">operatorName</span></span>|<span data-ttu-id="80d8b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80d8b-112">String</span></span>|<span data-ttu-id="80d8b-113">Name des Operators auf den Quell- und Ziel-Operanden angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="80d8b-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="80d8b-114">Einer der unterstützten Operatoren muss sein.</span><span class="sxs-lookup"><span data-stu-id="80d8b-114">Must be one of the supported operators.</span></span> <span data-ttu-id="80d8b-115">Unterstützte Operatoren können ermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="80d8b-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="80d8b-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="80d8b-116">sourceOperandName</span></span>|<span data-ttu-id="80d8b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80d8b-117">String</span></span>|<span data-ttu-id="80d8b-118">Name der Datenquelle Operand (Operand getesteten).</span><span class="sxs-lookup"><span data-stu-id="80d8b-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="80d8b-119">Der Name der Operand muss einem den Attributnamen im Quellobjekt übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="80d8b-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="80d8b-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="80d8b-120">targetOperand</span></span>|[<span data-ttu-id="80d8b-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="80d8b-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="80d8b-122">Werte, denen mit der Quelloperanden getestet wird.</span><span class="sxs-lookup"><span data-stu-id="80d8b-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80d8b-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80d8b-123">JSON representation</span></span>

<span data-ttu-id="80d8b-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80d8b-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
