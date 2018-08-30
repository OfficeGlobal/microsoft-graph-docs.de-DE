# <a name="post-resource-type"></a><span data-ttu-id="933cc-101">Beitragsressourcentyp</span><span class="sxs-lookup"><span data-stu-id="933cc-101">post resource type</span></span>
<span data-ttu-id="933cc-102">Stellt ein einzelnes Post-Element in einer [conversationThread](conversationthread.md)-Entität dar.</span><span class="sxs-lookup"><span data-stu-id="933cc-102">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="933cc-103">Zwar können Sie Beiträge nicht explizit erstellen; es wird jedoch bei jedem der folgenden Vorgänge ein Beitrag erstellt:</span><span class="sxs-lookup"><span data-stu-id="933cc-103">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="933cc-104">auf einen vorhandenen Beitrag antworten</span><span class="sxs-lookup"><span data-stu-id="933cc-104">Reply to an existing post</span></span>](../api/post_reply.md) 
- [<span data-ttu-id="933cc-105">auf einen vorhandenen Thread antworten</span><span class="sxs-lookup"><span data-stu-id="933cc-105">Reply to an existing thread</span></span>](../api/conversationthread_reply.md) 
- [<span data-ttu-id="933cc-106">einen Thread in einer neuen Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="933cc-106">Create a thread in a new conversation</span></span>](../api/group_post_threads.md)
- [<span data-ttu-id="933cc-107">eine neue Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="933cc-107">Create a new conversation</span></span>](../api/group_post_conversations.md)

<span data-ttu-id="933cc-108">Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md) eigene Daten hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="933cc-108">This resource lets you add your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="933cc-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="933cc-109">Methods</span></span>

| <span data-ttu-id="933cc-110">Methode</span><span class="sxs-lookup"><span data-stu-id="933cc-110">Method</span></span>       | <span data-ttu-id="933cc-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="933cc-111">Return Type</span></span>  |<span data-ttu-id="933cc-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="933cc-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="933cc-113">Liste der Beiträge</span><span class="sxs-lookup"><span data-stu-id="933cc-113">List posts</span></span>](../api/conversationthread_list_posts.md) | [<span data-ttu-id="933cc-114">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-114">post</span></span>](post.md) |<span data-ttu-id="933cc-115">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="933cc-115">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="933cc-116">Beitrag anfordern</span><span class="sxs-lookup"><span data-stu-id="933cc-116">Get post</span></span>](../api/post_get.md) | [<span data-ttu-id="933cc-117">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-117">post</span></span>](post.md) |<span data-ttu-id="933cc-118">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread.</span><span class="sxs-lookup"><span data-stu-id="933cc-118">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="933cc-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="933cc-119">Reply</span></span>](../api/post_reply.md)|<span data-ttu-id="933cc-120">Keine</span><span class="sxs-lookup"><span data-stu-id="933cc-120">None</span></span>|<span data-ttu-id="933cc-121">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="933cc-121">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="933cc-122">Weiterleiten</span><span class="sxs-lookup"><span data-stu-id="933cc-122">Forward</span></span>](../api/post_forward.md)|<span data-ttu-id="933cc-123">Keine</span><span class="sxs-lookup"><span data-stu-id="933cc-123">None</span></span>|<span data-ttu-id="933cc-124">Dient zum Weiterleiten eines Beitrags an einen Empfänger.</span><span class="sxs-lookup"><span data-stu-id="933cc-124">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="933cc-125">**Anlagen**</span><span class="sxs-lookup"><span data-stu-id="933cc-125">**Attachments**</span></span>| | |
|[<span data-ttu-id="933cc-126">Liste der Anlagen</span><span class="sxs-lookup"><span data-stu-id="933cc-126">List attachments</span></span>](../api/post_list_attachments.md) |<span data-ttu-id="933cc-127">[Anlagen](attachment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="933cc-127">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="933cc-128">Ruft alle Anlagen für einen Beitrag ab.</span><span class="sxs-lookup"><span data-stu-id="933cc-128">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="933cc-129">Hinzufügen von Anlagen</span><span class="sxs-lookup"><span data-stu-id="933cc-129">Add attachment</span></span>](../api/post_post_attachments.md) |[<span data-ttu-id="933cc-130">Anlage</span><span class="sxs-lookup"><span data-stu-id="933cc-130">attachment</span></span>](attachment.md)| <span data-ttu-id="933cc-131">Dient zum Hinzufügen einer Anlage zu einem Beitrag.</span><span class="sxs-lookup"><span data-stu-id="933cc-131">Add an attachment to a post.</span></span> |
|<span data-ttu-id="933cc-132">**Offene Erweiterungen**</span><span class="sxs-lookup"><span data-stu-id="933cc-132">**Open extensions**</span></span>| | |
|[<span data-ttu-id="933cc-133">Offene Erweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="933cc-133">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="933cc-134">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="933cc-134">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="933cc-135">Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.</span><span class="sxs-lookup"><span data-stu-id="933cc-135">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="933cc-136">Offene Erweiterung abrufen</span><span class="sxs-lookup"><span data-stu-id="933cc-136">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="933cc-137">[openTypeExtension](opentypeextension.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="933cc-137">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="933cc-138">Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.</span><span class="sxs-lookup"><span data-stu-id="933cc-138">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="933cc-139">**Schemaerweiterungen**</span><span class="sxs-lookup"><span data-stu-id="933cc-139">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="933cc-140">Schemaerweiterungswerte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="933cc-140">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="933cc-141">Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="933cc-141">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="933cc-142">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="933cc-142">**Extended properties**</span></span>| | |
|[<span data-ttu-id="933cc-143">Einwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="933cc-143">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="933cc-144">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-144">post</span></span>](post.md)  |<span data-ttu-id="933cc-145">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag.</span><span class="sxs-lookup"><span data-stu-id="933cc-145">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="933cc-146">Beitrag mit erweiterter Eigenschaft zum Einzelwert anfordern</span><span class="sxs-lookup"><span data-stu-id="933cc-146">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="933cc-147">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-147">post</span></span>](post.md) | <span data-ttu-id="933cc-148">Dient zum Abrufen von Beiträgen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="933cc-148">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="933cc-149">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="933cc-149">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="933cc-150">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-150">post</span></span>](post.md) | <span data-ttu-id="933cc-151">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-151">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="933cc-152">Beiterag mit mehrwertiger erweiterter Eigenschaft anfordern</span><span class="sxs-lookup"><span data-stu-id="933cc-152">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="933cc-153">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-153">post</span></span>](post.md) | <span data-ttu-id="933cc-154">Dient zum Abrufen eines Beitrags mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="933cc-154">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="933cc-155">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="933cc-155">Properties</span></span>
| <span data-ttu-id="933cc-156">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="933cc-156">Property</span></span>     | <span data-ttu-id="933cc-157">Typ</span><span class="sxs-lookup"><span data-stu-id="933cc-157">Type</span></span>   |<span data-ttu-id="933cc-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="933cc-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="933cc-159">Text</span><span class="sxs-lookup"><span data-stu-id="933cc-159">body</span></span>|[<span data-ttu-id="933cc-160">itemBody</span><span class="sxs-lookup"><span data-stu-id="933cc-160">itemBody</span></span>](itembody.md)|<span data-ttu-id="933cc-p101">Der Inhalt des Beitrags. Dies ist eine Standardeigenschaft. Für diese Eigenschaft sind Nullwerte zulässig.</span><span class="sxs-lookup"><span data-stu-id="933cc-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="933cc-164">Kategorien</span><span class="sxs-lookup"><span data-stu-id="933cc-164">categories</span></span>|<span data-ttu-id="933cc-165">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="933cc-165">String collection</span></span>|<span data-ttu-id="933cc-166">Die Kategorien, die mit dem Beitrag verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="933cc-166">The categories associated with the post.</span></span>|
|<span data-ttu-id="933cc-167">changeKey</span><span class="sxs-lookup"><span data-stu-id="933cc-167">changeKey</span></span>|<span data-ttu-id="933cc-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="933cc-168">String</span></span>|<span data-ttu-id="933cc-p102">Gibt die Version des Beitrags an. Jedes Mal, wenn der Beitrag geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="933cc-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="933cc-172">conversationId</span><span class="sxs-lookup"><span data-stu-id="933cc-172">conversationId</span></span>|<span data-ttu-id="933cc-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="933cc-173">String</span></span>|<span data-ttu-id="933cc-p103">Eindeutige ID der Unterhaltung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="933cc-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="933cc-176">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="933cc-176">conversationThreadId</span></span>|<span data-ttu-id="933cc-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="933cc-177">String</span></span>|<span data-ttu-id="933cc-p104">Eindeutige ID des Unterhaltungsthreads. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="933cc-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="933cc-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="933cc-180">createdDateTime</span></span>|<span data-ttu-id="933cc-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="933cc-181">DateTimeOffset</span></span>|<span data-ttu-id="933cc-p105">Gibt an, wann der Beitrag erstellt wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="933cc-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="933cc-185">Von</span><span class="sxs-lookup"><span data-stu-id="933cc-185">from</span></span>|[<span data-ttu-id="933cc-186">Empfänger</span><span class="sxs-lookup"><span data-stu-id="933cc-186">recipient</span></span>](recipient.md)|<span data-ttu-id="933cc-p106">Wird in Zugriffsszenarien mit Stellvertretungen verwendet. Gibt an, wer die Nachricht im Auftrag eines anderen Benutzers veröffentlicht hat. Dies ist eine Standardeigenschaft.</span><span class="sxs-lookup"><span data-stu-id="933cc-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="933cc-190">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="933cc-190">hasAttachments</span></span>|<span data-ttu-id="933cc-191">boolesch</span><span class="sxs-lookup"><span data-stu-id="933cc-191">Boolean</span></span>|<span data-ttu-id="933cc-p107">Gibt an, ob der Beitrag mindestens eine Anlage enthält. Dies ist eine Standardeigenschaft.</span><span class="sxs-lookup"><span data-stu-id="933cc-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="933cc-194">ID</span><span class="sxs-lookup"><span data-stu-id="933cc-194">id</span></span>|<span data-ttu-id="933cc-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="933cc-195">String</span></span>| <span data-ttu-id="933cc-196">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="933cc-196">Read-only.</span></span>|
|<span data-ttu-id="933cc-197">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="933cc-197">lastModifiedDateTime</span></span>|<span data-ttu-id="933cc-198">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="933cc-198">DateTimeOffset</span></span>|<span data-ttu-id="933cc-p108">Gibt an, wann der Beitrag zuletzt geändert wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="933cc-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="933cc-202">newParticipants</span><span class="sxs-lookup"><span data-stu-id="933cc-202">newParticipants</span></span>|<span data-ttu-id="933cc-203">[Empfänger](recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="933cc-203">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="933cc-204">Teilnehmer einer Unterhaltung, die im Rahmen des Beitrags zu dem Thread hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="933cc-204">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="933cc-205">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="933cc-205">receivedDateTime</span></span>|<span data-ttu-id="933cc-206">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="933cc-206">DateTimeOffset</span></span>|<span data-ttu-id="933cc-p109">Gibt an, wann der Beitrag empfangen wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="933cc-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="933cc-210">Sender</span><span class="sxs-lookup"><span data-stu-id="933cc-210">sender</span></span>|[<span data-ttu-id="933cc-211">Empfänger</span><span class="sxs-lookup"><span data-stu-id="933cc-211">recipient</span></span>](recipient.md)|<span data-ttu-id="933cc-p110">Enthält die E-Mail-Adresse des Absenders. Bei dem Sender-Wert wird davon ausgegangen, dass dies die Adresse des authentifizierten Benutzers ist, wenn Absender nicht angegeben wurde. Dies ist eine Standardeigenschaft.</span><span class="sxs-lookup"><span data-stu-id="933cc-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="933cc-215">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="933cc-215">Relationships</span></span>
| <span data-ttu-id="933cc-216">Beziehung</span><span class="sxs-lookup"><span data-stu-id="933cc-216">Relationship</span></span> | <span data-ttu-id="933cc-217">Typ</span><span class="sxs-lookup"><span data-stu-id="933cc-217">Type</span></span>   |<span data-ttu-id="933cc-218">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="933cc-218">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="933cc-219">Anlagen</span><span class="sxs-lookup"><span data-stu-id="933cc-219">attachments</span></span>|<span data-ttu-id="933cc-220">[Anlagensammlung](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="933cc-220">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="933cc-p111">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="933cc-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="933cc-223">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="933cc-223">extensions</span></span>|<span data-ttu-id="933cc-224">[Erweiterungssammlung](extension.md)</span><span class="sxs-lookup"><span data-stu-id="933cc-224">[Extension](extension.md) collection</span></span>|<span data-ttu-id="933cc-p112">Die Sammlung der für den Beitrag definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="933cc-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="933cc-228">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="933cc-228">inReplyTo</span></span>|[<span data-ttu-id="933cc-229">Beitrag</span><span class="sxs-lookup"><span data-stu-id="933cc-229">post</span></span>](post.md)| <span data-ttu-id="933cc-230">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="933cc-230">Read-only.</span></span>|
|<span data-ttu-id="933cc-231">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="933cc-231">multiValueExtendedProperties</span></span>|<span data-ttu-id="933cc-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="933cc-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="933cc-p113">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="933cc-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="933cc-236">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="933cc-236">singleValueExtendedProperties</span></span>|<span data-ttu-id="933cc-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="933cc-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="933cc-p114">Die Sammlung erweiterter einwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="933cc-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="933cc-241">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="933cc-241">JSON representation</span></span>

<span data-ttu-id="933cc-242">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="933cc-242">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a><span data-ttu-id="933cc-243">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="933cc-243">See also</span></span>

- [<span data-ttu-id="933cc-244">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="933cc-244">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="933cc-245">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="933cc-245">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="933cc-246">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="933cc-246">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
