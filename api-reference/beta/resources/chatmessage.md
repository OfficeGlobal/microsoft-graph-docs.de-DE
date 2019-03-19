---
title: chatMessage-Ressourcentyp
description: Stellt eine einzelne Chatnachricht innerhalb eines Kanals oder einer Chatentität dar. Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.
localization_priority: Priority
ms.openlocfilehash: a74f422c6bf60e1293d8620b440152be77dacdc7
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644321"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="4c973-104">chatMessage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4c973-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c973-105">Stellt eine einzelne Chatnachricht innerhalb eines [Kanals](channel.md) oder einer Chatentität dar.</span><span class="sxs-lookup"><span data-stu-id="4c973-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="4c973-106">Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.</span><span class="sxs-lookup"><span data-stu-id="4c973-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="4c973-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="4c973-107">Methods</span></span>

| <span data-ttu-id="4c973-108">Methode</span><span class="sxs-lookup"><span data-stu-id="4c973-108">Method</span></span>       | <span data-ttu-id="4c973-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4c973-109">Return Type</span></span>  |<span data-ttu-id="4c973-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c973-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c973-111">Kanalnachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="4c973-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="4c973-112">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4c973-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="4c973-113">Abrufen der Liste aller Stammnachrichten in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="4c973-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="4c973-114">Kanalnachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="4c973-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="4c973-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="4c973-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="4c973-116">Abrufen einer einzelnen Stammnachricht aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="4c973-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="4c973-117">Antworten in einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="4c973-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="4c973-118">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4c973-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="4c973-119">Abrufen der Liste aller Antworten auf eine Nachricht im Kanal.</span><span class="sxs-lookup"><span data-stu-id="4c973-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="4c973-120">Antwort auf eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="4c973-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="4c973-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="4c973-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="4c973-122">Abrufen einer einzelnen Antwort auf eine Nachricht in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="4c973-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="4c973-123">Senden einer Nachricht in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="4c973-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="4c973-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="4c973-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="4c973-125">Erstellen Sie eine neue Nachricht auf oberster Ebene in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="4c973-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="4c973-126">Antworten auf eine Nachricht in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="4c973-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="4c973-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="4c973-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="4c973-128">Antworten Sie auf eine Nachricht in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="4c973-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="4c973-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4c973-129">Properties</span></span>
| <span data-ttu-id="4c973-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c973-130">Property</span></span>     | <span data-ttu-id="4c973-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4c973-131">Type</span></span>   |<span data-ttu-id="4c973-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c973-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c973-133">id</span><span class="sxs-lookup"><span data-stu-id="4c973-133">id</span></span>|<span data-ttu-id="4c973-134">String</span><span class="sxs-lookup"><span data-stu-id="4c973-134">String</span></span>| <span data-ttu-id="4c973-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4c973-135">Read-only.</span></span> <span data-ttu-id="4c973-136">Eindeutige ID der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4c973-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="4c973-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="4c973-137">replyToId</span></span>| <span data-ttu-id="4c973-138">string</span><span class="sxs-lookup"><span data-stu-id="4c973-138">string</span></span> | <span data-ttu-id="4c973-139">ID der übergeordneten Nachricht/Stammnachricht des Threads.</span><span class="sxs-lookup"><span data-stu-id="4c973-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="4c973-140">von</span><span class="sxs-lookup"><span data-stu-id="4c973-140">from</span></span>|[<span data-ttu-id="4c973-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="4c973-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="4c973-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4c973-142">Read only.</span></span> <span data-ttu-id="4c973-143">Einzelheiten über den Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4c973-143">Details of the sender of the message</span></span>|
|<span data-ttu-id="4c973-144">etag</span><span class="sxs-lookup"><span data-stu-id="4c973-144">etag</span></span>| <span data-ttu-id="4c973-145">string</span><span class="sxs-lookup"><span data-stu-id="4c973-145">string</span></span> | <span data-ttu-id="4c973-146">Versionsnummer der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4c973-146">Version number of the message</span></span> |
|<span data-ttu-id="4c973-147">messageType</span><span class="sxs-lookup"><span data-stu-id="4c973-147">messageType</span></span>|<span data-ttu-id="4c973-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c973-148">String</span></span>|<span data-ttu-id="4c973-149">Der Typ der Nachricht; aktuell unterstützte Werte sind: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="4c973-149">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="4c973-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c973-150">createdDateTime</span></span>|<span data-ttu-id="4c973-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c973-151">dateTimeOffset</span></span>|<span data-ttu-id="4c973-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4c973-152">Read only.</span></span> <span data-ttu-id="4c973-153">Zeitstempel, wann die Nachricht erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4c973-153">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="4c973-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c973-154">lastModifiedDateTime</span></span>|<span data-ttu-id="4c973-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c973-155">dateTimeOffset</span></span>|<span data-ttu-id="4c973-156">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4c973-156">Read only.</span></span> <span data-ttu-id="4c973-157">Zeitstempel, wann die Nachricht bearbeitet/aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="4c973-157">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="4c973-158">deleted</span><span class="sxs-lookup"><span data-stu-id="4c973-158">deleted</span></span>|<span data-ttu-id="4c973-159">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4c973-159">Boolean</span></span>|<span data-ttu-id="4c973-160">Gibt an, ob eine Nachricht vorläufig gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="4c973-160">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="4c973-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c973-161">deletedDateTime</span></span>|<span data-ttu-id="4c973-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c973-162">dateTimeOffset</span></span>|<span data-ttu-id="4c973-163">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4c973-163">Read only.</span></span> <span data-ttu-id="4c973-164">Zeitstempel, wann die Nachricht gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="4c973-164">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="4c973-165">subject</span><span class="sxs-lookup"><span data-stu-id="4c973-165">subject</span></span>|<span data-ttu-id="4c973-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c973-166">string</span></span>|<span data-ttu-id="4c973-167">Nachrichtenbetreff</span><span class="sxs-lookup"><span data-stu-id="4c973-167">Message subject line.</span></span> <span data-ttu-id="4c973-168">Optional.</span><span class="sxs-lookup"><span data-stu-id="4c973-168">Optional.</span></span>|
|<span data-ttu-id="4c973-169">Text</span><span class="sxs-lookup"><span data-stu-id="4c973-169">body</span></span>|[<span data-ttu-id="4c973-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="4c973-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="4c973-171">Nur-Text-/HTML-Darstellung des Inhalts der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4c973-171">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="4c973-172">Gibt standardmäßig Nur-Text wieder; Anwendung kann HTML wahlweise als Teil eines Abfrageparameters auswählen</span><span class="sxs-lookup"><span data-stu-id="4c973-172">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="4c973-173">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="4c973-173">summary</span></span>|<span data-ttu-id="4c973-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c973-174">string</span></span>|<span data-ttu-id="4c973-175">Zusammenfassungstext der Nachricht, die für Pushbenachrichtigungen und Zusammenfassungs- oder Fallbackansichten verwendet werden kann </span><span class="sxs-lookup"><span data-stu-id="4c973-175">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="4c973-176">Erwähnungen</span><span class="sxs-lookup"><span data-stu-id="4c973-176">mentions</span></span>|<span data-ttu-id="4c973-177">[chatMessageMention](chatmention.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4c973-177">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="4c973-178">Liste der Entitäten, die in der Nachricht angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="4c973-178">List of entities mentioned in the message.</span></span> <span data-ttu-id="4c973-179">Derzeit unterstützt: user, bot, team, channel.</span><span class="sxs-lookup"><span data-stu-id="4c973-179">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="4c973-180">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="4c973-180">importance</span></span>| <span data-ttu-id="4c973-181">string</span><span class="sxs-lookup"><span data-stu-id="4c973-181">string</span></span> | <span data-ttu-id="4c973-182">Legt die Wichtigkeit der Nachricht fest: Hoch, Niedrig.</span><span class="sxs-lookup"><span data-stu-id="4c973-182">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="4c973-183">Reaktionen</span><span class="sxs-lookup"><span data-stu-id="4c973-183">reactions</span></span>| <span data-ttu-id="4c973-184">[chatMessageReaction](chatreaction.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4c973-184">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="4c973-185">Reaktionen auf diese Nachricht (z. B. Gefällt mir)</span><span class="sxs-lookup"><span data-stu-id="4c973-185">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="4c973-186">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="4c973-186">locale</span></span>|<span data-ttu-id="4c973-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c973-187">string</span></span>|<span data-ttu-id="4c973-188">Vom Client festgelegtes Gebietsschema der Nachricht</span><span class="sxs-lookup"><span data-stu-id="4c973-188">Locale of the message set by the client</span></span>|
|<span data-ttu-id="4c973-189">Anlagen</span><span class="sxs-lookup"><span data-stu-id="4c973-189">attachments</span></span>|<span data-ttu-id="4c973-190">[chatMessageAttachment](chatattachment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4c973-190">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="4c973-191">Angefügte Dateien.</span><span class="sxs-lookup"><span data-stu-id="4c973-191">Attached files</span></span> <span data-ttu-id="4c973-192">Anlagen sind derzeit schreibgeschützt – das Senden von Anlagen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c973-192">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4c973-193">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4c973-193">JSON representation</span></span>

<span data-ttu-id="4c973-194">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4c973-194">The following is a JSON representation of the resource.</span></span>

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
