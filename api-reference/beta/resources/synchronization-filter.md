---
title: Filter-Ressourcentyp
description: Bestimmt, welche Objekte für die Anwendung bereitgestellt werden soll. Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden. Wenn ein Filter Gültigkeitsbereichs vorhanden ist, werden Objekte, die nicht den Filter erfüllen während der Synchronisierung übersprungen.
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516679"
---
# <a name="filter-resource-type"></a><span data-ttu-id="76833-105">Filter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="76833-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76833-106">Bestimmt, welche Objekte für die Anwendung bereitgestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="76833-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="76833-107">Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden.</span><span class="sxs-lookup"><span data-stu-id="76833-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="76833-108">Wenn ein Filter Gültigkeitsbereichs vorhanden ist, werden Objekte, die nicht den Filter erfüllen während der Synchronisierung übersprungen.</span><span class="sxs-lookup"><span data-stu-id="76833-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="76833-109">Filter ist Teil der [Objekt-Zuordnung](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="76833-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="76833-110">Es besteht aus mehreren Gruppen Filter aus, und jeder Filtergruppe enthält eine oder mehrere Klauseln.</span><span class="sxs-lookup"><span data-stu-id="76833-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="76833-111">Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.</span><span class="sxs-lookup"><span data-stu-id="76833-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="76833-112">Ein Objekt gilt im Bereich für die Gruppe ein (Gruppe ausgewertet wird, um `true`), wenn die Gruppen in der Gruppe wird ausgewertet `true`.</span><span class="sxs-lookup"><span data-stu-id="76833-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="76833-113">Weitere Informationen finden Sie unter [attributbasierte Anwendung provisioning mit Gültigkeitsbereichs Filter](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="76833-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="76833-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="76833-114">Properties</span></span>
| <span data-ttu-id="76833-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76833-115">Property</span></span>     | <span data-ttu-id="76833-116">Typ</span><span class="sxs-lookup"><span data-stu-id="76833-116">Type</span></span>   |<span data-ttu-id="76833-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76833-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76833-118">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="76833-118">categoryFilterGroups</span></span>|<span data-ttu-id="76833-119">[FilterGroup](synchronization-filtergroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="76833-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="76833-120">`*Experimental*`Filter für Gruppe festgelegt werden, ob die angegebene Objekt gehört und im Rahmen dieser Zuordnung Objekt verarbeitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="76833-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="76833-121">Ein Objekt gilt im Bereich \*, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` \*.</span><span class="sxs-lookup"><span data-stu-id="76833-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="76833-122">Gruppen</span><span class="sxs-lookup"><span data-stu-id="76833-122">groups</span></span>|<span data-ttu-id="76833-123">[FilterGroup](synchronization-filtergroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="76833-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="76833-124">Filter verwendet, um zu entscheiden, ob das angegebene Objekt in den Bereich für die Bereitstellung ist Gruppe festgelegt.</span><span class="sxs-lookup"><span data-stu-id="76833-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="76833-125">**Dies ist der Filter, die in den meisten Fällen verwendet werden soll**.</span><span class="sxs-lookup"><span data-stu-id="76833-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="76833-126">Wenn ein Objekt verwendet, um diesen Filter zu einem bestimmten Zeitpunkt, zu erfüllen und klicken Sie dann auf das Objekt oder die Filter geändert wurde, sodass dieser Filter nicht ist mehr, entsprechendes Objekt erfüllt \* erhalten Ihre Bereitstellung ".</span><span class="sxs-lookup"><span data-stu-id="76833-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="76833-127">Ein Objekt gilt im Bereich \*, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` \*.</span><span class="sxs-lookup"><span data-stu-id="76833-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="76833-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="76833-128">inputFilterGroups</span></span>|<span data-ttu-id="76833-129">[FilterGroup](synchronization-filtergroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="76833-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="76833-130">`*Experimental*`Filter zum Herausfiltern von Objekten im frühen Stadium aus dem Verzeichnis zu lesen Gruppe festgelegt.</span><span class="sxs-lookup"><span data-stu-id="76833-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="76833-131">Wenn ein Objekt nicht diesen Filter entsprechen wird es nicht weiter verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="76833-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="76833-132">Wichtig zu verstehen, wenn ein Objekt verwendet, um diesen Filter zu einem bestimmten Zeitpunkt zu erfüllen, und klicken Sie dann das Objekt oder die Filter geändert wurde, ist dieser Filter nicht mehr erfüllt ist, das Objekt Netzwerktools *nicht Ihre Bereitstellung abgerufen wird*.</span><span class="sxs-lookup"><span data-stu-id="76833-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="76833-133">Ein Objekt gilt im Bereich \*, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` \*.</span><span class="sxs-lookup"><span data-stu-id="76833-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76833-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="76833-134">JSON representation</span></span>

<span data-ttu-id="76833-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="76833-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
