---
title: Ressourcentyp filterGroup
description: Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.
ms.openlocfilehash: d49f7a4364f1d8ce3e1c4daba3bb331cf9a9c001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064279"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="5e792-104">Ressourcentyp filterGroup</span><span class="sxs-lookup"><span data-stu-id="5e792-104">filterGroup resource type</span></span>

> <span data-ttu-id="5e792-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5e792-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e792-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e792-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e792-107">Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden.</span><span class="sxs-lookup"><span data-stu-id="5e792-107">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="5e792-108">Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.</span><span class="sxs-lookup"><span data-stu-id="5e792-108">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="5e792-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5e792-109">Properties</span></span>
| <span data-ttu-id="5e792-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e792-110">Property</span></span>     | <span data-ttu-id="5e792-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5e792-111">Type</span></span>   |<span data-ttu-id="5e792-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e792-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e792-113">Klauseln</span><span class="sxs-lookup"><span data-stu-id="5e792-113">clauses</span></span>|<span data-ttu-id="5e792-114">[FilterClause](synchronization-filterclause.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5e792-114">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="5e792-115">Filtert Klauseln (Conditions) dieser Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="5e792-115">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="5e792-116">Alle Klauseln in einer Gruppe eingehalten werden müssen, in der Reihenfolge für die Filtergruppe ergibt `true`.</span><span class="sxs-lookup"><span data-stu-id="5e792-116">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="5e792-117">name</span><span class="sxs-lookup"><span data-stu-id="5e792-117">name</span></span>|<span data-ttu-id="5e792-118">String</span><span class="sxs-lookup"><span data-stu-id="5e792-118">String</span></span>|<span data-ttu-id="5e792-119">Lesbare Namen der Filtergruppe.</span><span class="sxs-lookup"><span data-stu-id="5e792-119">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e792-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5e792-120">JSON representation</span></span>

<span data-ttu-id="5e792-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5e792-121">The following is a JSON representation of the resource.</span></span>

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