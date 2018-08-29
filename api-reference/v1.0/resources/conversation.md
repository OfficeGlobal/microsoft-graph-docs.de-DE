# <a name="conversation-resource-type"></a><span data-ttu-id="e67a0-101">Ressourcentyp conversation</span><span class="sxs-lookup"><span data-stu-id="e67a0-101">conversation resource type</span></span>

<span data-ttu-id="e67a0-p101">Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.</span><span class="sxs-lookup"><span data-stu-id="e67a0-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

## <a name="methods"></a><span data-ttu-id="e67a0-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="e67a0-104">Methods</span></span>

| <span data-ttu-id="e67a0-105">Methode</span><span class="sxs-lookup"><span data-stu-id="e67a0-105">Method</span></span>       | <span data-ttu-id="e67a0-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e67a0-106">Return Type</span></span>  |<span data-ttu-id="e67a0-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e67a0-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e67a0-108">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="e67a0-108">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="e67a0-109">[conversation](conversation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e67a0-109">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="e67a0-110">Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e67a0-110">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="e67a0-111">Erstellen</span><span class="sxs-lookup"><span data-stu-id="e67a0-111">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="e67a0-112">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="e67a0-112">conversation</span></span>](conversation.md)| <span data-ttu-id="e67a0-113">Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="e67a0-113">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="e67a0-114">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="e67a0-114">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="e67a0-115">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="e67a0-115">conversation</span></span>](conversation.md) |<span data-ttu-id="e67a0-116">Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="e67a0-116">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="e67a0-117">Löschen</span><span class="sxs-lookup"><span data-stu-id="e67a0-117">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="e67a0-118">Keine</span><span class="sxs-lookup"><span data-stu-id="e67a0-118">None</span></span> |<span data-ttu-id="e67a0-119">Unterhaltungsobjekt löschen.</span><span class="sxs-lookup"><span data-stu-id="e67a0-119">Delete conversation object.</span></span> |
|[<span data-ttu-id="e67a0-120">Unterhaltungsthreads auflisten</span><span class="sxs-lookup"><span data-stu-id="e67a0-120">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="e67a0-121">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e67a0-121">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="e67a0-122">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="e67a0-122">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="e67a0-123">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="e67a0-123">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="e67a0-124">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e67a0-124">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="e67a0-125">Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="e67a0-125">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e67a0-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e67a0-126">Properties</span></span>
| <span data-ttu-id="e67a0-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e67a0-127">Property</span></span>     | <span data-ttu-id="e67a0-128">Typ</span><span class="sxs-lookup"><span data-stu-id="e67a0-128">Type</span></span>   |<span data-ttu-id="e67a0-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e67a0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e67a0-130">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e67a0-130">hasAttachments</span></span>|<span data-ttu-id="e67a0-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="e67a0-131">Boolean</span></span>|<span data-ttu-id="e67a0-132">Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="e67a0-132">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="e67a0-133">id</span><span class="sxs-lookup"><span data-stu-id="e67a0-133">id</span></span>|<span data-ttu-id="e67a0-134">String</span><span class="sxs-lookup"><span data-stu-id="e67a0-134">String</span></span>|<span data-ttu-id="e67a0-p102">Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e67a0-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="e67a0-137">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="e67a0-137">lastDeliveredDateTime</span></span>|<span data-ttu-id="e67a0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e67a0-138">DateTimeOffset</span></span>|<span data-ttu-id="e67a0-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e67a0-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e67a0-141">Vorschau</span><span class="sxs-lookup"><span data-stu-id="e67a0-141">preview</span></span>|<span data-ttu-id="e67a0-142">String</span><span class="sxs-lookup"><span data-stu-id="e67a0-142">String</span></span>|<span data-ttu-id="e67a0-143">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="e67a0-143">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="e67a0-144">Thema</span><span class="sxs-lookup"><span data-stu-id="e67a0-144">topic</span></span>|<span data-ttu-id="e67a0-145">String</span><span class="sxs-lookup"><span data-stu-id="e67a0-145">String</span></span>|<span data-ttu-id="e67a0-p104">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="e67a0-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="e67a0-148">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="e67a0-148">uniqueSenders</span></span>|<span data-ttu-id="e67a0-149">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e67a0-149">String collection</span></span>|<span data-ttu-id="e67a0-150">Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="e67a0-150">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e67a0-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e67a0-151">Relationships</span></span>
| <span data-ttu-id="e67a0-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e67a0-152">Relationship</span></span> | <span data-ttu-id="e67a0-153">Typ</span><span class="sxs-lookup"><span data-stu-id="e67a0-153">Type</span></span>   |<span data-ttu-id="e67a0-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e67a0-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e67a0-155">Threads</span><span class="sxs-lookup"><span data-stu-id="e67a0-155">threads</span></span>|<span data-ttu-id="e67a0-156">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e67a0-156">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="e67a0-p105">Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e67a0-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e67a0-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e67a0-161">JSON representation</span></span>

<span data-ttu-id="e67a0-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e67a0-162">Here is a JSON representation of the resource</span></span>

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
