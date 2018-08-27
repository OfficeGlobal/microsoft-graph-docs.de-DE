---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 84de2a8aa6796051b3b11ebec0d0f8f5934ea1fc
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "19069343"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="87c21-102">SiteCollection-Ressource</span><span class="sxs-lookup"><span data-stu-id="87c21-102">SiteCollection resource</span></span>

<span data-ttu-id="87c21-103">Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.</span><span class="sxs-lookup"><span data-stu-id="87c21-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="87c21-104">Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="87c21-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87c21-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87c21-105">JSON representation</span></span>

<span data-ttu-id="87c21-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87c21-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="87c21-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87c21-107">Properties</span></span>

| <span data-ttu-id="87c21-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="87c21-108">Property name</span></span>        | <span data-ttu-id="87c21-109">Typ</span><span class="sxs-lookup"><span data-stu-id="87c21-109">Type</span></span>     | <span data-ttu-id="87c21-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87c21-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="87c21-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="87c21-111">**hostname**</span></span>         | <span data-ttu-id="87c21-112">string</span><span class="sxs-lookup"><span data-stu-id="87c21-112">string</span></span>   | <span data-ttu-id="87c21-p101">Der Hostname der Websitesammlung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87c21-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="87c21-115">**root**</span><span class="sxs-lookup"><span data-stu-id="87c21-115">**root**</span></span>             | <span data-ttu-id="87c21-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="87c21-116">[root][]</span></span> | <span data-ttu-id="87c21-117">Falls vorhanden gibt dies an, dass dies eine Stammwebsitesammlung in SharePoint ist.</span><span class="sxs-lookup"><span data-stu-id="87c21-117">If present, indicates that this is the root site in the site collection. Read-only.</span></span> <span data-ttu-id="87c21-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87c21-118">Read-only.</span></span>

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
