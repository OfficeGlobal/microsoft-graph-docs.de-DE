---
title: Filtertyp-Ressource
description: Bestimmt, welche Objekte für die Anwendung bereitgestellt werden soll. Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden. Wenn ein Filter Gültigkeitsbereichs vorhanden ist, werden Objekte, die nicht den Filter erfüllen während der Synchronisierung übersprungen.
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894411"
---
# <a name="filter-resource-type"></a><span data-ttu-id="6756d-105">Filtertyp-Ressource</span><span class="sxs-lookup"><span data-stu-id="6756d-105">filter resource type</span></span>

> <span data-ttu-id="6756d-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6756d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6756d-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6756d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6756d-108">Bestimmt, welche Objekte für die Anwendung bereitgestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="6756d-108">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="6756d-109">Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden.</span><span class="sxs-lookup"><span data-stu-id="6756d-109">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="6756d-110">Wenn ein Filter Gültigkeitsbereichs vorhanden ist, werden Objekte, die nicht den Filter erfüllen während der Synchronisierung übersprungen.</span><span class="sxs-lookup"><span data-stu-id="6756d-110">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="6756d-111">Filter ist Teil der [Objekt-Zuordnung](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="6756d-111">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="6756d-112">Es besteht aus mehreren Gruppen Filter aus, und jeder Filtergruppe enthält eine oder mehrere Klauseln.</span><span class="sxs-lookup"><span data-stu-id="6756d-112">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="6756d-113">Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.</span><span class="sxs-lookup"><span data-stu-id="6756d-113">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="6756d-114">Ein Objekt gilt im Bereich für die Gruppe ein (Gruppe ausgewertet wird, um `true`), wenn die Gruppen in der Gruppe wird ausgewertet `true`.</span><span class="sxs-lookup"><span data-stu-id="6756d-114">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="6756d-115">Weitere Informationen finden Sie unter [attributbasierte Anwendung provisioning mit Gültigkeitsbereichs Filter](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="6756d-115">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="6756d-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6756d-116">Properties</span></span>
| <span data-ttu-id="6756d-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6756d-117">Property</span></span>     | <span data-ttu-id="6756d-118">Typ</span><span class="sxs-lookup"><span data-stu-id="6756d-118">Type</span></span>   |<span data-ttu-id="6756d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6756d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6756d-120">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="6756d-120">categoryFilterGroups</span></span>|<span data-ttu-id="6756d-121">[FilterGroup](synchronization-filtergroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6756d-121">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="6756d-122">`*Experimental*`Filter für Gruppe festgelegt werden, ob die angegebene Objekt gehört und im Rahmen dieser Zuordnung Objekt verarbeitet werden soll.</span><span class="sxs-lookup"><span data-stu-id="6756d-122">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="6756d-123">Ein Objekt gilt im Bereich \*, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` \*.</span><span class="sxs-lookup"><span data-stu-id="6756d-123">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="6756d-124">Gruppen</span><span class="sxs-lookup"><span data-stu-id="6756d-124">groups</span></span>|<span data-ttu-id="6756d-125">[FilterGroup](synchronization-filtergroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6756d-125">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="6756d-126">Filter verwendet, um zu entscheiden, ob das angegebene Objekt in den Bereich für die Bereitstellung ist Gruppe festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6756d-126">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="6756d-127">**Dies ist der Filter, die in den meisten Fällen verwendet werden soll**.</span><span class="sxs-lookup"><span data-stu-id="6756d-127">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="6756d-128">Wenn ein Objekt verwendet, um diesen Filter zu einem bestimmten Zeitpunkt, zu erfüllen und klicken Sie dann auf das Objekt oder die Filter geändert wurde, sodass dieser Filter nicht ist mehr, entsprechendes Objekt erfüllt \* erhalten Ihre Bereitstellung ".</span><span class="sxs-lookup"><span data-stu-id="6756d-128">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="6756d-129">Ein Objekt gilt im Bereich \*, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` \*.</span><span class="sxs-lookup"><span data-stu-id="6756d-129">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="6756d-130">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="6756d-130">inputFilterGroups</span></span>|<span data-ttu-id="6756d-131">[FilterGroup](synchronization-filtergroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6756d-131">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="6756d-132">`*Experimental*`Filter zum Herausfiltern von Objekten im frühen Stadium aus dem Verzeichnis zu lesen Gruppe festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6756d-132">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="6756d-133">Wenn ein Objekt nicht diesen Filter entsprechen wird es nicht weiter verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="6756d-133">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="6756d-134">Wichtig zu verstehen, wenn ein Objekt verwendet, um diesen Filter zu einem bestimmten Zeitpunkt zu erfüllen, und klicken Sie dann das Objekt oder die Filter geändert wurde, ist dieser Filter nicht mehr erfüllt ist, das Objekt Netzwerktools *nicht Ihre Bereitstellung abgerufen wird*.</span><span class="sxs-lookup"><span data-stu-id="6756d-134">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="6756d-135">Ein Objekt gilt im Bereich \*, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` \*.</span><span class="sxs-lookup"><span data-stu-id="6756d-135">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6756d-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6756d-136">JSON representation</span></span>

<span data-ttu-id="6756d-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6756d-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
