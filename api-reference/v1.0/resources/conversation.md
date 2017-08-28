# <a name="conversation-resource-type"></a><span data-ttu-id="5e1df-101">Ressourcentyp conversation</span><span class="sxs-lookup"><span data-stu-id="5e1df-101">conversation resource type</span></span>

<span data-ttu-id="5e1df-p101">Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.</span><span class="sxs-lookup"><span data-stu-id="5e1df-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

## <a name="methods"></a><span data-ttu-id="5e1df-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="5e1df-104">Methods</span></span>

| <span data-ttu-id="5e1df-105">Methode</span><span class="sxs-lookup"><span data-stu-id="5e1df-105">Method</span></span>       | <span data-ttu-id="5e1df-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5e1df-106">Return Type</span></span>  |<span data-ttu-id="5e1df-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e1df-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e1df-108">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="5e1df-108">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="5e1df-109">[conversation](conversation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e1df-109">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="5e1df-110">Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="5e1df-110">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="5e1df-111">Erstellen</span><span class="sxs-lookup"><span data-stu-id="5e1df-111">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="5e1df-112">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="5e1df-112">conversation</span></span>](conversation.md)| <span data-ttu-id="5e1df-113">Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="5e1df-113">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="5e1df-114">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="5e1df-114">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="5e1df-115">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="5e1df-115">conversation</span></span>](conversation.md) |<span data-ttu-id="5e1df-116">Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="5e1df-116">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="5e1df-117">Löschen</span><span class="sxs-lookup"><span data-stu-id="5e1df-117">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="5e1df-118">Keine</span><span class="sxs-lookup"><span data-stu-id="5e1df-118">None</span></span> |<span data-ttu-id="5e1df-119">Unterhaltungsobjekt löschen.</span><span class="sxs-lookup"><span data-stu-id="5e1df-119">Delete conversation object.</span></span> |
|[<span data-ttu-id="5e1df-120">Unterhaltungsthreads auflisten</span><span class="sxs-lookup"><span data-stu-id="5e1df-120">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="5e1df-121">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e1df-121">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="5e1df-122">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="5e1df-122">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="5e1df-123">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="5e1df-123">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="5e1df-124">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e1df-124">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="5e1df-125">Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="5e1df-125">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e1df-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5e1df-126">Properties</span></span>
| <span data-ttu-id="5e1df-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e1df-127">Property</span></span>     | <span data-ttu-id="5e1df-128">Typ</span><span class="sxs-lookup"><span data-stu-id="5e1df-128">Type</span></span>   |<span data-ttu-id="5e1df-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e1df-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1df-130">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="5e1df-130">hasAttachments</span></span>|<span data-ttu-id="5e1df-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e1df-131">Boolean</span></span>|<span data-ttu-id="5e1df-132">Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="5e1df-132">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="5e1df-133">id</span><span class="sxs-lookup"><span data-stu-id="5e1df-133">id</span></span>|<span data-ttu-id="5e1df-134">String</span><span class="sxs-lookup"><span data-stu-id="5e1df-134">String</span></span>|<span data-ttu-id="5e1df-p102">Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5e1df-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="5e1df-137">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="5e1df-137">lastDeliveredDateTime</span></span>|<span data-ttu-id="5e1df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e1df-138">DateTimeOffset</span></span>|<span data-ttu-id="5e1df-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5e1df-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5e1df-141">Vorschau</span><span class="sxs-lookup"><span data-stu-id="5e1df-141">preview</span></span>|<span data-ttu-id="5e1df-142">String</span><span class="sxs-lookup"><span data-stu-id="5e1df-142">String</span></span>|<span data-ttu-id="5e1df-143">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="5e1df-143">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="5e1df-144">Thema</span><span class="sxs-lookup"><span data-stu-id="5e1df-144">topic</span></span>|<span data-ttu-id="5e1df-145">String</span><span class="sxs-lookup"><span data-stu-id="5e1df-145">String</span></span>|<span data-ttu-id="5e1df-p104">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="5e1df-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="5e1df-148">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="5e1df-148">uniqueSenders</span></span>|<span data-ttu-id="5e1df-149">String collection</span><span class="sxs-lookup"><span data-stu-id="5e1df-149">String collection</span></span>|<span data-ttu-id="5e1df-150">Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="5e1df-150">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e1df-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5e1df-151">Relationships</span></span>
| <span data-ttu-id="5e1df-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5e1df-152">Relationship</span></span> | <span data-ttu-id="5e1df-153">Typ</span><span class="sxs-lookup"><span data-stu-id="5e1df-153">Type</span></span>   |<span data-ttu-id="5e1df-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e1df-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1df-155">Threads</span><span class="sxs-lookup"><span data-stu-id="5e1df-155">threads</span></span>|<span data-ttu-id="5e1df-156">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e1df-156">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="5e1df-p105">Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5e1df-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e1df-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5e1df-161">JSON representation</span></span>

<span data-ttu-id="5e1df-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5e1df-162">Here is a JSON representation of the resource</span></span>

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
