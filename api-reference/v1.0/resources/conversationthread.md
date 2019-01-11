---
title: Ressourcentyp conversationThread
description: Ein conversationThread ist eine Sammlung von Beiträgen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 89f57e90551efbea435181c35751d54168c498f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886429"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="3329a-103">Ressourcentyp conversationThread</span><span class="sxs-lookup"><span data-stu-id="3329a-103">conversationThread resource type</span></span>
<span data-ttu-id="3329a-104">Ein conversationThread ist eine Sammlung von [Beiträgen](post.md).</span><span class="sxs-lookup"><span data-stu-id="3329a-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="3329a-p101">Die Empfängersammlung des letzten Beitrags besteht aus den aggregierten Empfängern des gesamten Threads. Ein Thread kann eine wachsende Sammlung von Empfängern haben. Ein neuer Thread wird erstellt, wenn ein Empfänger aus dem Thread entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="3329a-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="3329a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="3329a-108">Methods</span></span>

| <span data-ttu-id="3329a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="3329a-109">Method</span></span>       | <span data-ttu-id="3329a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3329a-110">Return Type</span></span>  |<span data-ttu-id="3329a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3329a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3329a-112">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="3329a-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="3329a-113">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3329a-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="3329a-114">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="3329a-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="3329a-115">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="3329a-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="3329a-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="3329a-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="3329a-p102">Beginnt eine neue Unterhaltung, indem zunächst ein Thread erstellt wird. Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="3329a-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="3329a-119">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="3329a-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="3329a-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="3329a-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="3329a-121">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="3329a-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="3329a-122">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3329a-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="3329a-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="3329a-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="3329a-124">conversationThread-Objekt aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="3329a-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="3329a-125">Löschen</span><span class="sxs-lookup"><span data-stu-id="3329a-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="3329a-126">Keine</span><span class="sxs-lookup"><span data-stu-id="3329a-126">None</span></span> |<span data-ttu-id="3329a-127">conversationThread-Objekt löschen.</span><span class="sxs-lookup"><span data-stu-id="3329a-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="3329a-128">Antworten</span><span class="sxs-lookup"><span data-stu-id="3329a-128">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="3329a-129">Keine</span><span class="sxs-lookup"><span data-stu-id="3329a-129">None</span></span>|<span data-ttu-id="3329a-130">Antworten Sie auf diesen Thread, indem Sie eine neue Beitragsentität erstellen.</span><span class="sxs-lookup"><span data-stu-id="3329a-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="3329a-131">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="3329a-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="3329a-132">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3329a-132">[post](post.md) collection</span></span>| <span data-ttu-id="3329a-133">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="3329a-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="3329a-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3329a-134">Properties</span></span>
| <span data-ttu-id="3329a-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3329a-135">Property</span></span>     | <span data-ttu-id="3329a-136">Typ</span><span class="sxs-lookup"><span data-stu-id="3329a-136">Type</span></span>   |<span data-ttu-id="3329a-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3329a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3329a-138">id</span><span class="sxs-lookup"><span data-stu-id="3329a-138">id</span></span>|<span data-ttu-id="3329a-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3329a-139">String</span></span>| <span data-ttu-id="3329a-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3329a-140">Read-only.</span></span>|
|<span data-ttu-id="3329a-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="3329a-141">toRecipients</span></span>|<span data-ttu-id="3329a-142">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3329a-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="3329a-143">Die An:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="3329a-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="3329a-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="3329a-144">ccRecipients</span></span>|<span data-ttu-id="3329a-145">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3329a-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="3329a-146">Die Cc:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="3329a-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="3329a-147">Thema</span><span class="sxs-lookup"><span data-stu-id="3329a-147">topic</span></span>|<span data-ttu-id="3329a-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3329a-148">String</span></span>|<span data-ttu-id="3329a-p103">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="3329a-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="3329a-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="3329a-151">hasAttachments</span></span>|<span data-ttu-id="3329a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="3329a-152">Boolean</span></span>|<span data-ttu-id="3329a-153">Gibt an, ob einer der Beiträge innerhalb dieses Threads über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="3329a-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="3329a-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="3329a-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="3329a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3329a-155">DateTimeOffset</span></span>|<span data-ttu-id="3329a-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3329a-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3329a-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="3329a-158">uniqueSenders</span></span>|<span data-ttu-id="3329a-159">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3329a-159">String collection</span></span>|<span data-ttu-id="3329a-160">Alle Benutzer, die eine Nachricht an diesen Thread gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="3329a-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="3329a-161">Vorschau</span><span class="sxs-lookup"><span data-stu-id="3329a-161">preview</span></span>|<span data-ttu-id="3329a-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3329a-162">String</span></span>|<span data-ttu-id="3329a-163">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="3329a-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="3329a-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="3329a-164">isLocked</span></span>|<span data-ttu-id="3329a-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3329a-165">Boolean</span></span>|<span data-ttu-id="3329a-166">Zeigt an, ob der Thread gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="3329a-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3329a-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3329a-167">Relationships</span></span>
| <span data-ttu-id="3329a-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3329a-168">Relationship</span></span> | <span data-ttu-id="3329a-169">Typ</span><span class="sxs-lookup"><span data-stu-id="3329a-169">Type</span></span>   |<span data-ttu-id="3329a-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3329a-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3329a-171">posts</span><span class="sxs-lookup"><span data-stu-id="3329a-171">posts</span></span>|<span data-ttu-id="3329a-172">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3329a-172">[post](post.md) collection</span></span>| <span data-ttu-id="3329a-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="3329a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3329a-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3329a-175">JSON representation</span></span>

<span data-ttu-id="3329a-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3329a-176">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
