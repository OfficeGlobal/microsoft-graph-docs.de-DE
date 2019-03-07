---
title: chatMessage-Ressourcentyp
description: Stellt eine einzelne Chatnachricht innerhalb eines Kanals oder einer Chatentität dar. Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458659"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="1a848-104">chatMessage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1a848-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a848-105">Stellt eine einzelne Chatnachricht innerhalb eines [Kanals](channel.md) oder einer Chatentität dar.</span><span class="sxs-lookup"><span data-stu-id="1a848-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="1a848-106">Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.</span><span class="sxs-lookup"><span data-stu-id="1a848-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="1a848-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="1a848-107">Methods</span></span>

| <span data-ttu-id="1a848-108">Methode</span><span class="sxs-lookup"><span data-stu-id="1a848-108">Method</span></span>       | <span data-ttu-id="1a848-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1a848-109">Return Type</span></span>  |<span data-ttu-id="1a848-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a848-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a848-111">Kanalnachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="1a848-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="1a848-112">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1a848-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="1a848-113">Abrufen der Liste aller Stammnachrichten in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="1a848-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="1a848-114">Kanalnachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="1a848-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="1a848-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1a848-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="1a848-116">Abrufen einer einzelnen Stammnachricht aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="1a848-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="1a848-117">Antworten in einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="1a848-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="1a848-118">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1a848-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="1a848-119">Abrufen der Liste aller Antworten auf eine Nachricht im Kanal.</span><span class="sxs-lookup"><span data-stu-id="1a848-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="1a848-120">Antwort auf eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="1a848-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="1a848-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1a848-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1a848-122">Abrufen einer einzelnen Antwort auf eine Nachricht in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="1a848-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="1a848-123">Senden einer Nachricht in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="1a848-123">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="1a848-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1a848-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1a848-125">Erstellen Sie eine neue Nachricht auf oberster Ebene in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="1a848-125">Create a new message in a channel.</span></span>|
|[<span data-ttu-id="1a848-126">Antworten auf eine Nachricht in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="1a848-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="1a848-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1a848-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1a848-128">Antworten Sie auf eine Nachricht in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="1a848-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="1a848-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1a848-129">Properties</span></span>
| <span data-ttu-id="1a848-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a848-130">Property</span></span>     | <span data-ttu-id="1a848-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1a848-131">Type</span></span>   |<span data-ttu-id="1a848-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a848-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a848-133">id</span><span class="sxs-lookup"><span data-stu-id="1a848-133">id</span></span>|<span data-ttu-id="1a848-134">String</span><span class="sxs-lookup"><span data-stu-id="1a848-134">String</span></span>| <span data-ttu-id="1a848-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1a848-135">Read-only.</span></span> <span data-ttu-id="1a848-136">Eindeutige ID der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="1a848-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="1a848-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="1a848-137">replyToId</span></span>| <span data-ttu-id="1a848-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-138">string</span></span> | <span data-ttu-id="1a848-139">ID der übergeordneten Nachricht/Stammnachricht des Threads</span><span class="sxs-lookup"><span data-stu-id="1a848-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="1a848-140">von</span><span class="sxs-lookup"><span data-stu-id="1a848-140">from</span></span>|[<span data-ttu-id="1a848-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a848-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="1a848-142">Einzelheiten über den Absender der Nachricht</span><span class="sxs-lookup"><span data-stu-id="1a848-142">Details of the sender of the message</span></span>|
|<span data-ttu-id="1a848-143">etag</span><span class="sxs-lookup"><span data-stu-id="1a848-143">etag</span></span>| <span data-ttu-id="1a848-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-144">string</span></span> | <span data-ttu-id="1a848-145">Versionsnummer der Nachricht</span><span class="sxs-lookup"><span data-stu-id="1a848-145">Version number of the message</span></span> |
|<span data-ttu-id="1a848-146">messageType</span><span class="sxs-lookup"><span data-stu-id="1a848-146">messageType</span></span>|<span data-ttu-id="1a848-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-147">String</span></span>|<span data-ttu-id="1a848-148">Der Typ der Nachricht; aktuell unterstützte Werte sind: message, chatEvent, Typing</span><span class="sxs-lookup"><span data-stu-id="1a848-148">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="1a848-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a848-149">createdDateTime</span></span>|<span data-ttu-id="1a848-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a848-150">dateTimeOffset</span></span>|<span data-ttu-id="1a848-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1a848-151">Read only.</span></span> <span data-ttu-id="1a848-152">Zeitstempel, wann die Nachricht erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="1a848-152">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="1a848-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a848-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1a848-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a848-154">dateTimeOffset</span></span>|<span data-ttu-id="1a848-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1a848-155">Read only.</span></span> <span data-ttu-id="1a848-156">Zeitstempel, wann die Nachricht bearbeitet/aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="1a848-156">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="1a848-157">deleted</span><span class="sxs-lookup"><span data-stu-id="1a848-157">deleted</span></span>|<span data-ttu-id="1a848-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a848-158">Boolean</span></span>|<span data-ttu-id="1a848-159">Gibt an, ob eine Nachricht vorläufig gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="1a848-159">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="1a848-160">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a848-160">deletedDateTime</span></span>|<span data-ttu-id="1a848-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a848-161">dateTimeOffset</span></span>|<span data-ttu-id="1a848-162">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1a848-162">Read only.</span></span> <span data-ttu-id="1a848-163">Zeitstempel, wann die Nachricht gelöscht wurde</span><span class="sxs-lookup"><span data-stu-id="1a848-163">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="1a848-164">subject</span><span class="sxs-lookup"><span data-stu-id="1a848-164">subject</span></span>|<span data-ttu-id="1a848-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-165">string</span></span>|<span data-ttu-id="1a848-166">Nachrichtenbetreff</span><span class="sxs-lookup"><span data-stu-id="1a848-166">Message subject line.</span></span> <span data-ttu-id="1a848-167">Optional</span><span class="sxs-lookup"><span data-stu-id="1a848-167">Optional</span></span>|
|<span data-ttu-id="1a848-168">Text</span><span class="sxs-lookup"><span data-stu-id="1a848-168">body</span></span>|[<span data-ttu-id="1a848-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="1a848-169">itemBody</span></span>](itembody.md)|<span data-ttu-id="1a848-170">Nur-Text-/HTML-Darstellung des Inhalts der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="1a848-170">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="1a848-171">Gibt standardmäßig Nur-Text wieder; Anwendung kann HTML wahlweise als Teil eines Abfrageparameters auswählen</span><span class="sxs-lookup"><span data-stu-id="1a848-171">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="1a848-172">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="1a848-172">summary</span></span>|<span data-ttu-id="1a848-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-173">string</span></span>|<span data-ttu-id="1a848-174">Zusammenfassungstext der Nachricht, die für Pushbenachrichtigungen und Zusammenfassungs- oder Fallbackansichten verwendet werden kann </span><span class="sxs-lookup"><span data-stu-id="1a848-174">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="1a848-175">Erwähnungen</span><span class="sxs-lookup"><span data-stu-id="1a848-175">mentions</span></span>|<span data-ttu-id="1a848-176">[chatMessageMention](chatmention.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1a848-176">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="1a848-177">Liste der Entitäten, die in der Nachricht angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="1a848-177">List of entities mentioned in the message.</span></span> <span data-ttu-id="1a848-178">Derzeit unterstützt: user, bot, team, channel</span><span class="sxs-lookup"><span data-stu-id="1a848-178">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="1a848-179">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="1a848-179">importance</span></span>| <span data-ttu-id="1a848-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-180">string</span></span> | <span data-ttu-id="1a848-181">Legt die Wichtigkeit der Nachricht fest: Hoch, Niedrig</span><span class="sxs-lookup"><span data-stu-id="1a848-181">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="1a848-182">Reaktionen</span><span class="sxs-lookup"><span data-stu-id="1a848-182">reactions</span></span>| <span data-ttu-id="1a848-183">[chatMessageReaction](chatreaction.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1a848-183">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="1a848-184">Reaktionen auf diese Nachricht (z. B. Gefällt mir)</span><span class="sxs-lookup"><span data-stu-id="1a848-184">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="1a848-185">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="1a848-185">locale</span></span>|<span data-ttu-id="1a848-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a848-186">string</span></span>|<span data-ttu-id="1a848-187">Vom Client festgelegtes Gebietsschema der Nachricht</span><span class="sxs-lookup"><span data-stu-id="1a848-187">Locale of the message set by the client</span></span>|
|<span data-ttu-id="1a848-188">Anlagen</span><span class="sxs-lookup"><span data-stu-id="1a848-188">attachments</span></span>|<span data-ttu-id="1a848-189">[chatMessageAttachment](chatattachment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1a848-189">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="1a848-190">Angefügte Dateien</span><span class="sxs-lookup"><span data-stu-id="1a848-190">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1a848-191">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1a848-191">JSON representation</span></span>

<span data-ttu-id="1a848-192">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1a848-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
