---
title: Ressourcentyp conversationThread
description: Ein conversationThread ist eine Sammlung von Beiträgen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 1101bb56e69b6418cfd57e719cf1633fa76b161c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845269"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="4ab50-103">Ressourcentyp conversationThread</span><span class="sxs-lookup"><span data-stu-id="4ab50-103">conversationThread resource type</span></span>

> <span data-ttu-id="4ab50-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4ab50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ab50-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ab50-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ab50-106">Ein conversationThread ist eine Sammlung von [Beiträgen](post.md).</span><span class="sxs-lookup"><span data-stu-id="4ab50-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="4ab50-p102">Die Empfängersammlung des letzten Beitrags besteht aus den aggregierten Empfängern des gesamten Threads. Ein Thread kann eine wachsende Sammlung von Empfängern haben. Ein neuer Thread wird erstellt, wenn ein Empfänger aus dem Thread entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="4ab50-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="4ab50-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="4ab50-110">Methods</span></span>

| <span data-ttu-id="4ab50-111">Methode</span><span class="sxs-lookup"><span data-stu-id="4ab50-111">Method</span></span>       | <span data-ttu-id="4ab50-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4ab50-112">Return Type</span></span>  |<span data-ttu-id="4ab50-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ab50-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ab50-114">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="4ab50-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="4ab50-115">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4ab50-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="4ab50-116">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="4ab50-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="4ab50-117">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="4ab50-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="4ab50-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4ab50-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4ab50-p103">Beginnt eine neue Unterhaltung, indem zunächst ein Thread erstellt wird. Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="4ab50-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="4ab50-121">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="4ab50-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="4ab50-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4ab50-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4ab50-123">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="4ab50-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="4ab50-124">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4ab50-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="4ab50-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4ab50-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="4ab50-126">conversationThread-Objekt aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="4ab50-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="4ab50-127">Löschen</span><span class="sxs-lookup"><span data-stu-id="4ab50-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="4ab50-128">Keine</span><span class="sxs-lookup"><span data-stu-id="4ab50-128">None</span></span> |<span data-ttu-id="4ab50-129">conversationThread-Objekt löschen.</span><span class="sxs-lookup"><span data-stu-id="4ab50-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="4ab50-130">Antworten</span><span class="sxs-lookup"><span data-stu-id="4ab50-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="4ab50-131">Keine</span><span class="sxs-lookup"><span data-stu-id="4ab50-131">None</span></span>|<span data-ttu-id="4ab50-132">Antworten Sie auf diesen Thread, indem Sie eine neue Beitragsentität erstellen.</span><span class="sxs-lookup"><span data-stu-id="4ab50-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="4ab50-133">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="4ab50-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="4ab50-134">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4ab50-134">[post](post.md) collection</span></span>| <span data-ttu-id="4ab50-135">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="4ab50-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ab50-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ab50-136">Properties</span></span>
| <span data-ttu-id="4ab50-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ab50-137">Property</span></span>     | <span data-ttu-id="4ab50-138">Typ</span><span class="sxs-lookup"><span data-stu-id="4ab50-138">Type</span></span>   |<span data-ttu-id="4ab50-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ab50-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ab50-140">id</span><span class="sxs-lookup"><span data-stu-id="4ab50-140">id</span></span>|<span data-ttu-id="4ab50-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ab50-141">String</span></span>| <span data-ttu-id="4ab50-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4ab50-142">Read-only.</span></span>|
|<span data-ttu-id="4ab50-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4ab50-143">toRecipients</span></span>|<span data-ttu-id="4ab50-144">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4ab50-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4ab50-145">Die An:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="4ab50-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="4ab50-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="4ab50-146">ccRecipients</span></span>|<span data-ttu-id="4ab50-147">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4ab50-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4ab50-148">Die Cc:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="4ab50-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="4ab50-149">Thema</span><span class="sxs-lookup"><span data-stu-id="4ab50-149">topic</span></span>|<span data-ttu-id="4ab50-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ab50-150">String</span></span>|<span data-ttu-id="4ab50-p104">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="4ab50-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="4ab50-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4ab50-153">hasAttachments</span></span>|<span data-ttu-id="4ab50-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab50-154">Boolean</span></span>|<span data-ttu-id="4ab50-155">Gibt an, ob einer der Beiträge innerhalb dieses Threads über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="4ab50-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="4ab50-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab50-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="4ab50-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab50-157">DateTimeOffset</span></span>|<span data-ttu-id="4ab50-p105">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4ab50-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4ab50-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="4ab50-160">uniqueSenders</span></span>|<span data-ttu-id="4ab50-161">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4ab50-161">String collection</span></span>|<span data-ttu-id="4ab50-162">Alle Benutzer, die eine Nachricht an diesen Thread gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="4ab50-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="4ab50-163">Vorschau</span><span class="sxs-lookup"><span data-stu-id="4ab50-163">preview</span></span>|<span data-ttu-id="4ab50-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ab50-164">String</span></span>|<span data-ttu-id="4ab50-165">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="4ab50-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="4ab50-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="4ab50-166">isLocked</span></span>|<span data-ttu-id="4ab50-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab50-167">Boolean</span></span>|<span data-ttu-id="4ab50-168">Zeigt an, ob der Thread gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="4ab50-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ab50-169">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4ab50-169">Relationships</span></span>
| <span data-ttu-id="4ab50-170">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4ab50-170">Relationship</span></span> | <span data-ttu-id="4ab50-171">Typ</span><span class="sxs-lookup"><span data-stu-id="4ab50-171">Type</span></span>   |<span data-ttu-id="4ab50-172">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ab50-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ab50-173">posts</span><span class="sxs-lookup"><span data-stu-id="4ab50-173">posts</span></span>|<span data-ttu-id="4ab50-174">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4ab50-174">[post](post.md) collection</span></span>| <span data-ttu-id="4ab50-p106">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4ab50-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ab50-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4ab50-177">JSON representation</span></span>

<span data-ttu-id="4ab50-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4ab50-178">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
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
