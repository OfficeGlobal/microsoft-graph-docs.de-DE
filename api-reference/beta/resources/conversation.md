---
title: Ressourcentyp conversation
description: Eine Unterhaltung ist eine Sammlung von Threads, und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7d489a75f72a705a77231af940094b7aa2d18fe1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528648"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="b2d74-104">Ressourcentyp conversation</span><span class="sxs-lookup"><span data-stu-id="b2d74-104">conversation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d74-p102">Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.</span><span class="sxs-lookup"><span data-stu-id="b2d74-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="b2d74-107">Diese Ressource unterstützt Abonnieren von [Benachrichtigungen ändern](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="b2d74-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="b2d74-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="b2d74-108">Methods</span></span>

| <span data-ttu-id="b2d74-109">Methode</span><span class="sxs-lookup"><span data-stu-id="b2d74-109">Method</span></span>       | <span data-ttu-id="b2d74-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b2d74-110">Return Type</span></span>  |<span data-ttu-id="b2d74-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2d74-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2d74-112">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="b2d74-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="b2d74-113">[conversation](conversation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2d74-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="b2d74-114">Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="b2d74-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="b2d74-115">Erstellen</span><span class="sxs-lookup"><span data-stu-id="b2d74-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="b2d74-116">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="b2d74-116">conversation</span></span>](conversation.md)| <span data-ttu-id="b2d74-117">Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="b2d74-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="b2d74-118">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="b2d74-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="b2d74-119">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="b2d74-119">conversation</span></span>](conversation.md) |<span data-ttu-id="b2d74-120">Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="b2d74-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="b2d74-121">Löschen</span><span class="sxs-lookup"><span data-stu-id="b2d74-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="b2d74-122">Keine</span><span class="sxs-lookup"><span data-stu-id="b2d74-122">None</span></span> |<span data-ttu-id="b2d74-123">Unterhaltungsobjekt löschen.</span><span class="sxs-lookup"><span data-stu-id="b2d74-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="b2d74-124">Unterhaltungsthreads auflisten</span><span class="sxs-lookup"><span data-stu-id="b2d74-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="b2d74-125">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2d74-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="b2d74-126">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="b2d74-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="b2d74-127">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="b2d74-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="b2d74-128">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2d74-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="b2d74-129">Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="b2d74-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2d74-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2d74-130">Properties</span></span>
| <span data-ttu-id="b2d74-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2d74-131">Property</span></span>     | <span data-ttu-id="b2d74-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b2d74-132">Type</span></span>   |<span data-ttu-id="b2d74-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2d74-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2d74-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="b2d74-134">hasAttachments</span></span>|<span data-ttu-id="b2d74-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2d74-135">Boolean</span></span>|<span data-ttu-id="b2d74-136">Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="b2d74-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="b2d74-137">id</span><span class="sxs-lookup"><span data-stu-id="b2d74-137">id</span></span>|<span data-ttu-id="b2d74-138">String</span><span class="sxs-lookup"><span data-stu-id="b2d74-138">String</span></span>|<span data-ttu-id="b2d74-p103">Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b2d74-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="b2d74-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="b2d74-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="b2d74-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2d74-142">DateTimeOffset</span></span>|<span data-ttu-id="b2d74-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b2d74-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b2d74-145">Vorschau</span><span class="sxs-lookup"><span data-stu-id="b2d74-145">preview</span></span>|<span data-ttu-id="b2d74-146">String</span><span class="sxs-lookup"><span data-stu-id="b2d74-146">String</span></span>|<span data-ttu-id="b2d74-147">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="b2d74-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="b2d74-148">Thema</span><span class="sxs-lookup"><span data-stu-id="b2d74-148">topic</span></span>|<span data-ttu-id="b2d74-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2d74-149">String</span></span>|<span data-ttu-id="b2d74-p105">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b2d74-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="b2d74-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="b2d74-152">uniqueSenders</span></span>|<span data-ttu-id="b2d74-153">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b2d74-153">String collection</span></span>|<span data-ttu-id="b2d74-154">Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="b2d74-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2d74-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b2d74-155">Relationships</span></span>
| <span data-ttu-id="b2d74-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b2d74-156">Relationship</span></span> | <span data-ttu-id="b2d74-157">Typ</span><span class="sxs-lookup"><span data-stu-id="b2d74-157">Type</span></span>   |<span data-ttu-id="b2d74-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2d74-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2d74-159">Threads</span><span class="sxs-lookup"><span data-stu-id="b2d74-159">threads</span></span>|<span data-ttu-id="b2d74-160">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2d74-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="b2d74-p106">Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b2d74-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2d74-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2d74-165">JSON representation</span></span>

<span data-ttu-id="b2d74-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2d74-166">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/conversation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
