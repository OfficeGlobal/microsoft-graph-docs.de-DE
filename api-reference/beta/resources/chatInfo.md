---
title: Ressourcentyp chatInfo
description: Informationen zu einer Nachricht in Microsoft-Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 840073d6882d6665be60e7386eaafe3168b70dbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940750"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="bd3c2-103">Ressourcentyp chatInfo</span><span class="sxs-lookup"><span data-stu-id="bd3c2-103">chatInfo resource type</span></span>

> <span data-ttu-id="bd3c2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd3c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd3c2-106">Informationen zu einer Nachricht in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="bd3c2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd3c2-107">Properties</span></span>

| <span data-ttu-id="bd3c2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd3c2-108">Property</span></span>            | <span data-ttu-id="bd3c2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bd3c2-109">Type</span></span>    | <span data-ttu-id="bd3c2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd3c2-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="bd3c2-111">messageId</span><span class="sxs-lookup"><span data-stu-id="bd3c2-111">messageId</span></span>           | <span data-ttu-id="bd3c2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd3c2-112">String</span></span>  | <span data-ttu-id="bd3c2-113">Der eindeutige Bezeichner für eine Nachricht in einem Microsoft-Teams Kanal.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="bd3c2-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="bd3c2-114">replyChainMessageId</span></span> | <span data-ttu-id="bd3c2-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd3c2-115">String</span></span>  | <span data-ttu-id="bd3c2-116">Die ID der Antwort-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="bd3c2-117">threadId</span><span class="sxs-lookup"><span data-stu-id="bd3c2-117">threadId</span></span>            | <span data-ttu-id="bd3c2-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd3c2-118">String</span></span>  | <span data-ttu-id="bd3c2-119">Der eindeutige Bezeichner für ein Thread im Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd3c2-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd3c2-120">JSON representation</span></span>

<span data-ttu-id="bd3c2-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd3c2-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
