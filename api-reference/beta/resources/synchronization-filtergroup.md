---
title: Ressourcentyp filterGroup
description: Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514187"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="eed90-104">Ressourcentyp filterGroup</span><span class="sxs-lookup"><span data-stu-id="eed90-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eed90-105">Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden.</span><span class="sxs-lookup"><span data-stu-id="eed90-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="eed90-106">Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.</span><span class="sxs-lookup"><span data-stu-id="eed90-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="eed90-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eed90-107">Properties</span></span>
| <span data-ttu-id="eed90-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eed90-108">Property</span></span>     | <span data-ttu-id="eed90-109">Typ</span><span class="sxs-lookup"><span data-stu-id="eed90-109">Type</span></span>   |<span data-ttu-id="eed90-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eed90-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eed90-111">Klauseln</span><span class="sxs-lookup"><span data-stu-id="eed90-111">clauses</span></span>|<span data-ttu-id="eed90-112">[FilterClause](synchronization-filterclause.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="eed90-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="eed90-113">Filtert Klauseln (Conditions) dieser Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="eed90-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="eed90-114">Alle Klauseln in einer Gruppe eingehalten werden müssen, in der Reihenfolge für die Filtergruppe ergibt `true`.</span><span class="sxs-lookup"><span data-stu-id="eed90-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="eed90-115">name</span><span class="sxs-lookup"><span data-stu-id="eed90-115">name</span></span>|<span data-ttu-id="eed90-116">String</span><span class="sxs-lookup"><span data-stu-id="eed90-116">String</span></span>|<span data-ttu-id="eed90-117">Lesbare Namen der Filtergruppe.</span><span class="sxs-lookup"><span data-stu-id="eed90-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eed90-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eed90-118">JSON representation</span></span>

<span data-ttu-id="eed90-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eed90-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
