---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c9f4c3dc54b9eee6cc1ab24058e3fe238fed89a3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480600"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="530b0-102">SharePointIds-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="530b0-102">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="530b0-103">Die **SharePointIds**-Ressource gruppiert die verschiedenen Bezeichner für ein in einer SharePoint-Website oder auf OneDrive for Business gespeichertes Element in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="530b0-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="530b0-104">**Hinweis:** von OneDrive Personal zurückgegebene Elemente umfassen kein **SharePointIds**-Facet.</span><span class="sxs-lookup"><span data-stu-id="530b0-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="530b0-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="530b0-105">JSON representation</span></span>

<span data-ttu-id="530b0-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="530b0-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="530b0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="530b0-107">Properties</span></span>

| <span data-ttu-id="530b0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="530b0-108">Property</span></span>         | <span data-ttu-id="530b0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="530b0-109">Type</span></span>         | <span data-ttu-id="530b0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="530b0-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="530b0-111">listId</span><span class="sxs-lookup"><span data-stu-id="530b0-111">listId</span></span>           | <span data-ttu-id="530b0-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530b0-112">string</span></span>       | <span data-ttu-id="530b0-113">Der eindeutige Bezeichner (GUID) für die Liste des Elements in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="530b0-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="530b0-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="530b0-114">listItemId</span></span>       | <span data-ttu-id="530b0-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530b0-115">string</span></span>       | <span data-ttu-id="530b0-116">Ein ganzzahliger Bezeichner für das Element innerhalb der Liste.</span><span class="sxs-lookup"><span data-stu-id="530b0-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="530b0-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="530b0-117">listItemUniqueId</span></span> | <span data-ttu-id="530b0-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530b0-118">string</span></span>       | <span data-ttu-id="530b0-119">Der eindeutige Bezeichner (GUID) für das Element in OneDrive for Business oder auf einer SharePoint-Website.</span><span class="sxs-lookup"><span data-stu-id="530b0-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="530b0-120">siteId</span><span class="sxs-lookup"><span data-stu-id="530b0-120">siteId</span></span>           | <span data-ttu-id="530b0-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530b0-121">string</span></span>       | <span data-ttu-id="530b0-122">Der eindeutige Bezeichner (GUID) für die Websitesammlung (SPSite) des Elements.</span><span class="sxs-lookup"><span data-stu-id="530b0-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="530b0-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="530b0-123">siteUrl</span></span>          | <span data-ttu-id="530b0-124">string (URL)</span><span class="sxs-lookup"><span data-stu-id="530b0-124">string (url)</span></span> | <span data-ttu-id="530b0-125">Die SharePoint-URL für die Website, die das Element enthält.</span><span class="sxs-lookup"><span data-stu-id="530b0-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="530b0-126">tenantId</span><span class="sxs-lookup"><span data-stu-id="530b0-126">tenantId</span></span>         | <span data-ttu-id="530b0-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="530b0-127">string</span></span>       | <span data-ttu-id="530b0-128">Der eindeutige Bezeichner (GUID) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="530b0-128">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="530b0-129">webId</span><span class="sxs-lookup"><span data-stu-id="530b0-129">webId</span></span>            | <span data-ttu-id="530b0-130">string</span><span class="sxs-lookup"><span data-stu-id="530b0-130">string</span></span>       | <span data-ttu-id="530b0-131">Der eindeutige Bezeichner (GUID) für die Website (SPWeb) des Elements.</span><span class="sxs-lookup"><span data-stu-id="530b0-131">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="530b0-132">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="530b0-132">Remarks</span></span>

<span data-ttu-id="530b0-133">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="530b0-133">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepointids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
