---
title: Ressourcentyp mediaConfig
description: Die Medienkonfiguration für die Verbindung zu einem Anruf verwendet.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ec76adf2d3a508ebe2518ed0010a1c653daca546
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867348"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="04b49-103">Ressourcentyp mediaConfig</span><span class="sxs-lookup"><span data-stu-id="04b49-103">mediaConfig resource type</span></span>

> <span data-ttu-id="04b49-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04b49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04b49-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04b49-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04b49-106">Die Medienkonfiguration für die Verbindung zu einem Anruf verwendet.</span><span class="sxs-lookup"><span data-stu-id="04b49-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="04b49-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04b49-107">Properties</span></span>

| <span data-ttu-id="04b49-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04b49-108">Property</span></span>       | <span data-ttu-id="04b49-109">Typ</span><span class="sxs-lookup"><span data-stu-id="04b49-109">Type</span></span>    | <span data-ttu-id="04b49-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04b49-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04b49-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="04b49-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="04b49-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="04b49-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="04b49-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04b49-113">JSON representation</span></span>

<span data-ttu-id="04b49-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="04b49-114">The following is a JSON representation of the resource.</span></span>

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
