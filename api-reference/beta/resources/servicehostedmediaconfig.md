---
title: Ressourcentyp serviceHostedMediaConfig
description: Der Typ des ServiceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ec2ff24ef0bb45a9b49ecf2d0dc5e7419318b5af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828700"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="3d9b3-103">Ressourcentyp serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="3d9b3-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="3d9b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3d9b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d9b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d9b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d9b3-106">Der Typ des ServiceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="3d9b3-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="3d9b3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d9b3-107">Properties</span></span>

| <span data-ttu-id="3d9b3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d9b3-108">Property</span></span>                    | <span data-ttu-id="3d9b3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3d9b3-109">Type</span></span>                                                        | <span data-ttu-id="3d9b3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d9b3-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="3d9b3-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="3d9b3-111">preFetchMedia</span></span>               | <span data-ttu-id="3d9b3-112">[MediaInfo](mediainfo.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3d9b3-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="3d9b3-113">Die Liste der Media vorab abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3d9b3-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="3d9b3-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="3d9b3-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="3d9b3-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3d9b3-115">Boolean</span></span>                                                     | <span data-ttu-id="3d9b3-116">Audio Standardgruppe Self Teilnehmer aufheben.</span><span class="sxs-lookup"><span data-stu-id="3d9b3-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d9b3-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d9b3-117">JSON representation</span></span>

<span data-ttu-id="3d9b3-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d9b3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "#microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="3d9b3-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d9b3-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
