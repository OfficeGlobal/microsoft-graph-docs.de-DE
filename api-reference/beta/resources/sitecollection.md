---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: d54246002c158270ae23cf81cdc93673f40bd78c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061883"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="c708d-102">SiteCollection-Ressource</span><span class="sxs-lookup"><span data-stu-id="c708d-102">SiteCollection resource</span></span>

> <span data-ttu-id="c708d-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c708d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c708d-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c708d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c708d-105">Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.</span><span class="sxs-lookup"><span data-stu-id="c708d-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="c708d-106">Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="c708d-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c708d-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c708d-107">JSON representation</span></span>

<span data-ttu-id="c708d-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c708d-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c708d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c708d-109">Properties</span></span>

| <span data-ttu-id="c708d-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="c708d-110">Property name</span></span>        | <span data-ttu-id="c708d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c708d-111">Type</span></span>     | <span data-ttu-id="c708d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c708d-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="c708d-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="c708d-113">**hostname**</span></span>         | <span data-ttu-id="c708d-114">string</span><span class="sxs-lookup"><span data-stu-id="c708d-114">string</span></span>   | <span data-ttu-id="c708d-p102">Der Hostname der Websitesammlung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c708d-p102">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="c708d-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="c708d-117">**dataLocationCode**</span></span> | <span data-ttu-id="c708d-118">string</span><span class="sxs-lookup"><span data-stu-id="c708d-118">string</span></span>   | <span data-ttu-id="c708d-119">Der Code geografische Region, in dem diese Websitesammlung befindet.</span><span class="sxs-lookup"><span data-stu-id="c708d-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="c708d-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c708d-120">Read-only.</span></span>
| <span data-ttu-id="c708d-121">**root**</span><span class="sxs-lookup"><span data-stu-id="c708d-121">**root**</span></span>             | <span data-ttu-id="c708d-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="c708d-122">[root][]</span></span> | <span data-ttu-id="c708d-123">Falls vorhanden, gibt an, dass dies eine Stammwebsitesammlung in SharePoint ist.</span><span class="sxs-lookup"><span data-stu-id="c708d-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="c708d-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c708d-124">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
