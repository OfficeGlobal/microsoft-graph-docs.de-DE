# <a name="conversationthread-resource-type"></a><span data-ttu-id="fbdbe-101">Ressourcentyp conversationThread</span><span class="sxs-lookup"><span data-stu-id="fbdbe-101">conversationThread resource type</span></span>
<span data-ttu-id="fbdbe-102">Ein conversationThread ist eine Sammlung von [Beiträgen](post.md).</span><span class="sxs-lookup"><span data-stu-id="fbdbe-102">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="fbdbe-p101">Die Empfängersammlung des letzten Beitrags besteht aus den aggregierten Empfängern des gesamten Threads. Ein Thread kann eine wachsende Sammlung von Empfängern haben. Ein neuer Thread wird erstellt, wenn ein Empfänger aus dem Thread entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="fbdbe-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="fbdbe-106">Methods</span></span>

| <span data-ttu-id="fbdbe-107">Methode</span><span class="sxs-lookup"><span data-stu-id="fbdbe-107">Method</span></span>       | <span data-ttu-id="fbdbe-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fbdbe-108">Return Type</span></span>  |<span data-ttu-id="fbdbe-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbdbe-110">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="fbdbe-110">List threads</span></span>](../api/group_list_threads.md) | <span data-ttu-id="fbdbe-111">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-111">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="fbdbe-112">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-112">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="fbdbe-113">Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="fbdbe-113">Create thread</span></span>](../api/group_post_threads.md) | [<span data-ttu-id="fbdbe-114">conversationThread</span><span class="sxs-lookup"><span data-stu-id="fbdbe-114">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="fbdbe-p102">Beginnt eine neue Unterhaltung, indem zunächst ein Thread erstellt wird. Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="fbdbe-117">conversationThread abrufen</span><span class="sxs-lookup"><span data-stu-id="fbdbe-117">Get conversationThread</span></span>](../api/conversationthread_get.md) | [<span data-ttu-id="fbdbe-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="fbdbe-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="fbdbe-119">Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-119">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="fbdbe-120">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fbdbe-120">Update</span></span>](../api/conversationthread_update.md) | [<span data-ttu-id="fbdbe-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="fbdbe-121">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="fbdbe-122">conversationThread-Objekt aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-122">Update conversationThread object.</span></span> |
|[<span data-ttu-id="fbdbe-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="fbdbe-123">Delete</span></span>](../api/conversationthread_delete.md) | <span data-ttu-id="fbdbe-124">Keine</span><span class="sxs-lookup"><span data-stu-id="fbdbe-124">None</span></span> |<span data-ttu-id="fbdbe-125">conversationThread-Objekt löschen.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-125">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="fbdbe-126">Antworten</span><span class="sxs-lookup"><span data-stu-id="fbdbe-126">Reply</span></span>](../api/conversationthread_reply.md)|<span data-ttu-id="fbdbe-127">Keine</span><span class="sxs-lookup"><span data-stu-id="fbdbe-127">None</span></span>|<span data-ttu-id="fbdbe-128">Antworten Sie auf diesen Thread, indem Sie eine neue Beitragsentität erstellen.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-128">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="fbdbe-129">Beiträge auflisten</span><span class="sxs-lookup"><span data-stu-id="fbdbe-129">List Posts</span></span>](../api/conversationthread_list_posts.md) |<span data-ttu-id="fbdbe-130">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-130">[post](post.md) collection</span></span>| <span data-ttu-id="fbdbe-131">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-131">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="fbdbe-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fbdbe-132">Properties</span></span>
| <span data-ttu-id="fbdbe-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fbdbe-133">Property</span></span>     | <span data-ttu-id="fbdbe-134">Typ</span><span class="sxs-lookup"><span data-stu-id="fbdbe-134">Type</span></span>   |<span data-ttu-id="fbdbe-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbdbe-136">id</span><span class="sxs-lookup"><span data-stu-id="fbdbe-136">id</span></span>|<span data-ttu-id="fbdbe-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fbdbe-137">String</span></span>| <span data-ttu-id="fbdbe-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-138">Read-only.</span></span>|
|<span data-ttu-id="fbdbe-139">toRecipients</span><span class="sxs-lookup"><span data-stu-id="fbdbe-139">toRecipients</span></span>|<span data-ttu-id="fbdbe-140">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-140">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="fbdbe-141">Die An:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-141">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="fbdbe-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="fbdbe-142">ccRecipients</span></span>|<span data-ttu-id="fbdbe-143">[recipient](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="fbdbe-144">Die Cc:-Empfänger des Threads.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-144">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="fbdbe-145">Thema</span><span class="sxs-lookup"><span data-stu-id="fbdbe-145">topic</span></span>|<span data-ttu-id="fbdbe-146">String</span><span class="sxs-lookup"><span data-stu-id="fbdbe-146">String</span></span>|<span data-ttu-id="fbdbe-p103">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="fbdbe-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="fbdbe-149">hasAttachments</span></span>|<span data-ttu-id="fbdbe-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbdbe-150">Boolean</span></span>|<span data-ttu-id="fbdbe-151">Gibt an, ob einer der Beiträge innerhalb dieses Threads über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-151">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="fbdbe-152">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="fbdbe-152">lastDeliveredDateTime</span></span>|<span data-ttu-id="fbdbe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbdbe-153">DateTimeOffset</span></span>|<span data-ttu-id="fbdbe-p104">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fbdbe-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fbdbe-156">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="fbdbe-156">uniqueSenders</span></span>|<span data-ttu-id="fbdbe-157">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-157">String collection</span></span>|<span data-ttu-id="fbdbe-158">Alle Benutzer, die eine Nachricht an diesen Thread gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-158">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="fbdbe-159">Vorschau</span><span class="sxs-lookup"><span data-stu-id="fbdbe-159">preview</span></span>|<span data-ttu-id="fbdbe-160">String</span><span class="sxs-lookup"><span data-stu-id="fbdbe-160">String</span></span>|<span data-ttu-id="fbdbe-161">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-161">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="fbdbe-162">isLocked</span><span class="sxs-lookup"><span data-stu-id="fbdbe-162">isLocked</span></span>|<span data-ttu-id="fbdbe-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbdbe-163">Boolean</span></span>|<span data-ttu-id="fbdbe-164">Zeigt an, ob der Thread gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-164">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbdbe-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fbdbe-165">Relationships</span></span>
| <span data-ttu-id="fbdbe-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-166">Relationship</span></span> | <span data-ttu-id="fbdbe-167">Typ</span><span class="sxs-lookup"><span data-stu-id="fbdbe-167">Type</span></span>   |<span data-ttu-id="fbdbe-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbdbe-169">posts</span><span class="sxs-lookup"><span data-stu-id="fbdbe-169">posts</span></span>|<span data-ttu-id="fbdbe-170">[post](post.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-170">[post](post.md) collection</span></span>| <span data-ttu-id="fbdbe-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbdbe-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fbdbe-173">JSON representation</span></span>

<span data-ttu-id="fbdbe-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fbdbe-174">Here is a JSON representation of the resource</span></span>

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
