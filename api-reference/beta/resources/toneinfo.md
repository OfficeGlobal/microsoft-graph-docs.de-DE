---
title: Ressourcentyp toneInfo
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: b4ed9667c2e2156f52703c6fa15f4937ead5cef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065439"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="f7cb0-103">Ressourcentyp toneInfo</span><span class="sxs-lookup"><span data-stu-id="f7cb0-103">toneInfo resource type</span></span>

> <span data-ttu-id="f7cb0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7cb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7cb0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7cb0-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="f7cb0-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7cb0-106">Properties</span></span>

| <span data-ttu-id="f7cb0-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7cb0-107">Property</span></span>       | <span data-ttu-id="f7cb0-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f7cb0-108">Type</span></span>    | <span data-ttu-id="f7cb0-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7cb0-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7cb0-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="f7cb0-110">sequenceId</span></span> | <span data-ttu-id="f7cb0-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f7cb0-111">Int64</span></span> | <span data-ttu-id="f7cb0-112">Ein inkrementelle Bezeichner für eine Sortierung DTMF-Ereignisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="f7cb0-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="f7cb0-113">Tone</span><span class="sxs-lookup"><span data-stu-id="f7cb0-113">tone</span></span> | <span data-ttu-id="f7cb0-114">String</span><span class="sxs-lookup"><span data-stu-id="f7cb0-114">String</span></span> | <span data-ttu-id="f7cb0-115">Mögliche Werte sind: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="f7cb0-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7cb0-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7cb0-116">JSON representation</span></span>

<span data-ttu-id="f7cb0-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7cb0-117">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->