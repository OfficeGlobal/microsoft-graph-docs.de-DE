---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharepointIds
ms.openlocfilehash: 28788090ccda113d6f4cd669e89777be84e6c2d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018222"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="301c8-102">SharePointIds-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="301c8-102">SharePointIds resource type</span></span>

<span data-ttu-id="301c8-103">Die **SharePointIds**-Ressource gruppiert die verschiedenen Bezeichner für ein in einer SharePoint-Website oder auf OneDrive for Business gespeichertes Element in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="301c8-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="301c8-104">**Hinweis:** von OneDrive Personal zurückgegebene Elemente umfassen kein **SharePointIds**-Facet.</span><span class="sxs-lookup"><span data-stu-id="301c8-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="301c8-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="301c8-105">JSON representation</span></span>

<span data-ttu-id="301c8-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="301c8-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="301c8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="301c8-107">Properties</span></span>

| <span data-ttu-id="301c8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="301c8-108">Property</span></span>         | <span data-ttu-id="301c8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="301c8-109">Type</span></span>         | <span data-ttu-id="301c8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="301c8-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="301c8-111">listId</span><span class="sxs-lookup"><span data-stu-id="301c8-111">listId</span></span>           | <span data-ttu-id="301c8-112">string</span><span class="sxs-lookup"><span data-stu-id="301c8-112">string</span></span>       | <span data-ttu-id="301c8-113">Der eindeutige Bezeichner (GUID) für die Liste des Elements in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="301c8-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="301c8-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="301c8-114">listItemId</span></span>       | <span data-ttu-id="301c8-115">string</span><span class="sxs-lookup"><span data-stu-id="301c8-115">string</span></span>       | <span data-ttu-id="301c8-116">Ein ganzzahliger Bezeichner für das Element innerhalb der Liste.</span><span class="sxs-lookup"><span data-stu-id="301c8-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="301c8-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="301c8-117">listItemUniqueId</span></span> | <span data-ttu-id="301c8-118">string</span><span class="sxs-lookup"><span data-stu-id="301c8-118">string</span></span>       | <span data-ttu-id="301c8-119">Der eindeutige Bezeichner (GUID) für das Element in OneDrive for Business oder auf einer SharePoint-Website.</span><span class="sxs-lookup"><span data-stu-id="301c8-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="301c8-120">siteId</span><span class="sxs-lookup"><span data-stu-id="301c8-120">siteId</span></span>           | <span data-ttu-id="301c8-121">string</span><span class="sxs-lookup"><span data-stu-id="301c8-121">string</span></span>       | <span data-ttu-id="301c8-122">Der eindeutige Bezeichner (GUID) für die Websitesammlung (SPSite) des Elements.</span><span class="sxs-lookup"><span data-stu-id="301c8-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="301c8-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="301c8-123">siteUrl</span></span>          | <span data-ttu-id="301c8-124">string (URL)</span><span class="sxs-lookup"><span data-stu-id="301c8-124">string (url)</span></span> | <span data-ttu-id="301c8-125">Die SharePoint-URL für die Website, die das Element enthält.</span><span class="sxs-lookup"><span data-stu-id="301c8-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="301c8-126">webId</span><span class="sxs-lookup"><span data-stu-id="301c8-126">webId</span></span>            | <span data-ttu-id="301c8-127">string</span><span class="sxs-lookup"><span data-stu-id="301c8-127">string</span></span>       | <span data-ttu-id="301c8-128">Der eindeutige Bezeichner (GUID) für die Website (SPWeb) des Elements.</span><span class="sxs-lookup"><span data-stu-id="301c8-128">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="301c8-129">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="301c8-129">Remarks</span></span>

<span data-ttu-id="301c8-130">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="301c8-130">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
