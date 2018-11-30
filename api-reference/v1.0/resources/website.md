---
title: website-Ressourcentyp
description: Stellt eine Website dar.
ms.openlocfilehash: 14934aae418581f4c75c880be67bf51fd0bc293c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016550"
---
# <a name="website-resource-type"></a><span data-ttu-id="ace89-103">website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ace89-103">website resource type</span></span>

<span data-ttu-id="ace89-104">Stellt eine Website dar.</span><span class="sxs-lookup"><span data-stu-id="ace89-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="ace89-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ace89-105">Properties</span></span>
| <span data-ttu-id="ace89-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ace89-106">Property</span></span>     | <span data-ttu-id="ace89-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ace89-107">Type</span></span>   |<span data-ttu-id="ace89-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ace89-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ace89-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ace89-109">type</span></span>|<span data-ttu-id="ace89-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="ace89-110">websiteType</span></span>| <span data-ttu-id="ace89-111">Die möglichen Werte sind: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="ace89-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="ace89-112">address</span><span class="sxs-lookup"><span data-stu-id="ace89-112">address</span></span>|<span data-ttu-id="ace89-113">string</span><span class="sxs-lookup"><span data-stu-id="ace89-113">string</span></span>|<span data-ttu-id="ace89-114">Die URL der Website.</span><span class="sxs-lookup"><span data-stu-id="ace89-114">The URL of the website.</span></span>|
|<span data-ttu-id="ace89-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ace89-115">displayName</span></span>|<span data-ttu-id="ace89-116">string</span><span class="sxs-lookup"><span data-stu-id="ace89-116">string</span></span>|<span data-ttu-id="ace89-117">Der Anzeigename der Website.</span><span class="sxs-lookup"><span data-stu-id="ace89-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ace89-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ace89-118">JSON representation</span></span>

<span data-ttu-id="ace89-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ace89-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
