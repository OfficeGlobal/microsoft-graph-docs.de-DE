---
title: Ressourcentyp filterGroup
description: Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.
localization_priority: Normal
ms.openlocfilehash: 174c02518069e949c49887d9e21e778e8455509a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836113"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="f32f3-104">Ressourcentyp filterGroup</span><span class="sxs-lookup"><span data-stu-id="f32f3-104">filterGroup resource type</span></span>

> <span data-ttu-id="f32f3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f32f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f32f3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f32f3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f32f3-107">Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden.</span><span class="sxs-lookup"><span data-stu-id="f32f3-107">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="f32f3-108">Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.</span><span class="sxs-lookup"><span data-stu-id="f32f3-108">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="f32f3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f32f3-109">Properties</span></span>
| <span data-ttu-id="f32f3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f32f3-110">Property</span></span>     | <span data-ttu-id="f32f3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f32f3-111">Type</span></span>   |<span data-ttu-id="f32f3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f32f3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f32f3-113">Klauseln</span><span class="sxs-lookup"><span data-stu-id="f32f3-113">clauses</span></span>|<span data-ttu-id="f32f3-114">[FilterClause](synchronization-filterclause.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f32f3-114">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="f32f3-115">Filtert Klauseln (Conditions) dieser Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="f32f3-115">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="f32f3-116">Alle Klauseln in einer Gruppe eingehalten werden müssen, in der Reihenfolge für die Filtergruppe ergibt `true`.</span><span class="sxs-lookup"><span data-stu-id="f32f3-116">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="f32f3-117">name</span><span class="sxs-lookup"><span data-stu-id="f32f3-117">name</span></span>|<span data-ttu-id="f32f3-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f32f3-118">String</span></span>|<span data-ttu-id="f32f3-119">Lesbare Namen der Filtergruppe.</span><span class="sxs-lookup"><span data-stu-id="f32f3-119">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f32f3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f32f3-120">JSON representation</span></span>

<span data-ttu-id="f32f3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f32f3-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
