# <a name="conversation-resource-type"></a><span data-ttu-id="129f2-101">Ressourcentyp conversation</span><span class="sxs-lookup"><span data-stu-id="129f2-101">conversation resource type</span></span>

<span data-ttu-id="129f2-p101">Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.</span><span class="sxs-lookup"><span data-stu-id="129f2-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="129f2-104">Diese Ressource unterstützt Abonnieren von [Benachrichtigungen ändern](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="129f2-104">This resource supports subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="129f2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="129f2-105">Methods</span></span>

| <span data-ttu-id="129f2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="129f2-106">Method</span></span>       | <span data-ttu-id="129f2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="129f2-107">Return Type</span></span>  |<span data-ttu-id="129f2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="129f2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="129f2-109">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="129f2-109">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="129f2-110">[conversation](conversation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="129f2-110">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="129f2-111">Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="129f2-111">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="129f2-112">Erstellen</span><span class="sxs-lookup"><span data-stu-id="129f2-112">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="129f2-113">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="129f2-113">conversation</span></span>](conversation.md)| <span data-ttu-id="129f2-114">Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.</span><span class="sxs-lookup"><span data-stu-id="129f2-114">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="129f2-115">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="129f2-115">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="129f2-116">Unterhaltung</span><span class="sxs-lookup"><span data-stu-id="129f2-116">conversation</span></span>](conversation.md) |<span data-ttu-id="129f2-117">Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.</span><span class="sxs-lookup"><span data-stu-id="129f2-117">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="129f2-118">Löschen</span><span class="sxs-lookup"><span data-stu-id="129f2-118">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="129f2-119">Keine</span><span class="sxs-lookup"><span data-stu-id="129f2-119">None</span></span> |<span data-ttu-id="129f2-120">Unterhaltungsobjekt löschen.</span><span class="sxs-lookup"><span data-stu-id="129f2-120">Delete conversation object.</span></span> |
|[<span data-ttu-id="129f2-121">Unterhaltungsthreads auflisten</span><span class="sxs-lookup"><span data-stu-id="129f2-121">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="129f2-122">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="129f2-122">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="129f2-123">Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="129f2-123">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="129f2-124">Unterhaltungsthread erstellen</span><span class="sxs-lookup"><span data-stu-id="129f2-124">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="129f2-125">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="129f2-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="129f2-126">Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="129f2-126">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="129f2-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="129f2-127">Properties</span></span>
| <span data-ttu-id="129f2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="129f2-128">Property</span></span>     | <span data-ttu-id="129f2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="129f2-129">Type</span></span>   |<span data-ttu-id="129f2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="129f2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="129f2-131">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="129f2-131">hasAttachments</span></span>|<span data-ttu-id="129f2-132">boolesch</span><span class="sxs-lookup"><span data-stu-id="129f2-132">Boolean</span></span>|<span data-ttu-id="129f2-133">Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.</span><span class="sxs-lookup"><span data-stu-id="129f2-133">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="129f2-134">ID</span><span class="sxs-lookup"><span data-stu-id="129f2-134">id</span></span>|<span data-ttu-id="129f2-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="129f2-135">String</span></span>|<span data-ttu-id="129f2-p102">Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="129f2-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="129f2-138">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="129f2-138">lastDeliveredDateTime</span></span>|<span data-ttu-id="129f2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="129f2-139">DateTimeOffset</span></span>|<span data-ttu-id="129f2-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="129f2-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="129f2-142">Vorschau</span><span class="sxs-lookup"><span data-stu-id="129f2-142">preview</span></span>|<span data-ttu-id="129f2-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="129f2-143">String</span></span>|<span data-ttu-id="129f2-144">Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.</span><span class="sxs-lookup"><span data-stu-id="129f2-144">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="129f2-145">Thema</span><span class="sxs-lookup"><span data-stu-id="129f2-145">topic</span></span>|<span data-ttu-id="129f2-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="129f2-146">String</span></span>|<span data-ttu-id="129f2-p104">Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="129f2-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="129f2-149">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="129f2-149">uniqueSenders</span></span>|<span data-ttu-id="129f2-150">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="129f2-150">String collection</span></span>|<span data-ttu-id="129f2-151">Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="129f2-151">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="129f2-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="129f2-152">Relationships</span></span>
| <span data-ttu-id="129f2-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="129f2-153">Relationship</span></span> | <span data-ttu-id="129f2-154">Typ</span><span class="sxs-lookup"><span data-stu-id="129f2-154">Type</span></span>   |<span data-ttu-id="129f2-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="129f2-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="129f2-156">Threads</span><span class="sxs-lookup"><span data-stu-id="129f2-156">threads</span></span>|<span data-ttu-id="129f2-157">[conversationThread](conversationthread.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="129f2-157">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="129f2-p105">Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="129f2-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="129f2-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="129f2-162">JSON representation</span></span>

<span data-ttu-id="129f2-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="129f2-163">Here is a JSON representation of the resource</span></span>

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
