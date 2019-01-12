---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd003bde0eca5fd21cb12c23d5c83699a6b79c8e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916964"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="fa2f2-103">Ressourcentyp mediaStream</span><span class="sxs-lookup"><span data-stu-id="fa2f2-103">mediaStream resource type</span></span>

> <span data-ttu-id="fa2f2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa2f2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa2f2-106">Der Typ des MediaStream.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="fa2f2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa2f2-107">Properties</span></span>

| <span data-ttu-id="fa2f2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa2f2-108">Property</span></span>    | <span data-ttu-id="fa2f2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fa2f2-109">Type</span></span>    | <span data-ttu-id="fa2f2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa2f2-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="fa2f2-111">Richtung</span><span class="sxs-lookup"><span data-stu-id="fa2f2-111">direction</span></span>   | <span data-ttu-id="fa2f2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa2f2-112">String</span></span>  | <span data-ttu-id="fa2f2-113">Die Richtung.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-113">The direction.</span></span> <span data-ttu-id="fa2f2-114">Die möglichen Werte sind `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="fa2f2-115">label</span><span class="sxs-lookup"><span data-stu-id="fa2f2-115">label</span></span>       | <span data-ttu-id="fa2f2-116">String</span><span class="sxs-lookup"><span data-stu-id="fa2f2-116">String</span></span>  | <span data-ttu-id="fa2f2-117">Die Bezeichnung des Media-Stream.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="fa2f2-118">mediaType</span><span class="sxs-lookup"><span data-stu-id="fa2f2-118">mediaType</span></span>   | <span data-ttu-id="fa2f2-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa2f2-119">String</span></span>  | <span data-ttu-id="fa2f2-120">Geben Sie das Medium.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-120">The media type.</span></span> <span data-ttu-id="fa2f2-121">Die mögliche Werte sind `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="fa2f2-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="fa2f2-122">serverMuted</span></span> | <span data-ttu-id="fa2f2-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fa2f2-123">Boolean</span></span> | <span data-ttu-id="fa2f2-124">Wenn vom Server die Medien stummgeschaltet sind.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="fa2f2-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="fa2f2-125">sourceId</span></span>    | <span data-ttu-id="fa2f2-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa2f2-126">String</span></span>  | <span data-ttu-id="fa2f2-127">Die Quell-ID.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="fa2f2-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa2f2-128">JSON representation</span></span>

<span data-ttu-id="fa2f2-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa2f2-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="fa2f2-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa2f2-130">Example</span></span>

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
