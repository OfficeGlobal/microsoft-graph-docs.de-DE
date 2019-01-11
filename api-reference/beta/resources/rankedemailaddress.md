---
title: Ressourcentyp rankedEmailAddress
description: Stellt eine bewerteter e-Mail-Adresse dar.
localization_priority: Normal
ms.openlocfilehash: bb3b906929bddcb52a57a478647000e7e16fa0be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818515"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="3a291-103">Ressourcentyp rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3a291-103">rankedEmailAddress resource type</span></span>

> <span data-ttu-id="3a291-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3a291-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a291-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a291-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a291-106">Stellt eine bewerteter e-Mail-Adresse dar.</span><span class="sxs-lookup"><span data-stu-id="3a291-106">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="3a291-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3a291-107">Properties</span></span>
| <span data-ttu-id="3a291-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a291-108">Property</span></span>     | <span data-ttu-id="3a291-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3a291-109">Type</span></span>   |<span data-ttu-id="3a291-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a291-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a291-111">address</span><span class="sxs-lookup"><span data-stu-id="3a291-111">address</span></span>|<span data-ttu-id="3a291-112">string</span><span class="sxs-lookup"><span data-stu-id="3a291-112">string</span></span>|<span data-ttu-id="3a291-113">Die E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="3a291-113">The email address.</span></span>|
|<span data-ttu-id="3a291-114">rank</span><span class="sxs-lookup"><span data-stu-id="3a291-114">rank</span></span>|<span data-ttu-id="3a291-115">double</span><span class="sxs-lookup"><span data-stu-id="3a291-115">double</span></span>|<span data-ttu-id="3a291-116">Die Rangfolge der e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="3a291-116">The rank of the email address.</span></span> <span data-ttu-id="3a291-117">Ein Rang wird als Sortierschlüssel, in Bezug auf die anderen zurückgegebenen Ergebnisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="3a291-117">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="3a291-118">Ein höherer Rangwert entspricht ein relevanter Ergebnis.</span><span class="sxs-lookup"><span data-stu-id="3a291-118">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="3a291-119">Relevanz ergibt sich für die Zusammenarbeit, Kommunikation und geschäftlichen Beziehung signalisiert.</span><span class="sxs-lookup"><span data-stu-id="3a291-119">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a291-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3a291-120">JSON representation</span></span>

<span data-ttu-id="3a291-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3a291-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
