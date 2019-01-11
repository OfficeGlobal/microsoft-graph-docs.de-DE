---
title: Ressourcentyp chatMessage
description: Stellt eine einzelne Chatnachricht innerhalb einer Entität Kanal oder Chat. Die Nachricht kann ein Stamm-Nachricht oder einen Teil davon ein Thread, der von der **ReplyToId** -Eigenschaft in der Nachricht definiert ist.
localization_priority: Priority
ms.openlocfilehash: ad381102f7e93a4dcccd7b68435d0687ed6b4837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855993"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="19e6e-104">Ressourcentyp chatMessage</span><span class="sxs-lookup"><span data-stu-id="19e6e-104">chatMessage resource type</span></span>

> <span data-ttu-id="19e6e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19e6e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19e6e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19e6e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19e6e-107">Stellt eine einzelne Chatnachricht innerhalb einer Entität [Kanal](channel.md) oder Chat.</span><span class="sxs-lookup"><span data-stu-id="19e6e-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="19e6e-108">Die Nachricht kann ein Stamm-Nachricht oder einen Teil davon ein Thread, der von der **ReplyToId** -Eigenschaft in der Nachricht definiert ist.</span><span class="sxs-lookup"><span data-stu-id="19e6e-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="19e6e-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="19e6e-109">Methods</span></span>

| <span data-ttu-id="19e6e-110">Methode</span><span class="sxs-lookup"><span data-stu-id="19e6e-110">Method</span></span>       | <span data-ttu-id="19e6e-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="19e6e-111">Return Type</span></span>  |<span data-ttu-id="19e6e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19e6e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19e6e-113">Liste Channel Nachrichten</span><span class="sxs-lookup"><span data-stu-id="19e6e-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="19e6e-114">[Chatmessage](chatmessage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="19e6e-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="19e6e-115">Rufen Sie die Liste aller Stamm-Nachrichten in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="19e6e-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="19e6e-116">Get-Channel-Nachricht</span><span class="sxs-lookup"><span data-stu-id="19e6e-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="19e6e-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="19e6e-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="19e6e-118">Rufen Sie eine Nachricht einzelnen Stamm aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="19e6e-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="19e6e-119">Liste Antworten auf eine Nachricht</span><span class="sxs-lookup"><span data-stu-id="19e6e-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="19e6e-120">[Chatmessage](chatmessage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="19e6e-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="19e6e-121">Abrufen der Liste mit allen Antworten auf eine Nachricht im Kanal.</span><span class="sxs-lookup"><span data-stu-id="19e6e-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="19e6e-122">Erhalten Sie eine Antwort auf eine Nachricht</span><span class="sxs-lookup"><span data-stu-id="19e6e-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="19e6e-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="19e6e-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="19e6e-124">Abrufen einer einzigen Antwort auf eine Nachricht in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="19e6e-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="19e6e-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19e6e-125">Properties</span></span>
| <span data-ttu-id="19e6e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19e6e-126">Property</span></span>     | <span data-ttu-id="19e6e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="19e6e-127">Type</span></span>   |<span data-ttu-id="19e6e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19e6e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19e6e-129">id</span><span class="sxs-lookup"><span data-stu-id="19e6e-129">id</span></span>|<span data-ttu-id="19e6e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19e6e-130">String</span></span>| <span data-ttu-id="19e6e-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19e6e-131">Read-only.</span></span> <span data-ttu-id="19e6e-132">Eindeutige ID der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="19e6e-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="19e6e-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="19e6e-133">replyToId</span></span>| <span data-ttu-id="19e6e-134">string</span><span class="sxs-lookup"><span data-stu-id="19e6e-134">string</span></span> | <span data-ttu-id="19e6e-135">ID der übergeordneten Nachricht/Root Nachricht des Threads</span><span class="sxs-lookup"><span data-stu-id="19e6e-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="19e6e-136">Von</span><span class="sxs-lookup"><span data-stu-id="19e6e-136">from</span></span>|[<span data-ttu-id="19e6e-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="19e6e-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="19e6e-138">Details des Absenders der Nachricht</span><span class="sxs-lookup"><span data-stu-id="19e6e-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="19e6e-139">etag</span><span class="sxs-lookup"><span data-stu-id="19e6e-139">etag</span></span>| <span data-ttu-id="19e6e-140">string</span><span class="sxs-lookup"><span data-stu-id="19e6e-140">string</span></span> | <span data-ttu-id="19e6e-141">Versionsnummer der Nachricht</span><span class="sxs-lookup"><span data-stu-id="19e6e-141">Version number of the message</span></span> |
|<span data-ttu-id="19e6e-142">messageType</span><span class="sxs-lookup"><span data-stu-id="19e6e-142">messageType</span></span>|<span data-ttu-id="19e6e-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19e6e-143">String</span></span>|<span data-ttu-id="19e6e-144">Der Typ der aktuellen Nachricht unterstützt Werte sind: Meldung, ChatEvent, Eingabe</span><span class="sxs-lookup"><span data-stu-id="19e6e-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="19e6e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19e6e-145">createdDateTime</span></span>|<span data-ttu-id="19e6e-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e6e-146">dateTimeOffset</span></span>|<span data-ttu-id="19e6e-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19e6e-147">Read only.</span></span> <span data-ttu-id="19e6e-148">Zeitstempel der Erstellung der Nachricht</span><span class="sxs-lookup"><span data-stu-id="19e6e-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="19e6e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19e6e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="19e6e-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e6e-150">dateTimeOffset</span></span>|<span data-ttu-id="19e6e-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19e6e-151">Read only.</span></span> <span data-ttu-id="19e6e-152">Wenn die Nachricht bearbeitet/aktualisiert wurde Zeitstempel</span><span class="sxs-lookup"><span data-stu-id="19e6e-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="19e6e-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="19e6e-153">isDeleted</span></span>|<span data-ttu-id="19e6e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="19e6e-154">boolean</span></span>|<span data-ttu-id="19e6e-155">Darstellt, wenn eine Nachricht weiche gelöscht wurde</span><span class="sxs-lookup"><span data-stu-id="19e6e-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="19e6e-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="19e6e-156">deletedDateTime</span></span>|<span data-ttu-id="19e6e-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e6e-157">dateTimeOffset</span></span>|<span data-ttu-id="19e6e-158">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19e6e-158">Read only.</span></span> <span data-ttu-id="19e6e-159">Zeitstempel, an dem die Nachricht gelöscht wurde</span><span class="sxs-lookup"><span data-stu-id="19e6e-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="19e6e-160">subject</span><span class="sxs-lookup"><span data-stu-id="19e6e-160">subject</span></span>|<span data-ttu-id="19e6e-161">string</span><span class="sxs-lookup"><span data-stu-id="19e6e-161">string</span></span>|<span data-ttu-id="19e6e-162">Betreffzeile der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="19e6e-162">Message subject line.</span></span> <span data-ttu-id="19e6e-163">Optional</span><span class="sxs-lookup"><span data-stu-id="19e6e-163">Optional</span></span>|
|<span data-ttu-id="19e6e-164">body</span><span class="sxs-lookup"><span data-stu-id="19e6e-164">body</span></span>|[<span data-ttu-id="19e6e-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="19e6e-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="19e6e-166">Nur-Text/HTML-Darstellung des Inhalts der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="19e6e-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="19e6e-167">Gibt nur-Text in der Standardeinstellung kann Anwendung HTML als Teil einer Abfrage Param auswählen</span><span class="sxs-lookup"><span data-stu-id="19e6e-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="19e6e-168">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="19e6e-168">summary</span></span>|<span data-ttu-id="19e6e-169">string</span><span class="sxs-lookup"><span data-stu-id="19e6e-169">string</span></span>|<span data-ttu-id="19e6e-170">Zusammengefassten Texts der Nachricht, die für Pushbenachrichtigungen und Übersichten oder fallen Back Ansichten verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="19e6e-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="19e6e-171">Erwähnungen</span><span class="sxs-lookup"><span data-stu-id="19e6e-171">mentions</span></span>|<span data-ttu-id="19e6e-172">[ChatMessageMention](chatmention.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="19e6e-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="19e6e-173">Liste der Entitäten, die in der Meldung genannten.</span><span class="sxs-lookup"><span data-stu-id="19e6e-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="19e6e-174">Derzeit unterstützt Benutzer, Bot, Team, DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="19e6e-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="19e6e-175">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="19e6e-175">importance</span></span>| <span data-ttu-id="19e6e-176">string</span><span class="sxs-lookup"><span data-stu-id="19e6e-176">string</span></span> | <span data-ttu-id="19e6e-177">Die Wichtigkeit der Nachricht: Normal, hoch</span><span class="sxs-lookup"><span data-stu-id="19e6e-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="19e6e-178">Reaktionen</span><span class="sxs-lookup"><span data-stu-id="19e6e-178">reactions</span></span>| <span data-ttu-id="19e6e-179">[ChatMessageReaction](chatreaction.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="19e6e-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="19e6e-180">Reaktionen für diese Nachricht (beispielsweise wie)</span><span class="sxs-lookup"><span data-stu-id="19e6e-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="19e6e-181">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="19e6e-181">locale</span></span>|<span data-ttu-id="19e6e-182">string</span><span class="sxs-lookup"><span data-stu-id="19e6e-182">string</span></span>|<span data-ttu-id="19e6e-183">Gebietsschema der Nachricht vom Client festgelegt</span><span class="sxs-lookup"><span data-stu-id="19e6e-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="19e6e-184">attachments</span><span class="sxs-lookup"><span data-stu-id="19e6e-184">attachments</span></span>|<span data-ttu-id="19e6e-185">[ChatMessageAttachment](chatattachment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="19e6e-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="19e6e-186">Dateianlagen</span><span class="sxs-lookup"><span data-stu-id="19e6e-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="19e6e-187">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19e6e-187">JSON representation</span></span>

<span data-ttu-id="19e6e-188">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19e6e-188">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
