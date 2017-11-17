# <a name="conversationthread-resource-type"></a><span data-ttu-id="4e792-101">Ressourcentyp conversationThread</span><span class="sxs-lookup"><span data-stu-id="4e792-101">conversationThread resource type</span></span>
<span data-ttu-id="4e792-102">Ein conversationThread ist eine Sammlung von [Beiträgen](post.md).</span><span class="sxs-lookup"><span data-stu-id="4e792-102">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="4e792-p101">Die Empfängersammlung des letzten Beitrags besteht aus den aggregierten Empfängern des gesamten Threads. Ein Thread kann eine wachsende Sammlung von Empfängern haben. Ein neuer Thread wird erstellt, wenn ein Empfänger aus dem Thread entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="4e792-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="4e792-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="4e792-106">Methods</span></span>

| <span data-ttu-id="4e792-107">Methode</span><span class="sxs-lookup"><span data-stu-id="4e792-107">Method</span></span>       | <span data-ttu-id="4e792-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4e792-108">Return Type</span></span>  |<span data-ttu-id="4e792-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e792-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e792-110">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="4e792-110">List threads</span></span>](../api/group_list_threads.md) | <span data-ttu-id="4e792-111">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e792-111">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="4e792-112">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="4e792-112">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="4e792-113">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="4e792-113">Create thread</span></span>](../api/group_post_threads.md) | [<span data-ttu-id="4e792-114">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4e792-114">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4e792-p102">Beginnt eine neue Unterhaltung, indem zunächst ein Thread erstellt wird. Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="4e792-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="4e792-117">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="4e792-117">Get conversationThread</span></span>](../api/conversationthread_get.md) | [<span data-ttu-id="4e792-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4e792-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4e792-119">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="4e792-119">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="4e792-120">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4e792-120">Update</span></span>](../api/conversationthread_update.md) | [<span data-ttu-id="4e792-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4e792-121">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="4e792-122">conversationThread-Objekt aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="4e792-122">Update conversationThread object.</span></span> |
|[<span data-ttu-id="4e792-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="4e792-123">Delete</span></span>](../api/conversationthread_delete.md) | <span data-ttu-id="4e792-124">Keine</span><span class="sxs-lookup"><span data-stu-id="4e792-124">None</span></span> |<span data-ttu-id="4e792-125">conversationThread-Objekt löschen.</span><span class="sxs-lookup"><span data-stu-id="4e792-125">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="4e792-126">Antworten</span><span class="sxs-lookup"><span data-stu-id="4e792-126">Reply</span></span>](../api/conversationthread_reply.md)|<span data-ttu-id="4e792-127">Keine</span><span class="sxs-lookup"><span data-stu-id="4e792-127">None</span></span>|<span data-ttu-id="4e792-128">Antworten Sie auf diesen Thread, indem Sie eine neue Beitragsentität erstellen.</span><span class="sxs-lookup"><span data-stu-id="4e792-128">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="4e792-129">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="4e792-129">List Posts</span></span>](../api/conversationthread_list_posts.md) |<span data-ttu-id="4e792-130">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e792-130">[post](post.md) collection</span></span>| <span data-ttu-id="4e792-131">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="4e792-131">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e792-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e792-132">Properties</span></span>
| <span data-ttu-id="4e792-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e792-133">Property</span></span>     | <span data-ttu-id="4e792-134">Typ</span><span class="sxs-lookup"><span data-stu-id="4e792-134">Type</span></span>   |<span data-ttu-id="4e792-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e792-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e792-136">id</span><span class="sxs-lookup"><span data-stu-id="4e792-136">id</span></span>|<span data-ttu-id="4e792-137">String</span><span class="sxs-lookup"><span data-stu-id="4e792-137">String</span></span>| <span data-ttu-id="4e792-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e792-138">Read-only.</span></span>|
|<span data-ttu-id="4e792-139">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4e792-139">toRecipients</span></span>|<span data-ttu-id="4e792-140">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e792-140">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4e792-141">Die An:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="4e792-141">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="4e792-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="4e792-142">ccRecipients</span></span>|<span data-ttu-id="4e792-143">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e792-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4e792-144">Die Cc:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="4e792-144">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="4e792-145">Thema</span><span class="sxs-lookup"><span data-stu-id="4e792-145">topic</span></span>|<span data-ttu-id="4e792-146">String</span><span class="sxs-lookup"><span data-stu-id="4e792-146">String</span></span>|<span data-ttu-id="4e792-p103">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="4e792-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="4e792-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4e792-149">hasAttachments</span></span>|<span data-ttu-id="4e792-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e792-150">Boolean</span></span>|<span data-ttu-id="4e792-151">Gibt an, ob einer der Beiträge innerhalb dieses Threads über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="4e792-151">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="4e792-152">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="4e792-152">lastDeliveredDateTime</span></span>|<span data-ttu-id="4e792-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e792-153">DateTimeOffset</span></span>|<span data-ttu-id="4e792-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4e792-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4e792-156">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="4e792-156">uniqueSenders</span></span>|<span data-ttu-id="4e792-157">String collection</span><span class="sxs-lookup"><span data-stu-id="4e792-157">String collection</span></span>|<span data-ttu-id="4e792-158">Alle Benutzer, die eine Nachricht an diesen Thread gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="4e792-158">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="4e792-159">Vorschau</span><span class="sxs-lookup"><span data-stu-id="4e792-159">preview</span></span>|<span data-ttu-id="4e792-160">String</span><span class="sxs-lookup"><span data-stu-id="4e792-160">String</span></span>|<span data-ttu-id="4e792-161">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="4e792-161">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="4e792-162">isLocked</span><span class="sxs-lookup"><span data-stu-id="4e792-162">isLocked</span></span>|<span data-ttu-id="4e792-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e792-163">Boolean</span></span>|<span data-ttu-id="4e792-164">Zeigt an, ob der Thread gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="4e792-164">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e792-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4e792-165">Relationships</span></span>
| <span data-ttu-id="4e792-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4e792-166">Relationship</span></span> | <span data-ttu-id="4e792-167">Typ</span><span class="sxs-lookup"><span data-stu-id="4e792-167">Type</span></span>   |<span data-ttu-id="4e792-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e792-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e792-169">posts</span><span class="sxs-lookup"><span data-stu-id="4e792-169">posts</span></span>|<span data-ttu-id="4e792-170">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e792-170">[post](post.md) collection</span></span>| <span data-ttu-id="4e792-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4e792-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e792-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e792-173">JSON representation</span></span>

<span data-ttu-id="4e792-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e792-174">Here is a JSON representation of the resource</span></span>

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
