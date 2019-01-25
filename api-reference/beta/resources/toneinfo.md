---
title: Ressourcentyp toneInfo
description: Ein einzelnes DTMF-Ereignis.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f58548f8f075494c6601db2962d88fb6cabb59ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526011"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="50c85-103">Ressourcentyp toneInfo</span><span class="sxs-lookup"><span data-stu-id="50c85-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50c85-104">Ein einzelnes DTMF-Ereignis.</span><span class="sxs-lookup"><span data-stu-id="50c85-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="50c85-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50c85-105">Properties</span></span>

| <span data-ttu-id="50c85-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50c85-106">Property</span></span>       | <span data-ttu-id="50c85-107">Typ</span><span class="sxs-lookup"><span data-stu-id="50c85-107">Type</span></span>    | <span data-ttu-id="50c85-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50c85-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50c85-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="50c85-109">sequenceId</span></span> | <span data-ttu-id="50c85-110">Int64</span><span class="sxs-lookup"><span data-stu-id="50c85-110">Int64</span></span> | <span data-ttu-id="50c85-111">Ein inkrementelle Bezeichner für eine Sortierung DTMF-Ereignisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="50c85-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="50c85-112">Tone</span><span class="sxs-lookup"><span data-stu-id="50c85-112">tone</span></span> | <span data-ttu-id="50c85-113">String</span><span class="sxs-lookup"><span data-stu-id="50c85-113">String</span></span> | <span data-ttu-id="50c85-114">Mögliche Werte sind: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="50c85-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50c85-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50c85-115">JSON representation</span></span>

<span data-ttu-id="50c85-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50c85-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/toneinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
