---
title: FilterClause Ressourcentyp
description: Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523869"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="04db2-103">FilterClause Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="04db2-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04db2-104">Stellt eine einzelne Assertion, die ein Objekt Candidate erfüllen muss, und wird ausgewertet entweder `true` (Objekt erfüllt die Assertion) oder `false` (Objekt erfüllt die Assertion nicht).</span><span class="sxs-lookup"><span data-stu-id="04db2-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="04db2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04db2-105">Properties</span></span>
| <span data-ttu-id="04db2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04db2-106">Property</span></span>     | <span data-ttu-id="04db2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="04db2-107">Type</span></span>   |<span data-ttu-id="04db2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04db2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04db2-109">operatorName</span><span class="sxs-lookup"><span data-stu-id="04db2-109">operatorName</span></span>|<span data-ttu-id="04db2-110">String</span><span class="sxs-lookup"><span data-stu-id="04db2-110">String</span></span>|<span data-ttu-id="04db2-111">Name des Operators auf den Quell- und Ziel-Operanden angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="04db2-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="04db2-112">Einer der unterstützten Operatoren muss sein.</span><span class="sxs-lookup"><span data-stu-id="04db2-112">Must be one of the supported operators.</span></span> <span data-ttu-id="04db2-113">Unterstützte Operatoren können ermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="04db2-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="04db2-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="04db2-114">sourceOperandName</span></span>|<span data-ttu-id="04db2-115">String</span><span class="sxs-lookup"><span data-stu-id="04db2-115">String</span></span>|<span data-ttu-id="04db2-116">Name der Datenquelle Operand (Operand getesteten).</span><span class="sxs-lookup"><span data-stu-id="04db2-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="04db2-117">Der Name der Operand muss einem den Attributnamen im Quellobjekt übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="04db2-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="04db2-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="04db2-118">targetOperand</span></span>|[<span data-ttu-id="04db2-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="04db2-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="04db2-120">Werte, denen mit der Quelloperanden getestet wird.</span><span class="sxs-lookup"><span data-stu-id="04db2-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04db2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04db2-121">JSON representation</span></span>

<span data-ttu-id="04db2-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="04db2-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
