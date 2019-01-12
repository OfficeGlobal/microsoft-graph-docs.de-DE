---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharepointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 641b4f5b8d78a38324b7b19c9136e8a53532a9d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979936"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="90936-102">SharePointIds-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="90936-102">SharePointIds resource type</span></span>

> <span data-ttu-id="90936-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="90936-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90936-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90936-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90936-105">Die **SharePointIds**-Ressource gruppiert die verschiedenen Bezeichner für ein in einer SharePoint-Website oder auf OneDrive for Business gespeichertes Element in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="90936-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="90936-106">**Hinweis:** von OneDrive Personal zurückgegebene Elemente umfassen kein **SharePointIds**-Facet.</span><span class="sxs-lookup"><span data-stu-id="90936-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90936-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="90936-107">JSON representation</span></span>

<span data-ttu-id="90936-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="90936-108">Here is a JSON representation of the resource</span></span>

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
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="90936-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="90936-109">Properties</span></span>

| <span data-ttu-id="90936-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90936-110">Property</span></span>         | <span data-ttu-id="90936-111">Typ</span><span class="sxs-lookup"><span data-stu-id="90936-111">Type</span></span>         | <span data-ttu-id="90936-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90936-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="90936-113">listId</span><span class="sxs-lookup"><span data-stu-id="90936-113">listId</span></span>           | <span data-ttu-id="90936-114">string</span><span class="sxs-lookup"><span data-stu-id="90936-114">string</span></span>       | <span data-ttu-id="90936-115">Der eindeutige Bezeichner (GUID) für die Liste des Elements in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="90936-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="90936-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="90936-116">listItemId</span></span>       | <span data-ttu-id="90936-117">string</span><span class="sxs-lookup"><span data-stu-id="90936-117">string</span></span>       | <span data-ttu-id="90936-118">Ein ganzzahliger Bezeichner für das Element innerhalb der Liste.</span><span class="sxs-lookup"><span data-stu-id="90936-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="90936-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="90936-119">listItemUniqueId</span></span> | <span data-ttu-id="90936-120">string</span><span class="sxs-lookup"><span data-stu-id="90936-120">string</span></span>       | <span data-ttu-id="90936-121">Der eindeutige Bezeichner (GUID) für das Element in OneDrive for Business oder auf einer SharePoint-Website.</span><span class="sxs-lookup"><span data-stu-id="90936-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="90936-122">siteId</span><span class="sxs-lookup"><span data-stu-id="90936-122">siteId</span></span>           | <span data-ttu-id="90936-123">string</span><span class="sxs-lookup"><span data-stu-id="90936-123">string</span></span>       | <span data-ttu-id="90936-124">Der eindeutige Bezeichner (GUID) für die Websitesammlung (SPSite) des Elements.</span><span class="sxs-lookup"><span data-stu-id="90936-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="90936-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="90936-125">siteUrl</span></span>          | <span data-ttu-id="90936-126">string (URL)</span><span class="sxs-lookup"><span data-stu-id="90936-126">string (url)</span></span> | <span data-ttu-id="90936-127">Die SharePoint-URL für die Website, die das Element enthält.</span><span class="sxs-lookup"><span data-stu-id="90936-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="90936-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="90936-128">tenantId</span></span>         | <span data-ttu-id="90936-129">string</span><span class="sxs-lookup"><span data-stu-id="90936-129">string</span></span>       | <span data-ttu-id="90936-130">Der eindeutige Bezeichner (Guid) für die Instanz.</span><span class="sxs-lookup"><span data-stu-id="90936-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="90936-131">webId</span><span class="sxs-lookup"><span data-stu-id="90936-131">webId</span></span>            | <span data-ttu-id="90936-132">string</span><span class="sxs-lookup"><span data-stu-id="90936-132">string</span></span>       | <span data-ttu-id="90936-133">Der eindeutige Bezeichner (GUID) für die Website (SPWeb) des Elements.</span><span class="sxs-lookup"><span data-stu-id="90936-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="90936-134">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="90936-134">Remarks</span></span>

<span data-ttu-id="90936-135">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="90936-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
