---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e9525882b08aaae5500ce23a4b54e95d0b0e0d65
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481804"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="6228b-102">SiteCollection-Ressource</span><span class="sxs-lookup"><span data-stu-id="6228b-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6228b-103">Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.</span><span class="sxs-lookup"><span data-stu-id="6228b-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="6228b-104">Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="6228b-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6228b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6228b-105">JSON representation</span></span>

<span data-ttu-id="6228b-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6228b-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6228b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6228b-107">Properties</span></span>

| <span data-ttu-id="6228b-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="6228b-108">Property name</span></span>        | <span data-ttu-id="6228b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6228b-109">Type</span></span>     | <span data-ttu-id="6228b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6228b-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="6228b-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="6228b-111">**hostname**</span></span>         | <span data-ttu-id="6228b-112">string</span><span class="sxs-lookup"><span data-stu-id="6228b-112">string</span></span>   | <span data-ttu-id="6228b-p101">Der Hostname der Websitesammlung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6228b-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="6228b-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="6228b-115">**dataLocationCode**</span></span> | <span data-ttu-id="6228b-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6228b-116">string</span></span>   | <span data-ttu-id="6228b-117">Der geographische Regionscode für die Position dieser Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="6228b-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="6228b-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6228b-118">Read-only.</span></span>
| <span data-ttu-id="6228b-119">**root**</span><span class="sxs-lookup"><span data-stu-id="6228b-119">**root**</span></span>             | <span data-ttu-id="6228b-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="6228b-120">[root][]</span></span> | <span data-ttu-id="6228b-121">Wenn vorhanden, gibt an, dass es sich um eine Stammwebsitesammlung in SharePoint handelt.</span><span class="sxs-lookup"><span data-stu-id="6228b-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="6228b-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6228b-122">Read-only.</span></span>

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
