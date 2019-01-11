---
title: Ressourcentyp audioDuckingConfiguration
description: Parameter für Vermeiden von anderen Quellen (können in und aus anderen Quellen).
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 713e7012381bf6b727321494f81e75c88c66ebe6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891560"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="ba08f-103">Ressourcentyp audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba08f-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="ba08f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ba08f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba08f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba08f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba08f-106">Parameter für Vermeiden von anderen Quellen (können in und aus anderen Quellen).</span><span class="sxs-lookup"><span data-stu-id="ba08f-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="ba08f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba08f-107">Properties</span></span>

| <span data-ttu-id="ba08f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba08f-108">Property</span></span>      | <span data-ttu-id="ba08f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ba08f-109">Type</span></span>     | <span data-ttu-id="ba08f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba08f-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="ba08f-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="ba08f-111">lowerLevel</span></span>    | <span data-ttu-id="ba08f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ba08f-112">Int64</span></span>    | <span data-ttu-id="ba08f-113">Das Volumen der Quellen in Prozent, wenn Sie die Quellen sind ducked wird.</span><span class="sxs-lookup"><span data-stu-id="ba08f-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="ba08f-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="ba08f-114">rampActive</span></span>    | <span data-ttu-id="ba08f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ba08f-115">Int64</span></span>    | <span data-ttu-id="ba08f-116">Die Zeitdauer (in Millisekunden) für ducked Datenquellen "Verblassen" dauert.</span><span class="sxs-lookup"><span data-stu-id="ba08f-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="ba08f-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="ba08f-117">rampInactive</span></span>  | <span data-ttu-id="ba08f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ba08f-118">Int64</span></span>    | <span data-ttu-id="ba08f-119">Die Zeitdauer (in Millisekunden) für ducked Datenquellen für eine "einblenden" dauert.</span><span class="sxs-lookup"><span data-stu-id="ba08f-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="ba08f-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="ba08f-120">upperLevel</span></span>    | <span data-ttu-id="ba08f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ba08f-121">Int64</span></span>    | <span data-ttu-id="ba08f-122">Das Volumen der Quellen in Prozent, wenn Sie die Quellen sind nicht ducked wird.</span><span class="sxs-lookup"><span data-stu-id="ba08f-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="ba08f-123">**Hinweis:** Lernen Dauer kann nicht mehr als 5000 Millisekunden sein.</span><span class="sxs-lookup"><span data-stu-id="ba08f-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba08f-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba08f-124">JSON representation</span></span>

<span data-ttu-id="ba08f-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba08f-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
