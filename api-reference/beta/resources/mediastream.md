---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519962"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="f864b-103">Ressourcentyp mediaStream</span><span class="sxs-lookup"><span data-stu-id="f864b-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f864b-104">Der Typ des MediaStream.</span><span class="sxs-lookup"><span data-stu-id="f864b-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="f864b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f864b-105">Properties</span></span>

| <span data-ttu-id="f864b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f864b-106">Property</span></span>    | <span data-ttu-id="f864b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f864b-107">Type</span></span>    | <span data-ttu-id="f864b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f864b-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f864b-109">Richtung</span><span class="sxs-lookup"><span data-stu-id="f864b-109">direction</span></span>   | <span data-ttu-id="f864b-110">String</span><span class="sxs-lookup"><span data-stu-id="f864b-110">String</span></span>  | <span data-ttu-id="f864b-111">Die Richtung.</span><span class="sxs-lookup"><span data-stu-id="f864b-111">The direction.</span></span> <span data-ttu-id="f864b-112">Die möglichen Werte sind `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="f864b-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="f864b-113">label</span><span class="sxs-lookup"><span data-stu-id="f864b-113">label</span></span>       | <span data-ttu-id="f864b-114">String</span><span class="sxs-lookup"><span data-stu-id="f864b-114">String</span></span>  | <span data-ttu-id="f864b-115">Die Bezeichnung des Media-Stream.</span><span class="sxs-lookup"><span data-stu-id="f864b-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="f864b-116">MediaType</span><span class="sxs-lookup"><span data-stu-id="f864b-116">mediaType</span></span>   | <span data-ttu-id="f864b-117">String</span><span class="sxs-lookup"><span data-stu-id="f864b-117">String</span></span>  | <span data-ttu-id="f864b-118">Geben Sie das Medium.</span><span class="sxs-lookup"><span data-stu-id="f864b-118">The media type.</span></span> <span data-ttu-id="f864b-119">Die mögliche Werte sind `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="f864b-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="f864b-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="f864b-120">serverMuted</span></span> | <span data-ttu-id="f864b-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f864b-121">Boolean</span></span> | <span data-ttu-id="f864b-122">Wenn vom Server die Medien stummgeschaltet sind.</span><span class="sxs-lookup"><span data-stu-id="f864b-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="f864b-123">SourceId</span><span class="sxs-lookup"><span data-stu-id="f864b-123">sourceId</span></span>    | <span data-ttu-id="f864b-124">String</span><span class="sxs-lookup"><span data-stu-id="f864b-124">String</span></span>  | <span data-ttu-id="f864b-125">Die Quell-ID.</span><span class="sxs-lookup"><span data-stu-id="f864b-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="f864b-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f864b-126">JSON representation</span></span>

<span data-ttu-id="f864b-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f864b-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="f864b-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f864b-128">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediastream.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
