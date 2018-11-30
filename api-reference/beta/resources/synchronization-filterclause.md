---
title: FilterClause Ressourcentyp
description: Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).
ms.openlocfilehash: 0861324849f224c4e750f0c7b926464280b9a377
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059365"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="5af04-103">FilterClause Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5af04-103">filterClause resource type</span></span>

> <span data-ttu-id="5af04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5af04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5af04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5af04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5af04-106">Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).</span><span class="sxs-lookup"><span data-stu-id="5af04-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="5af04-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5af04-107">Properties</span></span>
| <span data-ttu-id="5af04-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5af04-108">Property</span></span>     | <span data-ttu-id="5af04-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5af04-109">Type</span></span>   |<span data-ttu-id="5af04-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5af04-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5af04-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="5af04-111">operatorName</span></span>|<span data-ttu-id="5af04-112">String</span><span class="sxs-lookup"><span data-stu-id="5af04-112">String</span></span>|<span data-ttu-id="5af04-113">Name des Operators auf den Quell- und Ziel-Operanden angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5af04-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="5af04-114">Einer der unterstützten Operatoren muss sein.</span><span class="sxs-lookup"><span data-stu-id="5af04-114">Must be one of the supported operators.</span></span> <span data-ttu-id="5af04-115">Unterstützte Operatoren können ermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="5af04-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="5af04-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="5af04-116">sourceOperandName</span></span>|<span data-ttu-id="5af04-117">String</span><span class="sxs-lookup"><span data-stu-id="5af04-117">String</span></span>|<span data-ttu-id="5af04-118">Name der Datenquelle Operand (Operand getesteten).</span><span class="sxs-lookup"><span data-stu-id="5af04-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="5af04-119">Der Name der Operand muss einem den Attributnamen im Quellobjekt übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="5af04-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="5af04-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="5af04-120">targetOperand</span></span>|[<span data-ttu-id="5af04-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="5af04-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="5af04-122">Werte, denen mit der Quelloperanden getestet wird.</span><span class="sxs-lookup"><span data-stu-id="5af04-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5af04-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5af04-123">JSON representation</span></span>

<span data-ttu-id="5af04-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5af04-124">The following is a JSON representation of the resource.</span></span>

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