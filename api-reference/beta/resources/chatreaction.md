---
title: Ressourcentyp chatMessageReaction
description: 'Stellt eine Reaktion auf eine Entität ChatMessage dar. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810066"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="248e1-103">Ressourcentyp chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="248e1-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="248e1-104">Stellt eine Reaktion auf eine Entität [ChatMessage](chatmessage.md) dar.</span><span class="sxs-lookup"><span data-stu-id="248e1-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="248e1-105">Eine Entität vom Typ `chatMessageReaction` wird als Teil des [ChatMessage](chatmessage.md) -Entität als Teil des [Kanalnachrichten abrufen](../api/channel-get-message.md) -API zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="248e1-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="248e1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="248e1-106">Properties</span></span>
| <span data-ttu-id="248e1-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="248e1-107">Property</span></span>     | <span data-ttu-id="248e1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="248e1-108">Type</span></span>   |<span data-ttu-id="248e1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="248e1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="248e1-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="248e1-110">reactionType</span></span>|<span data-ttu-id="248e1-111">string</span><span class="sxs-lookup"><span data-stu-id="248e1-111">string</span></span>| <span data-ttu-id="248e1-112">Der Typ der Reaktion.</span><span class="sxs-lookup"><span data-stu-id="248e1-112">The type of reaction.</span></span> <span data-ttu-id="248e1-113">Geplante Werte:</span><span class="sxs-lookup"><span data-stu-id="248e1-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="248e1-114">Wie - wie eine Nachricht Inhalte leer in diesem Fall ist.</span><span class="sxs-lookup"><span data-stu-id="248e1-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="248e1-115">Emoji - Emoji Reaktion.</span><span class="sxs-lookup"><span data-stu-id="248e1-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="248e1-116">Inhalt wird auf Unicodewert, der die Emoji festgelegt.</span><span class="sxs-lookup"><span data-stu-id="248e1-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="248e1-117">Label - wird Inhalt auf die Zeichenfolge die Bezeichnung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="248e1-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="248e1-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="248e1-118">createdDateTime</span></span>|<span data-ttu-id="248e1-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="248e1-119">dateTimeOffset</span></span>|<span data-ttu-id="248e1-120">UTC-Zeitstempel der Stamm Nachricht im ISO 8601-Format.</span><span class="sxs-lookup"><span data-stu-id="248e1-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="248e1-121">user</span><span class="sxs-lookup"><span data-stu-id="248e1-121">user</span></span>|<span data-ttu-id="248e1-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="248e1-122">identitySet</span></span>|<span data-ttu-id="248e1-123">Der Benutzer, die an die Nachricht reagiert.</span><span class="sxs-lookup"><span data-stu-id="248e1-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="248e1-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="248e1-124">JSON representation</span></span>

<span data-ttu-id="248e1-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="248e1-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
