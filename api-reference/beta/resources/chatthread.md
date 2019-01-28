---
title: chatThread-Ressourcentyp
description: Ein chatThread ist eine Sammlung von chatMessages in Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521341"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="0d79c-103">chatThread-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d79c-103">chatThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d79c-104">Ein chatThread ist eine Sammlung von [chatMessages](chatmessage.md) in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0d79c-104">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="0d79c-105">Derzeit können chatThreads [in Kanälen erstellt werden](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="0d79c-105">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="0d79c-106">In künftigen API-Versionen wird das Lesen von vorhandenen chatThreads sowie das Lesen/Schreiben von direkten Chats zwischen Benutzern, die sich außerhalb des Bereichs eines Teams oder Kanals befinden, unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d79c-106">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="0d79c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="0d79c-107">Methods</span></span>

| <span data-ttu-id="0d79c-108">Methode</span><span class="sxs-lookup"><span data-stu-id="0d79c-108">Method</span></span>       | <span data-ttu-id="0d79c-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0d79c-109">Return Type</span></span>  |<span data-ttu-id="0d79c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d79c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d79c-111">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="0d79c-111">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="0d79c-112">chatThread</span><span class="sxs-lookup"><span data-stu-id="0d79c-112">chatThread</span></span>](chatthread.md) |<span data-ttu-id="0d79c-113">Starten Sie einen neuen Thread in dem angegebenen Kanal, wodurch Sie die erste Nachricht bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="0d79c-113">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d79c-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d79c-114">Properties</span></span>
| <span data-ttu-id="0d79c-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d79c-115">Property</span></span>     | <span data-ttu-id="0d79c-116">Typ</span><span class="sxs-lookup"><span data-stu-id="0d79c-116">Type</span></span>   |<span data-ttu-id="0d79c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d79c-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d79c-118">id</span><span class="sxs-lookup"><span data-stu-id="0d79c-118">id</span></span>|<span data-ttu-id="0d79c-119">String</span><span class="sxs-lookup"><span data-stu-id="0d79c-119">String</span></span>| <span data-ttu-id="0d79c-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0d79c-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d79c-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d79c-121">Relationships</span></span>
| <span data-ttu-id="0d79c-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0d79c-122">Relationship</span></span> | <span data-ttu-id="0d79c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0d79c-123">Type</span></span>   |<span data-ttu-id="0d79c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d79c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d79c-125">rootMessage</span><span class="sxs-lookup"><span data-stu-id="0d79c-125">rootMessage</span></span>|[<span data-ttu-id="0d79c-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0d79c-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="0d79c-127">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="0d79c-127">Nullable.</span></span>|
|<span data-ttu-id="0d79c-128">chatMessages</span><span class="sxs-lookup"><span data-stu-id="0d79c-128">chatMessages</span></span>|<span data-ttu-id="0d79c-129">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0d79c-129">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="0d79c-130">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="0d79c-130">Nullable.</span></span>|

> <span data-ttu-id="0d79c-131">Diese Beziehungen sind derzeit implizit vorhanden, können aber nicht gelesen oder geschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="0d79c-131">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="0d79c-132">In zukünftigen API-Betaversionen wird dies unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d79c-132">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d79c-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d79c-133">JSON representation</span></span>

<span data-ttu-id="0d79c-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d79c-134">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
