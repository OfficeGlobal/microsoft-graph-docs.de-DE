---
title: Ressourcentyp chatInfo
description: Informationen zu einer Nachricht in Microsoft-Teams.
author: VinodRavichandran
ms.openlocfilehash: 45af1a7e178286c77ed4bf90528eb602fd48a6bb
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380415"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="a5537-103">Ressourcentyp chatInfo</span><span class="sxs-lookup"><span data-stu-id="a5537-103">chatInfo resource type</span></span>

> <span data-ttu-id="a5537-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a5537-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5537-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5537-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5537-106">Informationen zu einer Nachricht in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="a5537-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="a5537-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5537-107">Properties</span></span>

| <span data-ttu-id="a5537-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5537-108">Property</span></span>            | <span data-ttu-id="a5537-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a5537-109">Type</span></span>    | <span data-ttu-id="a5537-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5537-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="a5537-111">messageId</span><span class="sxs-lookup"><span data-stu-id="a5537-111">messageId</span></span>           | <span data-ttu-id="a5537-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5537-112">String</span></span>  | <span data-ttu-id="a5537-113">Der eindeutige Bezeichner für eine Nachricht in einem Microsoft-Teams Kanal.</span><span class="sxs-lookup"><span data-stu-id="a5537-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="a5537-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="a5537-114">replyChainMessageId</span></span> | <span data-ttu-id="a5537-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5537-115">String</span></span>  | <span data-ttu-id="a5537-116">Die ID der Antwort-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="a5537-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="a5537-117">threadId</span><span class="sxs-lookup"><span data-stu-id="a5537-117">threadId</span></span>            | <span data-ttu-id="a5537-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5537-118">String</span></span>  | <span data-ttu-id="a5537-119">Der eindeutige Bezeichner für ein Thread im Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="a5537-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5537-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5537-120">JSON representation</span></span>

<span data-ttu-id="a5537-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5537-121">The following is a JSON representation of the resource.</span></span>

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
