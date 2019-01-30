---
title: website-Ressourcentyp
description: Stellt eine Website dar.
localization_priority: Normal
ms.openlocfilehash: 3f8aadaf0a6b6beb2394664f04195267062dc9ae
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641246"
---
# <a name="website-resource-type"></a><span data-ttu-id="fef11-103">website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fef11-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fef11-104">Stellt eine Website dar.</span><span class="sxs-lookup"><span data-stu-id="fef11-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="fef11-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fef11-105">Properties</span></span>
| <span data-ttu-id="fef11-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fef11-106">Property</span></span>     | <span data-ttu-id="fef11-107">Typ</span><span class="sxs-lookup"><span data-stu-id="fef11-107">Type</span></span>   |<span data-ttu-id="fef11-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fef11-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fef11-109">type</span><span class="sxs-lookup"><span data-stu-id="fef11-109">type</span></span>|<span data-ttu-id="fef11-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fef11-110">String</span></span>| <span data-ttu-id="fef11-111">Mögliche Werte: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="fef11-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="fef11-112">address</span><span class="sxs-lookup"><span data-stu-id="fef11-112">address</span></span>|<span data-ttu-id="fef11-113">string</span><span class="sxs-lookup"><span data-stu-id="fef11-113">string</span></span>|<span data-ttu-id="fef11-114">Die URL der Website.</span><span class="sxs-lookup"><span data-stu-id="fef11-114">The URL of the website.</span></span>|
|<span data-ttu-id="fef11-115">displayName</span><span class="sxs-lookup"><span data-stu-id="fef11-115">displayName</span></span>|<span data-ttu-id="fef11-116">string</span><span class="sxs-lookup"><span data-stu-id="fef11-116">string</span></span>|<span data-ttu-id="fef11-117">Der Anzeigename der Website.</span><span class="sxs-lookup"><span data-stu-id="fef11-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fef11-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fef11-118">JSON representation</span></span>

<span data-ttu-id="fef11-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fef11-119">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/website.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
