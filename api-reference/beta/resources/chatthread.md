---
title: chatThread-Ressourcentyp
description: Ein chatThread ist eine Sammlung von chatMessages in Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399605"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="d18f8-103">chatThread-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d18f8-103">chatThread resource type</span></span>

> <span data-ttu-id="d18f8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d18f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d18f8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d18f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d18f8-106">Ein chatThread ist eine Sammlung von [chatMessages](chatmessage.md) in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d18f8-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="d18f8-107">Derzeit können chatThreads [in Kanälen erstellt werden](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="d18f8-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="d18f8-108">In künftigen API-Versionen wird das Lesen von vorhandenen chatThreads sowie das Lesen/Schreiben von direkten Chats zwischen Benutzern, die sich außerhalb des Bereichs eines Teams oder Kanals befinden, unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d18f8-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="d18f8-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="d18f8-109">Methods</span></span>

| <span data-ttu-id="d18f8-110">Methode</span><span class="sxs-lookup"><span data-stu-id="d18f8-110">Method</span></span>       | <span data-ttu-id="d18f8-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d18f8-111">Return Type</span></span>  |<span data-ttu-id="d18f8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d18f8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d18f8-113">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="d18f8-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="d18f8-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="d18f8-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="d18f8-115">Starten Sie einen neuen Thread in dem angegebenen Kanal, wodurch Sie die erste Nachricht bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="d18f8-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="d18f8-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d18f8-116">Properties</span></span>
| <span data-ttu-id="d18f8-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d18f8-117">Property</span></span>     | <span data-ttu-id="d18f8-118">Typ</span><span class="sxs-lookup"><span data-stu-id="d18f8-118">Type</span></span>   |<span data-ttu-id="d18f8-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d18f8-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d18f8-120">id</span><span class="sxs-lookup"><span data-stu-id="d18f8-120">id</span></span>|<span data-ttu-id="d18f8-121">String</span><span class="sxs-lookup"><span data-stu-id="d18f8-121">String</span></span>| <span data-ttu-id="d18f8-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d18f8-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d18f8-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d18f8-123">Relationships</span></span>
| <span data-ttu-id="d18f8-124">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d18f8-124">Relationship</span></span> | <span data-ttu-id="d18f8-125">Typ</span><span class="sxs-lookup"><span data-stu-id="d18f8-125">Type</span></span>   |<span data-ttu-id="d18f8-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d18f8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d18f8-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="d18f8-127">rootMessage</span></span>|[<span data-ttu-id="d18f8-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d18f8-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="d18f8-129">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="d18f8-129">Nullable.</span></span>|
|<span data-ttu-id="d18f8-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="d18f8-130">chatMessages</span></span>|<span data-ttu-id="d18f8-131">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d18f8-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="d18f8-132">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="d18f8-132">Nullable.</span></span>|

> <span data-ttu-id="d18f8-133">Diese Beziehungen sind derzeit implizit vorhanden, können aber nicht gelesen oder geschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="d18f8-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="d18f8-134">In zukünftigen API-Betaversionen wird dies unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d18f8-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d18f8-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d18f8-135">JSON representation</span></span>

<span data-ttu-id="d18f8-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d18f8-136">Here is a JSON representation of the resource</span></span>

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
  "id": "string (identifier)"
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
