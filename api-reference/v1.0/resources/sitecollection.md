---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6fb5f05a1dbdf7485957bb4bf04db06432f17da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916985"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="cef25-102">SiteCollection-Ressource</span><span class="sxs-lookup"><span data-stu-id="cef25-102">SiteCollection resource</span></span>

<span data-ttu-id="cef25-103">Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.</span><span class="sxs-lookup"><span data-stu-id="cef25-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="cef25-104">Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="cef25-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cef25-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cef25-105">JSON representation</span></span>

<span data-ttu-id="cef25-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cef25-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="cef25-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cef25-107">Properties</span></span>

| <span data-ttu-id="cef25-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="cef25-108">Property name</span></span>        | <span data-ttu-id="cef25-109">Typ</span><span class="sxs-lookup"><span data-stu-id="cef25-109">Type</span></span>     | <span data-ttu-id="cef25-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cef25-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="cef25-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="cef25-111">**hostname**</span></span>         | <span data-ttu-id="cef25-112">string</span><span class="sxs-lookup"><span data-stu-id="cef25-112">string</span></span>   | <span data-ttu-id="cef25-p101">Der Hostname der Websitesammlung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cef25-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="cef25-115">**root**</span><span class="sxs-lookup"><span data-stu-id="cef25-115">**root**</span></span>             | <span data-ttu-id="cef25-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="cef25-116">[root][]</span></span> | <span data-ttu-id="cef25-117">Falls vorhanden, gibt an, dass dies eine Stammwebsitesammlung in SharePoint ist.</span><span class="sxs-lookup"><span data-stu-id="cef25-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="cef25-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cef25-118">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
