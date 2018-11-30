---
title: website-Ressourcentyp
description: Stellt eine Website dar.
ms.openlocfilehash: fa117dc6279e90b49c3c54d0a0ac534e30e633af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063642"
---
# <a name="website-resource-type"></a><span data-ttu-id="88c31-103">website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88c31-103">website resource type</span></span>

> <span data-ttu-id="88c31-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="88c31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88c31-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88c31-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88c31-106">Stellt eine Website dar.</span><span class="sxs-lookup"><span data-stu-id="88c31-106">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="88c31-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88c31-107">Properties</span></span>
| <span data-ttu-id="88c31-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88c31-108">Property</span></span>     | <span data-ttu-id="88c31-109">Typ</span><span class="sxs-lookup"><span data-stu-id="88c31-109">Type</span></span>   |<span data-ttu-id="88c31-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88c31-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88c31-111">Typ</span><span class="sxs-lookup"><span data-stu-id="88c31-111">type</span></span>|<span data-ttu-id="88c31-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88c31-112">String</span></span>| <span data-ttu-id="88c31-113">Mögliche Werte: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="88c31-113">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="88c31-114">address</span><span class="sxs-lookup"><span data-stu-id="88c31-114">address</span></span>|<span data-ttu-id="88c31-115">string</span><span class="sxs-lookup"><span data-stu-id="88c31-115">string</span></span>|<span data-ttu-id="88c31-116">Die URL der Website.</span><span class="sxs-lookup"><span data-stu-id="88c31-116">The URL of the website.</span></span>|
|<span data-ttu-id="88c31-117">displayName</span><span class="sxs-lookup"><span data-stu-id="88c31-117">displayName</span></span>|<span data-ttu-id="88c31-118">string</span><span class="sxs-lookup"><span data-stu-id="88c31-118">string</span></span>|<span data-ttu-id="88c31-119">Der Anzeigename der Website.</span><span class="sxs-lookup"><span data-stu-id="88c31-119">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88c31-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88c31-120">JSON representation</span></span>

<span data-ttu-id="88c31-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88c31-121">Here is a JSON representation of the resource.</span></span>

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