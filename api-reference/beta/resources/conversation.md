---
title: Ressourcentyp conversation
description: Eine Unterhaltung ist eine Sammlung von Threads, und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5cacad2b9539c398251ffd07899df7beb3c2f378
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991440"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="22ec5-104">Ressourcentyp conversation</span><span class="sxs-lookup"><span data-stu-id="22ec5-104">conversation resource type</span></span>

> <span data-ttu-id="22ec5-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="22ec5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22ec5-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22ec5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22ec5-p103">Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.</span><span class="sxs-lookup"><span data-stu-id="22ec5-p103">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="22ec5-109">Diese Ressource unterstützt Abonnieren von [Benachrichtigungen ändern](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="22ec5-109">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="22ec5-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="22ec5-110">Methods</span></span>

| <span data-ttu-id="22ec5-111">Methode</span><span class="sxs-lookup"><span data-stu-id="22ec5-111">Method</span></span>       | <span data-ttu-id="22ec5-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="22ec5-112">Return Type</span></span>  |<span data-ttu-id="22ec5-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22ec5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22ec5-114">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="22ec5-114">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="22ec5-115">[conversation](conversation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="22ec5-115">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="22ec5-116">Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="22ec5-116">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="22ec5-117">Erstellen</span><span class="sxs-lookup"><span data-stu-id="22ec5-117">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="22ec5-118">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="22ec5-118">conversation</span></span>](conversation.md)| <span data-ttu-id="22ec5-119">Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="22ec5-119">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="22ec5-120">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="22ec5-120">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="22ec5-121">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="22ec5-121">conversation</span></span>](conversation.md) |<span data-ttu-id="22ec5-122">Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="22ec5-122">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="22ec5-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="22ec5-123">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="22ec5-124">Keine</span><span class="sxs-lookup"><span data-stu-id="22ec5-124">None</span></span> |<span data-ttu-id="22ec5-125">Unterhaltungsobjekt löschen.</span><span class="sxs-lookup"><span data-stu-id="22ec5-125">Delete conversation object.</span></span> |
|[<span data-ttu-id="22ec5-126">Unterhaltungsthreads auflisten</span><span class="sxs-lookup"><span data-stu-id="22ec5-126">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="22ec5-127">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="22ec5-127">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="22ec5-128">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="22ec5-128">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="22ec5-129">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="22ec5-129">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="22ec5-130">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="22ec5-130">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="22ec5-131">Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="22ec5-131">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="22ec5-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="22ec5-132">Properties</span></span>
| <span data-ttu-id="22ec5-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22ec5-133">Property</span></span>     | <span data-ttu-id="22ec5-134">Typ</span><span class="sxs-lookup"><span data-stu-id="22ec5-134">Type</span></span>   |<span data-ttu-id="22ec5-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22ec5-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22ec5-136">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="22ec5-136">hasAttachments</span></span>|<span data-ttu-id="22ec5-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="22ec5-137">Boolean</span></span>|<span data-ttu-id="22ec5-138">Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="22ec5-138">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="22ec5-139">id</span><span class="sxs-lookup"><span data-stu-id="22ec5-139">id</span></span>|<span data-ttu-id="22ec5-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22ec5-140">String</span></span>|<span data-ttu-id="22ec5-p104">Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="22ec5-p104">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="22ec5-143">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="22ec5-143">lastDeliveredDateTime</span></span>|<span data-ttu-id="22ec5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ec5-144">DateTimeOffset</span></span>|<span data-ttu-id="22ec5-p105">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="22ec5-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="22ec5-147">Vorschau</span><span class="sxs-lookup"><span data-stu-id="22ec5-147">preview</span></span>|<span data-ttu-id="22ec5-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22ec5-148">String</span></span>|<span data-ttu-id="22ec5-149">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="22ec5-149">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="22ec5-150">Thema</span><span class="sxs-lookup"><span data-stu-id="22ec5-150">topic</span></span>|<span data-ttu-id="22ec5-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22ec5-151">String</span></span>|<span data-ttu-id="22ec5-p106">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="22ec5-p106">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="22ec5-154">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="22ec5-154">uniqueSenders</span></span>|<span data-ttu-id="22ec5-155">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="22ec5-155">String collection</span></span>|<span data-ttu-id="22ec5-156">Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="22ec5-156">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22ec5-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="22ec5-157">Relationships</span></span>
| <span data-ttu-id="22ec5-158">Beziehung</span><span class="sxs-lookup"><span data-stu-id="22ec5-158">Relationship</span></span> | <span data-ttu-id="22ec5-159">Typ</span><span class="sxs-lookup"><span data-stu-id="22ec5-159">Type</span></span>   |<span data-ttu-id="22ec5-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22ec5-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22ec5-161">Threads</span><span class="sxs-lookup"><span data-stu-id="22ec5-161">threads</span></span>|<span data-ttu-id="22ec5-162">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="22ec5-162">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="22ec5-p107">Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="22ec5-p107">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22ec5-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="22ec5-167">JSON representation</span></span>

<span data-ttu-id="22ec5-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="22ec5-168">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
