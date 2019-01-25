---
title: Ressourcentyp conversationThread
description: Ein conversationThread ist eine Sammlung von Beiträgen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 504b8b8d4e47f892da72ea7ef9588491d0642f21
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508174"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="d63de-103">Ressourcentyp conversationThread</span><span class="sxs-lookup"><span data-stu-id="d63de-103">conversationThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d63de-104">Ein conversationThread ist eine Sammlung von [Beiträgen](post.md).</span><span class="sxs-lookup"><span data-stu-id="d63de-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="d63de-p101">Die Empfängersammlung des letzten Beitrags besteht aus den aggregierten Empfängern des gesamten Threads. Ein Thread kann eine wachsende Sammlung von Empfängern haben. Ein neuer Thread wird erstellt, wenn ein Empfänger aus dem Thread entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="d63de-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="d63de-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="d63de-108">Methods</span></span>

| <span data-ttu-id="d63de-109">Methode</span><span class="sxs-lookup"><span data-stu-id="d63de-109">Method</span></span>       | <span data-ttu-id="d63de-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d63de-110">Return Type</span></span>  |<span data-ttu-id="d63de-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d63de-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d63de-112">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="d63de-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="d63de-113">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d63de-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="d63de-114">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="d63de-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="d63de-115">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="d63de-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="d63de-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="d63de-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="d63de-p102">Beginnt eine neue Unterhaltung, indem zunächst ein Thread erstellt wird. Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="d63de-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="d63de-119">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="d63de-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="d63de-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="d63de-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="d63de-121">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="d63de-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="d63de-122">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d63de-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="d63de-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="d63de-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="d63de-124">conversationThread-Objekt aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d63de-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="d63de-125">Löschen</span><span class="sxs-lookup"><span data-stu-id="d63de-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="d63de-126">Keine</span><span class="sxs-lookup"><span data-stu-id="d63de-126">None</span></span> |<span data-ttu-id="d63de-127">conversationThread-Objekt löschen.</span><span class="sxs-lookup"><span data-stu-id="d63de-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="d63de-128">Antworten</span><span class="sxs-lookup"><span data-stu-id="d63de-128">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="d63de-129">Keine</span><span class="sxs-lookup"><span data-stu-id="d63de-129">None</span></span>|<span data-ttu-id="d63de-130">Antworten Sie auf diesen Thread, indem Sie eine neue Beitragsentität erstellen.</span><span class="sxs-lookup"><span data-stu-id="d63de-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="d63de-131">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="d63de-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="d63de-132">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d63de-132">[post](post.md) collection</span></span>| <span data-ttu-id="d63de-133">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="d63de-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="d63de-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d63de-134">Properties</span></span>
| <span data-ttu-id="d63de-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d63de-135">Property</span></span>     | <span data-ttu-id="d63de-136">Typ</span><span class="sxs-lookup"><span data-stu-id="d63de-136">Type</span></span>   |<span data-ttu-id="d63de-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d63de-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d63de-138">id</span><span class="sxs-lookup"><span data-stu-id="d63de-138">id</span></span>|<span data-ttu-id="d63de-139">String</span><span class="sxs-lookup"><span data-stu-id="d63de-139">String</span></span>| <span data-ttu-id="d63de-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d63de-140">Read-only.</span></span>|
|<span data-ttu-id="d63de-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d63de-141">toRecipients</span></span>|<span data-ttu-id="d63de-142">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="d63de-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="d63de-143">Die An:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="d63de-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="d63de-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="d63de-144">ccRecipients</span></span>|<span data-ttu-id="d63de-145">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d63de-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="d63de-146">Die Cc:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="d63de-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="d63de-147">Thema</span><span class="sxs-lookup"><span data-stu-id="d63de-147">topic</span></span>|<span data-ttu-id="d63de-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d63de-148">String</span></span>|<span data-ttu-id="d63de-p103">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="d63de-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="d63de-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="d63de-151">hasAttachments</span></span>|<span data-ttu-id="d63de-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d63de-152">Boolean</span></span>|<span data-ttu-id="d63de-153">Gibt an, ob einer der Beiträge innerhalb dieses Threads über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="d63de-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="d63de-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="d63de-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="d63de-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d63de-155">DateTimeOffset</span></span>|<span data-ttu-id="d63de-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d63de-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d63de-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="d63de-158">uniqueSenders</span></span>|<span data-ttu-id="d63de-159">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d63de-159">String collection</span></span>|<span data-ttu-id="d63de-160">Alle Benutzer, die eine Nachricht an diesen Thread gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="d63de-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="d63de-161">Vorschau</span><span class="sxs-lookup"><span data-stu-id="d63de-161">preview</span></span>|<span data-ttu-id="d63de-162">String</span><span class="sxs-lookup"><span data-stu-id="d63de-162">String</span></span>|<span data-ttu-id="d63de-163">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="d63de-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="d63de-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="d63de-164">isLocked</span></span>|<span data-ttu-id="d63de-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="d63de-165">Boolean</span></span>|<span data-ttu-id="d63de-166">Zeigt an, ob der Thread gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="d63de-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d63de-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d63de-167">Relationships</span></span>
| <span data-ttu-id="d63de-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d63de-168">Relationship</span></span> | <span data-ttu-id="d63de-169">Typ</span><span class="sxs-lookup"><span data-stu-id="d63de-169">Type</span></span>   |<span data-ttu-id="d63de-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d63de-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d63de-171">posts</span><span class="sxs-lookup"><span data-stu-id="d63de-171">posts</span></span>|<span data-ttu-id="d63de-172">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d63de-172">[post](post.md) collection</span></span>| <span data-ttu-id="d63de-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d63de-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d63de-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d63de-175">JSON representation</span></span>

<span data-ttu-id="d63de-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d63de-176">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/conversationthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
