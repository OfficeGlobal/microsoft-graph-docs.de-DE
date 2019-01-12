---
title: Ressourcentyp mediaConfig
description: Die Medienkonfiguration für die Verbindung zu einem Anruf verwendet.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 74b3b5dc4c71db80e94216756a3513a03011572a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948919"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="96b03-103">Ressourcentyp mediaConfig</span><span class="sxs-lookup"><span data-stu-id="96b03-103">mediaConfig resource type</span></span>

> <span data-ttu-id="96b03-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96b03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96b03-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96b03-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96b03-106">Die Medienkonfiguration für die Verbindung zu einem Anruf verwendet.</span><span class="sxs-lookup"><span data-stu-id="96b03-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="96b03-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96b03-107">Properties</span></span>

| <span data-ttu-id="96b03-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96b03-108">Property</span></span>       | <span data-ttu-id="96b03-109">Typ</span><span class="sxs-lookup"><span data-stu-id="96b03-109">Type</span></span>    | <span data-ttu-id="96b03-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96b03-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96b03-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="96b03-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="96b03-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="96b03-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="96b03-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96b03-113">JSON representation</span></span>

<span data-ttu-id="96b03-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96b03-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
