---
title: scoredEmailAddress-Ressourcentyp
description: Gibt eine bewertete E-Mail-Adresse an.
localization_priority: Normal
ms.openlocfilehash: 740173e7d5f93dc875c08508bf73100727fdf415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819474"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="3bd45-103">scoredEmailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3bd45-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="3bd45-104">Gibt eine bewertete E-Mail-Adresse an.</span><span class="sxs-lookup"><span data-stu-id="3bd45-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="3bd45-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3bd45-105">Properties</span></span>
| <span data-ttu-id="3bd45-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3bd45-106">Property</span></span>     | <span data-ttu-id="3bd45-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3bd45-107">Type</span></span>   |<span data-ttu-id="3bd45-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bd45-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bd45-109">address</span><span class="sxs-lookup"><span data-stu-id="3bd45-109">address</span></span>|<span data-ttu-id="3bd45-110">string</span><span class="sxs-lookup"><span data-stu-id="3bd45-110">string</span></span>|<span data-ttu-id="3bd45-111">Die E-Mail-Adresse</span><span class="sxs-lookup"><span data-stu-id="3bd45-111">The email address.</span></span>|
|<span data-ttu-id="3bd45-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="3bd45-112">relevanceScore</span></span>|<span data-ttu-id="3bd45-113">double</span><span class="sxs-lookup"><span data-stu-id="3bd45-113">double</span></span>|<span data-ttu-id="3bd45-p101">Die Relevanzbewertung der E-Mail-Adresse. Eine Relevanzbewertung dient als Sortierschlüssel, in Bezug auf andere zurückgegebene Ergebnisse. Ein höherer Relevanzwert entspricht einem relevanteren Ergebnis. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt.</span><span class="sxs-lookup"><span data-stu-id="3bd45-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3bd45-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3bd45-118">JSON representation</span></span>

<span data-ttu-id="3bd45-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3bd45-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
