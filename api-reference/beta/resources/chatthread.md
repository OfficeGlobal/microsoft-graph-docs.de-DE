---
title: Ressourcentyp chatThread
description: Eine ChatThread ist eine Auflistung von ChatMessages in Microsoft-Teams.
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064966"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="c5d08-103">Ressourcentyp chatThread</span><span class="sxs-lookup"><span data-stu-id="c5d08-103">chatThread resource type</span></span>

> <span data-ttu-id="c5d08-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c5d08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5d08-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5d08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5d08-106">Eine ChatThread ist eine Auflistung von [ChatMessages](chatmessage.md) in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="c5d08-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="c5d08-107">Derzeit können ChatThreads [in Kanäle erstellt](../api/channel-post-chatthreads.md)werden.</span><span class="sxs-lookup"><span data-stu-id="c5d08-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="c5d08-108">Die Zukunft API Versionen wird beim Lesen der vorhandenen ChatThreads als auch Lesen/Schreiben von direkten Chats zwischen Benutzern, die sich des Bereichs einer Teamwebsite oder einer DDE-Kanal außerhalb unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5d08-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="c5d08-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="c5d08-109">Methods</span></span>

| <span data-ttu-id="c5d08-110">Methode</span><span class="sxs-lookup"><span data-stu-id="c5d08-110">Method</span></span>       | <span data-ttu-id="c5d08-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c5d08-111">Return Type</span></span>  |<span data-ttu-id="c5d08-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5d08-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5d08-113">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="c5d08-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="c5d08-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="c5d08-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="c5d08-115">Starten Sie einen neuen Thread in der angegebenen DDE-Kanal, die erste Nachricht bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="c5d08-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5d08-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c5d08-116">Properties</span></span>
| <span data-ttu-id="c5d08-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5d08-117">Property</span></span>     | <span data-ttu-id="c5d08-118">Typ</span><span class="sxs-lookup"><span data-stu-id="c5d08-118">Type</span></span>   |<span data-ttu-id="c5d08-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5d08-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5d08-120">id</span><span class="sxs-lookup"><span data-stu-id="c5d08-120">id</span></span>|<span data-ttu-id="c5d08-121">String</span><span class="sxs-lookup"><span data-stu-id="c5d08-121">String</span></span>| <span data-ttu-id="c5d08-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5d08-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5d08-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c5d08-123">Relationships</span></span>
| <span data-ttu-id="c5d08-124">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c5d08-124">Relationship</span></span> | <span data-ttu-id="c5d08-125">Typ</span><span class="sxs-lookup"><span data-stu-id="c5d08-125">Type</span></span>   |<span data-ttu-id="c5d08-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5d08-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5d08-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="c5d08-127">rootMessage</span></span>|[<span data-ttu-id="c5d08-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c5d08-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c5d08-129">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="c5d08-129">Nullable.</span></span>|
|<span data-ttu-id="c5d08-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="c5d08-130">chatMessages</span></span>|<span data-ttu-id="c5d08-131">[ChatMessage](chatmessage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c5d08-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c5d08-132">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="c5d08-132">Nullable.</span></span>|

> <span data-ttu-id="c5d08-133">Auf diese Beziehungen vorhanden sind implizit, kann nicht aber gelesen oder geschrieben.</span><span class="sxs-lookup"><span data-stu-id="c5d08-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="c5d08-134">Zukünftige Betaversionen API unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5d08-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5d08-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c5d08-135">JSON representation</span></span>

<span data-ttu-id="c5d08-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c5d08-136">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
