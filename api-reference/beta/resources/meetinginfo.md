---
title: Ressourcentyp meetingInfo
description: Besprechungsinformationen, die zum Erstellen oder teilnehmen an einer Besprechung angegeben.
author: VinodRavichandran
ms.openlocfilehash: f8039f05a2f25e254f7aefd740055babc1598dc1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380310"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="94ec6-103">Ressourcentyp meetingInfo</span><span class="sxs-lookup"><span data-stu-id="94ec6-103">meetingInfo resource type</span></span>

> <span data-ttu-id="94ec6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94ec6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94ec6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94ec6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94ec6-106">Besprechungsinformationen, die zum Erstellen oder teilnehmen an einer Besprechung angegeben.</span><span class="sxs-lookup"><span data-stu-id="94ec6-106">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="94ec6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94ec6-107">Properties</span></span>

| <span data-ttu-id="94ec6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94ec6-108">Property</span></span>       | <span data-ttu-id="94ec6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="94ec6-109">Type</span></span>    | <span data-ttu-id="94ec6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94ec6-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94ec6-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="94ec6-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="94ec6-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="94ec6-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="94ec6-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94ec6-113">JSON representation</span></span>

<span data-ttu-id="94ec6-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94ec6-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
