---
title: Ressourcentyp conversation
description: Eine Unterhaltung ist eine Sammlung von Threads, und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0066a636d2b36e74443380598c2ca6e8daf826c1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928157"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="38cfd-104">Ressourcentyp conversation</span><span class="sxs-lookup"><span data-stu-id="38cfd-104">conversation resource type</span></span>

<span data-ttu-id="38cfd-p102">Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.</span><span class="sxs-lookup"><span data-stu-id="38cfd-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="38cfd-107">Diese Ressource unterstützt Abonnieren von [Benachrichtigungen ändern](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="38cfd-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="38cfd-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="38cfd-108">Methods</span></span>

| <span data-ttu-id="38cfd-109">Methode</span><span class="sxs-lookup"><span data-stu-id="38cfd-109">Method</span></span>       | <span data-ttu-id="38cfd-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="38cfd-110">Return Type</span></span>  |<span data-ttu-id="38cfd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38cfd-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38cfd-112">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="38cfd-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="38cfd-113">[conversation](conversation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38cfd-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="38cfd-114">Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="38cfd-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="38cfd-115">Erstellen</span><span class="sxs-lookup"><span data-stu-id="38cfd-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="38cfd-116">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="38cfd-116">conversation</span></span>](conversation.md)| <span data-ttu-id="38cfd-117">Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="38cfd-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="38cfd-118">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="38cfd-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="38cfd-119">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="38cfd-119">conversation</span></span>](conversation.md) |<span data-ttu-id="38cfd-120">Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="38cfd-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="38cfd-121">Löschen</span><span class="sxs-lookup"><span data-stu-id="38cfd-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="38cfd-122">Keine</span><span class="sxs-lookup"><span data-stu-id="38cfd-122">None</span></span> |<span data-ttu-id="38cfd-123">Unterhaltungsobjekt löschen.</span><span class="sxs-lookup"><span data-stu-id="38cfd-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="38cfd-124">Unterhaltungsthreads auflisten</span><span class="sxs-lookup"><span data-stu-id="38cfd-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="38cfd-125">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38cfd-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="38cfd-126">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="38cfd-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="38cfd-127">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="38cfd-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="38cfd-128">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38cfd-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="38cfd-129">Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="38cfd-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="38cfd-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38cfd-130">Properties</span></span>
| <span data-ttu-id="38cfd-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38cfd-131">Property</span></span>     | <span data-ttu-id="38cfd-132">Typ</span><span class="sxs-lookup"><span data-stu-id="38cfd-132">Type</span></span>   |<span data-ttu-id="38cfd-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38cfd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38cfd-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="38cfd-134">hasAttachments</span></span>|<span data-ttu-id="38cfd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="38cfd-135">Boolean</span></span>|<span data-ttu-id="38cfd-136">Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="38cfd-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="38cfd-137">id</span><span class="sxs-lookup"><span data-stu-id="38cfd-137">id</span></span>|<span data-ttu-id="38cfd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38cfd-138">String</span></span>|<span data-ttu-id="38cfd-p103">Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38cfd-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="38cfd-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="38cfd-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="38cfd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38cfd-142">DateTimeOffset</span></span>|<span data-ttu-id="38cfd-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="38cfd-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="38cfd-145">Vorschau</span><span class="sxs-lookup"><span data-stu-id="38cfd-145">preview</span></span>|<span data-ttu-id="38cfd-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38cfd-146">String</span></span>|<span data-ttu-id="38cfd-147">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="38cfd-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="38cfd-148">Thema</span><span class="sxs-lookup"><span data-stu-id="38cfd-148">topic</span></span>|<span data-ttu-id="38cfd-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38cfd-149">String</span></span>|<span data-ttu-id="38cfd-p105">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="38cfd-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="38cfd-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="38cfd-152">uniqueSenders</span></span>|<span data-ttu-id="38cfd-153">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="38cfd-153">String collection</span></span>|<span data-ttu-id="38cfd-154">Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="38cfd-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38cfd-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="38cfd-155">Relationships</span></span>
| <span data-ttu-id="38cfd-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="38cfd-156">Relationship</span></span> | <span data-ttu-id="38cfd-157">Typ</span><span class="sxs-lookup"><span data-stu-id="38cfd-157">Type</span></span>   |<span data-ttu-id="38cfd-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38cfd-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38cfd-159">Threads</span><span class="sxs-lookup"><span data-stu-id="38cfd-159">threads</span></span>|<span data-ttu-id="38cfd-160">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38cfd-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="38cfd-p106">Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="38cfd-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38cfd-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38cfd-165">JSON representation</span></span>

<span data-ttu-id="38cfd-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38cfd-166">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
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
