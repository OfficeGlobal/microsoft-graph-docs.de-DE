---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
author: VinodRavichandran
ms.openlocfilehash: f870611700289f0254272b78e18e344d02dd123e
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380296"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="a9276-103">Ressourcentyp mediaStream</span><span class="sxs-lookup"><span data-stu-id="a9276-103">mediaStream resource type</span></span>

> <span data-ttu-id="a9276-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a9276-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9276-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9276-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9276-106">Der Typ des MediaStream.</span><span class="sxs-lookup"><span data-stu-id="a9276-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="a9276-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9276-107">Properties</span></span>

| <span data-ttu-id="a9276-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9276-108">Property</span></span>    | <span data-ttu-id="a9276-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a9276-109">Type</span></span>    | <span data-ttu-id="a9276-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9276-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a9276-111">Richtung</span><span class="sxs-lookup"><span data-stu-id="a9276-111">direction</span></span>   | <span data-ttu-id="a9276-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9276-112">String</span></span>  | <span data-ttu-id="a9276-113">Die Richtung.</span><span class="sxs-lookup"><span data-stu-id="a9276-113">The direction.</span></span> <span data-ttu-id="a9276-114">Die möglichen Werte sind `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="a9276-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="a9276-115">label</span><span class="sxs-lookup"><span data-stu-id="a9276-115">label</span></span>       | <span data-ttu-id="a9276-116">String</span><span class="sxs-lookup"><span data-stu-id="a9276-116">String</span></span>  | <span data-ttu-id="a9276-117">Die Bezeichnung des Media-Stream.</span><span class="sxs-lookup"><span data-stu-id="a9276-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="a9276-118">mediaType</span><span class="sxs-lookup"><span data-stu-id="a9276-118">mediaType</span></span>   | <span data-ttu-id="a9276-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9276-119">String</span></span>  | <span data-ttu-id="a9276-120">Geben Sie das Medium.</span><span class="sxs-lookup"><span data-stu-id="a9276-120">The media type.</span></span> <span data-ttu-id="a9276-121">Die mögliche Werte sind `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="a9276-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="a9276-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="a9276-122">serverMuted</span></span> | <span data-ttu-id="a9276-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a9276-123">Boolean</span></span> | <span data-ttu-id="a9276-124">Wenn vom Server die Medien stummgeschaltet sind.</span><span class="sxs-lookup"><span data-stu-id="a9276-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="a9276-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="a9276-125">sourceId</span></span>    | <span data-ttu-id="a9276-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9276-126">String</span></span>  | <span data-ttu-id="a9276-127">Die Quell-ID.</span><span class="sxs-lookup"><span data-stu-id="a9276-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="a9276-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9276-128">JSON representation</span></span>

<span data-ttu-id="a9276-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9276-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a><span data-ttu-id="a9276-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9276-130">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
