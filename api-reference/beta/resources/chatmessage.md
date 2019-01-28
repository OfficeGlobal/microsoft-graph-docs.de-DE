---
title: chatMessage-Ressourcentyp
description: Stellt eine einzelne Chatnachricht innerhalb eines Kanals oder einer Chatentität dar. Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.
localization_priority: Priority
ms.openlocfilehash: 98b9918d5763d6003a3c9a177057abe2e7b415ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517967"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="bacb5-104">chatMessage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bacb5-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bacb5-105">Stellt eine einzelne Chatnachricht innerhalb eines [Kanals](channel.md) oder einer Chatentität dar.</span><span class="sxs-lookup"><span data-stu-id="bacb5-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="bacb5-106">Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.</span><span class="sxs-lookup"><span data-stu-id="bacb5-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="bacb5-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="bacb5-107">Methods</span></span>

| <span data-ttu-id="bacb5-108">Methode</span><span class="sxs-lookup"><span data-stu-id="bacb5-108">Method</span></span>       | <span data-ttu-id="bacb5-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bacb5-109">Return Type</span></span>  |<span data-ttu-id="bacb5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bacb5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bacb5-111">Kanalnachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="bacb5-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="bacb5-112">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bacb5-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="bacb5-113">Abrufen der Liste aller Stammnachrichten in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="bacb5-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="bacb5-114">Kanalnachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="bacb5-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="bacb5-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="bacb5-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="bacb5-116">Abrufen einer einzelnen Stammnachricht aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="bacb5-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="bacb5-117">Antworten in einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="bacb5-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="bacb5-118">[chatMessage](chatmessage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bacb5-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="bacb5-119">Abrufen der Liste aller Antworten auf eine Nachricht im Kanal.</span><span class="sxs-lookup"><span data-stu-id="bacb5-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="bacb5-120">Antwort auf eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="bacb5-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="bacb5-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="bacb5-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="bacb5-122">Abrufen einer einzelnen Antwort auf eine Nachricht in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="bacb5-122">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="bacb5-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bacb5-123">Properties</span></span>
| <span data-ttu-id="bacb5-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bacb5-124">Property</span></span>     | <span data-ttu-id="bacb5-125">Typ</span><span class="sxs-lookup"><span data-stu-id="bacb5-125">Type</span></span>   |<span data-ttu-id="bacb5-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bacb5-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bacb5-127">id</span><span class="sxs-lookup"><span data-stu-id="bacb5-127">id</span></span>|<span data-ttu-id="bacb5-128">String</span><span class="sxs-lookup"><span data-stu-id="bacb5-128">String</span></span>| <span data-ttu-id="bacb5-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bacb5-129">Read-only.</span></span> <span data-ttu-id="bacb5-130">Eindeutige ID der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="bacb5-130">Unique ID of the message.</span></span>|
|<span data-ttu-id="bacb5-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="bacb5-131">replyToId</span></span>| <span data-ttu-id="bacb5-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-132">string</span></span> | <span data-ttu-id="bacb5-133">ID der übergeordneten Nachricht/Stammnachricht des Threads</span><span class="sxs-lookup"><span data-stu-id="bacb5-133">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="bacb5-134">von</span><span class="sxs-lookup"><span data-stu-id="bacb5-134">from</span></span>|[<span data-ttu-id="bacb5-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="bacb5-135">identitySet</span></span>](identityset.md)| <span data-ttu-id="bacb5-136">Einzelheiten über den Absender der Nachricht</span><span class="sxs-lookup"><span data-stu-id="bacb5-136">Details of the sender of the message</span></span>|
|<span data-ttu-id="bacb5-137">etag</span><span class="sxs-lookup"><span data-stu-id="bacb5-137">etag</span></span>| <span data-ttu-id="bacb5-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-138">string</span></span> | <span data-ttu-id="bacb5-139">Versionsnummer der Nachricht</span><span class="sxs-lookup"><span data-stu-id="bacb5-139">Version number of the message</span></span> |
|<span data-ttu-id="bacb5-140">messageType</span><span class="sxs-lookup"><span data-stu-id="bacb5-140">messageType</span></span>|<span data-ttu-id="bacb5-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-141">String</span></span>|<span data-ttu-id="bacb5-142">Der Typ der Nachricht; aktuell unterstützte Werte sind: message, chatEvent, Typing</span><span class="sxs-lookup"><span data-stu-id="bacb5-142">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="bacb5-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bacb5-143">createdDateTime</span></span>|<span data-ttu-id="bacb5-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacb5-144">dateTimeOffset</span></span>|<span data-ttu-id="bacb5-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bacb5-145">Read only.</span></span> <span data-ttu-id="bacb5-146">Zeitstempel, wann die Nachricht erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="bacb5-146">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="bacb5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bacb5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="bacb5-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacb5-148">dateTimeOffset</span></span>|<span data-ttu-id="bacb5-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bacb5-149">Read only.</span></span> <span data-ttu-id="bacb5-150">Zeitstempel, wann die Nachricht bearbeitet/aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="bacb5-150">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="bacb5-151">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bacb5-151">isDeleted</span></span>|<span data-ttu-id="bacb5-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bacb5-152">boolean</span></span>|<span data-ttu-id="bacb5-153">Gibt an, ob eine Nachricht vorläufig gelöscht wurde</span><span class="sxs-lookup"><span data-stu-id="bacb5-153">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="bacb5-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="bacb5-154">deletedDateTime</span></span>|<span data-ttu-id="bacb5-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacb5-155">dateTimeOffset</span></span>|<span data-ttu-id="bacb5-156">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bacb5-156">Read only.</span></span> <span data-ttu-id="bacb5-157">Zeitstempel, wann die Nachricht gelöscht wurde</span><span class="sxs-lookup"><span data-stu-id="bacb5-157">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="bacb5-158">subject</span><span class="sxs-lookup"><span data-stu-id="bacb5-158">subject</span></span>|<span data-ttu-id="bacb5-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-159">string</span></span>|<span data-ttu-id="bacb5-160">Nachrichtenbetreff</span><span class="sxs-lookup"><span data-stu-id="bacb5-160">Message subject line.</span></span> <span data-ttu-id="bacb5-161">Optional</span><span class="sxs-lookup"><span data-stu-id="bacb5-161">Optional</span></span>|
|<span data-ttu-id="bacb5-162">Text</span><span class="sxs-lookup"><span data-stu-id="bacb5-162">body</span></span>|[<span data-ttu-id="bacb5-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="bacb5-163">itemBody</span></span>](itembody.md)|<span data-ttu-id="bacb5-164">Nur-Text-/HTML-Darstellung des Inhalts der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="bacb5-164">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="bacb5-165">Gibt standardmäßig Nur-Text wieder; Anwendung kann HTML wahlweise als Teil eines Abfrageparameters auswählen</span><span class="sxs-lookup"><span data-stu-id="bacb5-165">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="bacb5-166">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="bacb5-166">summary</span></span>|<span data-ttu-id="bacb5-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-167">string</span></span>|<span data-ttu-id="bacb5-168">Zusammenfassungstext der Nachricht, die für Pushbenachrichtigungen und Zusammenfassungs- oder Fallbackansichten verwendet werden kann </span><span class="sxs-lookup"><span data-stu-id="bacb5-168">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="bacb5-169">Erwähnungen</span><span class="sxs-lookup"><span data-stu-id="bacb5-169">mentions</span></span>|<span data-ttu-id="bacb5-170">[chatMessageMention](chatmention.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bacb5-170">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="bacb5-171">Liste der Entitäten, die in der Nachricht angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="bacb5-171">List of entities mentioned in the message.</span></span> <span data-ttu-id="bacb5-172">Derzeit unterstützt: user, bot, team, channel</span><span class="sxs-lookup"><span data-stu-id="bacb5-172">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="bacb5-173">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="bacb5-173">importance</span></span>| <span data-ttu-id="bacb5-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-174">string</span></span> | <span data-ttu-id="bacb5-175">Legt die Wichtigkeit der Nachricht fest: Hoch, Niedrig</span><span class="sxs-lookup"><span data-stu-id="bacb5-175">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="bacb5-176">Reaktionen</span><span class="sxs-lookup"><span data-stu-id="bacb5-176">reactions</span></span>| <span data-ttu-id="bacb5-177">[chatMessageReaction](chatreaction.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bacb5-177">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="bacb5-178">Reaktionen auf diese Nachricht (z. B. Gefällt mir)</span><span class="sxs-lookup"><span data-stu-id="bacb5-178">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="bacb5-179">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="bacb5-179">locale</span></span>|<span data-ttu-id="bacb5-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bacb5-180">string</span></span>|<span data-ttu-id="bacb5-181">Vom Client festgelegtes Gebietsschema der Nachricht</span><span class="sxs-lookup"><span data-stu-id="bacb5-181">Locale of the message set by the client</span></span>|
|<span data-ttu-id="bacb5-182">Anlagen</span><span class="sxs-lookup"><span data-stu-id="bacb5-182">attachments</span></span>|<span data-ttu-id="bacb5-183">[chatMessageAttachment](chatattachment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bacb5-183">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="bacb5-184">Angefügte Dateien</span><span class="sxs-lookup"><span data-stu-id="bacb5-184">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bacb5-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bacb5-185">JSON representation</span></span>

<span data-ttu-id="bacb5-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bacb5-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
