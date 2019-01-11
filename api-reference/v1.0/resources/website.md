---
title: website-Ressourcentyp
description: Stellt eine Website dar.
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851366"
---
# <a name="website-resource-type"></a><span data-ttu-id="df648-103">website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df648-103">website resource type</span></span>

<span data-ttu-id="df648-104">Stellt eine Website dar.</span><span class="sxs-lookup"><span data-stu-id="df648-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="df648-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df648-105">Properties</span></span>
| <span data-ttu-id="df648-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df648-106">Property</span></span>     | <span data-ttu-id="df648-107">Typ</span><span class="sxs-lookup"><span data-stu-id="df648-107">Type</span></span>   |<span data-ttu-id="df648-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df648-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df648-109">type</span><span class="sxs-lookup"><span data-stu-id="df648-109">type</span></span>|<span data-ttu-id="df648-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="df648-110">websiteType</span></span>| <span data-ttu-id="df648-111">Die möglichen Werte sind: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="df648-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="df648-112">address</span><span class="sxs-lookup"><span data-stu-id="df648-112">address</span></span>|<span data-ttu-id="df648-113">string</span><span class="sxs-lookup"><span data-stu-id="df648-113">string</span></span>|<span data-ttu-id="df648-114">Die URL der Website.</span><span class="sxs-lookup"><span data-stu-id="df648-114">The URL of the website.</span></span>|
|<span data-ttu-id="df648-115">displayName</span><span class="sxs-lookup"><span data-stu-id="df648-115">displayName</span></span>|<span data-ttu-id="df648-116">string</span><span class="sxs-lookup"><span data-stu-id="df648-116">string</span></span>|<span data-ttu-id="df648-117">Der Anzeigename der Website.</span><span class="sxs-lookup"><span data-stu-id="df648-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df648-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df648-118">JSON representation</span></span>

<span data-ttu-id="df648-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df648-119">The following is a JSON representation of the resource.</span></span>

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
