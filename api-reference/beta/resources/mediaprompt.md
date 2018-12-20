---
title: Ressourcentyp mediaPrompt
description: Der Typ des MediaPrompt.
author: VinodRavichandran
ms.openlocfilehash: 4782772f463a613a759ad3b2b25cb05e7e160555
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380289"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="1d6e1-103">Ressourcentyp mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="1d6e1-103">mediaPrompt resource type</span></span>

> <span data-ttu-id="1d6e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d6e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d6e1-106">Der Typ des MediaPrompt.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-106">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="1d6e1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d6e1-107">Properties</span></span>

| <span data-ttu-id="1d6e1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d6e1-108">Property</span></span>    | <span data-ttu-id="1d6e1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1d6e1-109">Type</span></span>                      | <span data-ttu-id="1d6e1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d6e1-110">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="1d6e1-111">Schleife</span><span class="sxs-lookup"><span data-stu-id="1d6e1-111">loop</span></span>        | <span data-ttu-id="1d6e1-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1d6e1-112">Int32</span></span>                     | <span data-ttu-id="1d6e1-113">Die Anzahl der Schleifen.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-113">The loop count.</span></span> <span data-ttu-id="1d6e1-114">Wert 0 gibt an, dass Endlosschleife ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-114">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="1d6e1-115">Der Standardwert lautet `1`.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-115">The default value is `1`.</span></span> |
| <span data-ttu-id="1d6e1-116">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="1d6e1-116">mediaInfo</span></span>   | [<span data-ttu-id="1d6e1-117">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="1d6e1-117">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="1d6e1-118">Die Medieninformationen</span><span class="sxs-lookup"><span data-stu-id="1d6e1-118">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="1d6e1-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d6e1-119">JSON representation</span></span>

<span data-ttu-id="1d6e1-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d6e1-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="1d6e1-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d6e1-121">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
