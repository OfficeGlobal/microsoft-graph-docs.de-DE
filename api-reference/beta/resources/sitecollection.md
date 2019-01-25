---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 865fc21691eb37811300caaf675b123d1a544ac0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528130"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="39731-102">SiteCollection-Ressource</span><span class="sxs-lookup"><span data-stu-id="39731-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39731-103">Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.</span><span class="sxs-lookup"><span data-stu-id="39731-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="39731-104">Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="39731-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39731-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="39731-105">JSON representation</span></span>

<span data-ttu-id="39731-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="39731-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="39731-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="39731-107">Properties</span></span>

| <span data-ttu-id="39731-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="39731-108">Property name</span></span>        | <span data-ttu-id="39731-109">Typ</span><span class="sxs-lookup"><span data-stu-id="39731-109">Type</span></span>     | <span data-ttu-id="39731-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39731-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="39731-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="39731-111">**hostname**</span></span>         | <span data-ttu-id="39731-112">string</span><span class="sxs-lookup"><span data-stu-id="39731-112">string</span></span>   | <span data-ttu-id="39731-p101">Der Hostname der Websitesammlung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="39731-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="39731-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="39731-115">**dataLocationCode**</span></span> | <span data-ttu-id="39731-116">string</span><span class="sxs-lookup"><span data-stu-id="39731-116">string</span></span>   | <span data-ttu-id="39731-117">Der Code geografische Region, in dem diese Websitesammlung befindet.</span><span class="sxs-lookup"><span data-stu-id="39731-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="39731-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="39731-118">Read-only.</span></span>
| <span data-ttu-id="39731-119">**root**</span><span class="sxs-lookup"><span data-stu-id="39731-119">**root**</span></span>             | <span data-ttu-id="39731-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="39731-120">[root][]</span></span> | <span data-ttu-id="39731-121">Falls vorhanden, gibt an, dass dies eine Stammwebsitesammlung in SharePoint ist.</span><span class="sxs-lookup"><span data-stu-id="39731-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="39731-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="39731-122">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sitecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
