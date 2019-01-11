---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharepointIds
localization_priority: Normal
ms.openlocfilehash: ecbc5b4c3349333593730cb7b04c2eb5e5a1e4a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880262"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="10888-102">SharePointIds-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="10888-102">SharePointIds resource type</span></span>

<span data-ttu-id="10888-103">Die **SharePointIds**-Ressource gruppiert die verschiedenen Bezeichner für ein in einer SharePoint-Website oder auf OneDrive for Business gespeichertes Element in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="10888-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="10888-104">**Hinweis:** von OneDrive Personal zurückgegebene Elemente umfassen kein **SharePointIds**-Facet.</span><span class="sxs-lookup"><span data-stu-id="10888-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10888-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10888-105">JSON representation</span></span>

<span data-ttu-id="10888-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10888-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="10888-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10888-107">Properties</span></span>

| <span data-ttu-id="10888-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10888-108">Property</span></span>         | <span data-ttu-id="10888-109">Typ</span><span class="sxs-lookup"><span data-stu-id="10888-109">Type</span></span>         | <span data-ttu-id="10888-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10888-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="10888-111">listId</span><span class="sxs-lookup"><span data-stu-id="10888-111">listId</span></span>           | <span data-ttu-id="10888-112">string</span><span class="sxs-lookup"><span data-stu-id="10888-112">string</span></span>       | <span data-ttu-id="10888-113">Der eindeutige Bezeichner (GUID) für die Liste des Elements in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="10888-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="10888-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="10888-114">listItemId</span></span>       | <span data-ttu-id="10888-115">string</span><span class="sxs-lookup"><span data-stu-id="10888-115">string</span></span>       | <span data-ttu-id="10888-116">Ein ganzzahliger Bezeichner für das Element innerhalb der Liste.</span><span class="sxs-lookup"><span data-stu-id="10888-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="10888-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="10888-117">listItemUniqueId</span></span> | <span data-ttu-id="10888-118">string</span><span class="sxs-lookup"><span data-stu-id="10888-118">string</span></span>       | <span data-ttu-id="10888-119">Der eindeutige Bezeichner (GUID) für das Element in OneDrive for Business oder auf einer SharePoint-Website.</span><span class="sxs-lookup"><span data-stu-id="10888-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="10888-120">siteId</span><span class="sxs-lookup"><span data-stu-id="10888-120">siteId</span></span>           | <span data-ttu-id="10888-121">string</span><span class="sxs-lookup"><span data-stu-id="10888-121">string</span></span>       | <span data-ttu-id="10888-122">Der eindeutige Bezeichner (GUID) für die Websitesammlung (SPSite) des Elements.</span><span class="sxs-lookup"><span data-stu-id="10888-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="10888-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="10888-123">siteUrl</span></span>          | <span data-ttu-id="10888-124">string (URL)</span><span class="sxs-lookup"><span data-stu-id="10888-124">string (url)</span></span> | <span data-ttu-id="10888-125">Die SharePoint-URL für die Website, die das Element enthält.</span><span class="sxs-lookup"><span data-stu-id="10888-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="10888-126">webId</span><span class="sxs-lookup"><span data-stu-id="10888-126">webId</span></span>            | <span data-ttu-id="10888-127">string</span><span class="sxs-lookup"><span data-stu-id="10888-127">string</span></span>       | <span data-ttu-id="10888-128">Der eindeutige Bezeichner (GUID) für die Website (SPWeb) des Elements.</span><span class="sxs-lookup"><span data-stu-id="10888-128">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="10888-129">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="10888-129">Remarks</span></span>

<span data-ttu-id="10888-130">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="10888-130">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
