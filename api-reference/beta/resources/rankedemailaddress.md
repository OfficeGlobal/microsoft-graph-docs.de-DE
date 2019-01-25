---
title: Ressourcentyp rankedEmailAddress
description: Stellt eine bewerteter e-Mail-Adresse dar.
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510008"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="429fb-103">Ressourcentyp rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="429fb-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="429fb-104">Stellt eine bewerteter e-Mail-Adresse dar.</span><span class="sxs-lookup"><span data-stu-id="429fb-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="429fb-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="429fb-105">Properties</span></span>
| <span data-ttu-id="429fb-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="429fb-106">Property</span></span>     | <span data-ttu-id="429fb-107">Typ</span><span class="sxs-lookup"><span data-stu-id="429fb-107">Type</span></span>   |<span data-ttu-id="429fb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="429fb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="429fb-109">address</span><span class="sxs-lookup"><span data-stu-id="429fb-109">address</span></span>|<span data-ttu-id="429fb-110">string</span><span class="sxs-lookup"><span data-stu-id="429fb-110">string</span></span>|<span data-ttu-id="429fb-111">Die E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="429fb-111">The email address.</span></span>|
|<span data-ttu-id="429fb-112">rank</span><span class="sxs-lookup"><span data-stu-id="429fb-112">rank</span></span>|<span data-ttu-id="429fb-113">double</span><span class="sxs-lookup"><span data-stu-id="429fb-113">double</span></span>|<span data-ttu-id="429fb-114">Die Rangfolge der e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="429fb-114">The rank of the email address.</span></span> <span data-ttu-id="429fb-115">Ein Rang wird als Sortierschlüssel, in Bezug auf die anderen zurückgegebenen Ergebnisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="429fb-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="429fb-116">Ein höherer Rangwert entspricht ein relevanter Ergebnis.</span><span class="sxs-lookup"><span data-stu-id="429fb-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="429fb-117">Relevanz ergibt sich für die Zusammenarbeit, Kommunikation und geschäftlichen Beziehung signalisiert.</span><span class="sxs-lookup"><span data-stu-id="429fb-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="429fb-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="429fb-118">JSON representation</span></span>

<span data-ttu-id="429fb-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="429fb-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rankedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
