---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 6b36f3a0c2d958081f1b5663231a541f2e8a000f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="sitecollection-resource"></a><span data-ttu-id="d94b9-102">SiteCollection-Ressource</span><span class="sxs-lookup"><span data-stu-id="d94b9-102">SiteCollection resource</span></span>

<span data-ttu-id="d94b9-103">Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.</span><span class="sxs-lookup"><span data-stu-id="d94b9-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="d94b9-104">Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="d94b9-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d94b9-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d94b9-105">JSON representation</span></span>

<span data-ttu-id="d94b9-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d94b9-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com"
}
```

## <a name="properties"></a><span data-ttu-id="d94b9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d94b9-107">Properties</span></span>

| <span data-ttu-id="d94b9-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d94b9-108">Property name</span></span> | <span data-ttu-id="d94b9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d94b9-109">Type</span></span>    | <span data-ttu-id="d94b9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d94b9-110">Description</span></span>                                                                                                                  |
|:--------------|:--------|:---------------------------------------------------
| <span data-ttu-id="d94b9-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="d94b9-111">**hostname**</span></span>  | <span data-ttu-id="d94b9-112">string</span><span class="sxs-lookup"><span data-stu-id="d94b9-112">string</span></span>  | <span data-ttu-id="d94b9-p101">Der Hostname der Websitesammlung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d94b9-p101">The hostname for the site collection. Read-only.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
