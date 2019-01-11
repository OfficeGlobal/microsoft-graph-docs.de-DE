---
title: Ressourcentyp toneInfo
description: Ein einzelnes DTMF-Ereignis.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b9be7e0e69be8d127df92f717ab462021f9684b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817108"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="e78ce-103">Ressourcentyp toneInfo</span><span class="sxs-lookup"><span data-stu-id="e78ce-103">toneInfo resource type</span></span>

> <span data-ttu-id="e78ce-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e78ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e78ce-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e78ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e78ce-106">Ein einzelnes DTMF-Ereignis.</span><span class="sxs-lookup"><span data-stu-id="e78ce-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="e78ce-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e78ce-107">Properties</span></span>

| <span data-ttu-id="e78ce-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e78ce-108">Property</span></span>       | <span data-ttu-id="e78ce-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e78ce-109">Type</span></span>    | <span data-ttu-id="e78ce-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e78ce-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e78ce-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="e78ce-111">sequenceId</span></span> | <span data-ttu-id="e78ce-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e78ce-112">Int64</span></span> | <span data-ttu-id="e78ce-113">Ein inkrementelle Bezeichner für eine Sortierung DTMF-Ereignisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="e78ce-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="e78ce-114">Tone</span><span class="sxs-lookup"><span data-stu-id="e78ce-114">tone</span></span> | <span data-ttu-id="e78ce-115">String</span><span class="sxs-lookup"><span data-stu-id="e78ce-115">String</span></span> | <span data-ttu-id="e78ce-116">Mögliche Werte sind: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="e78ce-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e78ce-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e78ce-117">JSON representation</span></span>

<span data-ttu-id="e78ce-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e78ce-118">The following is a JSON representation of the resource.</span></span>

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
