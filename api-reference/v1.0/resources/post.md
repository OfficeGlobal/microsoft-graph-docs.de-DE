---
title: Beitragsressourcentyp
description: Stellt ein einzelnes Post-Element in einer conversationThread-Entität dar.
author: dkershaw10
ms.openlocfilehash: dcbf62d5415273ebd805fc930c746282519f386a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340040"
---
# <a name="post-resource-type"></a><span data-ttu-id="bf103-103">Beitragsressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bf103-103">post resource type</span></span>
<span data-ttu-id="bf103-104">Stellt ein einzelnes Post-Element in einer [conversationThread](conversationthread.md)-Entität dar.</span><span class="sxs-lookup"><span data-stu-id="bf103-104">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="bf103-105">Zwar können Sie Beiträge nicht explizit erstellen; es wird jedoch bei jedem der folgenden Vorgänge ein Beitrag erstellt:</span><span class="sxs-lookup"><span data-stu-id="bf103-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="bf103-106">auf einen vorhandenen Beitrag antworten</span><span class="sxs-lookup"><span data-stu-id="bf103-106">Reply to an existing post</span></span>](../api/post-reply.md) 
- [<span data-ttu-id="bf103-107">auf einen vorhandenen Thread antworten</span><span class="sxs-lookup"><span data-stu-id="bf103-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
- [<span data-ttu-id="bf103-108">einen Thread in einer neuen Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="bf103-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
- [<span data-ttu-id="bf103-109">eine neue Unterhaltung erstellen</span><span class="sxs-lookup"><span data-stu-id="bf103-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="bf103-110">Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="bf103-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="bf103-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="bf103-111">Methods</span></span>

| <span data-ttu-id="bf103-112">Methode</span><span class="sxs-lookup"><span data-stu-id="bf103-112">Method</span></span>       | <span data-ttu-id="bf103-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bf103-113">Return Type</span></span>  |<span data-ttu-id="bf103-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf103-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf103-115">List posts</span><span class="sxs-lookup"><span data-stu-id="bf103-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="bf103-116">post</span><span class="sxs-lookup"><span data-stu-id="bf103-116">post</span></span>](post.md) |<span data-ttu-id="bf103-117">Dient zum Abrufen der Beiträge des angegebenen Threads.</span><span class="sxs-lookup"><span data-stu-id="bf103-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="bf103-118">Get post</span><span class="sxs-lookup"><span data-stu-id="bf103-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="bf103-119">post</span><span class="sxs-lookup"><span data-stu-id="bf103-119">post</span></span>](post.md) |<span data-ttu-id="bf103-120">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread.</span><span class="sxs-lookup"><span data-stu-id="bf103-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="bf103-121">Reply</span><span class="sxs-lookup"><span data-stu-id="bf103-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="bf103-122">Keine</span><span class="sxs-lookup"><span data-stu-id="bf103-122">None</span></span>|<span data-ttu-id="bf103-123">Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung.</span><span class="sxs-lookup"><span data-stu-id="bf103-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="bf103-124">Forward</span><span class="sxs-lookup"><span data-stu-id="bf103-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="bf103-125">Keine</span><span class="sxs-lookup"><span data-stu-id="bf103-125">None</span></span>|<span data-ttu-id="bf103-126">Dient zum Weiterleiten eines Beitrags an einen Empfänger.</span><span class="sxs-lookup"><span data-stu-id="bf103-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="bf103-127">**Anlagen**</span><span class="sxs-lookup"><span data-stu-id="bf103-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="bf103-128">List attachments</span><span class="sxs-lookup"><span data-stu-id="bf103-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="bf103-129">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="bf103-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="bf103-130">Ruft alle Anlagen für einen Beitrag ab.</span><span class="sxs-lookup"><span data-stu-id="bf103-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="bf103-131">Hinzufügen von Anlagen</span><span class="sxs-lookup"><span data-stu-id="bf103-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="bf103-132">attachment</span><span class="sxs-lookup"><span data-stu-id="bf103-132">attachment</span></span>](attachment.md)| <span data-ttu-id="bf103-133">Dient zum Hinzufügen einer Anlage zu einem Beitrag.</span><span class="sxs-lookup"><span data-stu-id="bf103-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="bf103-134">**Offene Erweiterungen**</span><span class="sxs-lookup"><span data-stu-id="bf103-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="bf103-135">Offene Erweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="bf103-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="bf103-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="bf103-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="bf103-137">Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.</span><span class="sxs-lookup"><span data-stu-id="bf103-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="bf103-138">Offene Erweiterung abrufen</span><span class="sxs-lookup"><span data-stu-id="bf103-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="bf103-139">[openTypeExtension](opentypeextension.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bf103-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="bf103-140">Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.</span><span class="sxs-lookup"><span data-stu-id="bf103-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="bf103-141">**Schemaerweiterungen**</span><span class="sxs-lookup"><span data-stu-id="bf103-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="bf103-142">Schemaerweiterungswerte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="bf103-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="bf103-143">Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="bf103-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="bf103-144">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="bf103-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="bf103-145">Einwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="bf103-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="bf103-146">post</span><span class="sxs-lookup"><span data-stu-id="bf103-146">post</span></span>](post.md)  |<span data-ttu-id="bf103-147">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag.</span><span class="sxs-lookup"><span data-stu-id="bf103-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="bf103-148">Get post with single-value extended property</span><span class="sxs-lookup"><span data-stu-id="bf103-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="bf103-149">post</span><span class="sxs-lookup"><span data-stu-id="bf103-149">post</span></span>](post.md) | <span data-ttu-id="bf103-150">Dient zum Abrufen von Beiträgen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="bf103-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="bf103-151">Create multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="bf103-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="bf103-152">post</span><span class="sxs-lookup"><span data-stu-id="bf103-152">post</span></span>](post.md) | <span data-ttu-id="bf103-153">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag</span><span class="sxs-lookup"><span data-stu-id="bf103-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="bf103-154">Get post with multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="bf103-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="bf103-155">post</span><span class="sxs-lookup"><span data-stu-id="bf103-155">post</span></span>](post.md) | <span data-ttu-id="bf103-156">Dient zum Abrufen eines Beitrags mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="bf103-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="bf103-157">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bf103-157">Properties</span></span>
| <span data-ttu-id="bf103-158">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf103-158">Property</span></span>     | <span data-ttu-id="bf103-159">Typ</span><span class="sxs-lookup"><span data-stu-id="bf103-159">Type</span></span>   |<span data-ttu-id="bf103-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf103-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf103-161">body</span><span class="sxs-lookup"><span data-stu-id="bf103-161">body</span></span>|[<span data-ttu-id="bf103-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="bf103-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="bf103-p101">Der Inhalt des Beitrags. Dies ist eine Standardeigenschaft. Für diese Eigenschaft sind Nullwerte zulässig.</span><span class="sxs-lookup"><span data-stu-id="bf103-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="bf103-166">categories</span><span class="sxs-lookup"><span data-stu-id="bf103-166">categories</span></span>|<span data-ttu-id="bf103-167">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bf103-167">String collection</span></span>|<span data-ttu-id="bf103-168">Die Kategorien, die mit dem Beitrag verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="bf103-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="bf103-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="bf103-169">changeKey</span></span>|<span data-ttu-id="bf103-170">String</span><span class="sxs-lookup"><span data-stu-id="bf103-170">String</span></span>|<span data-ttu-id="bf103-p102">Gibt die Version des Beitrags an. Jedes Mal, wenn der Beitrag geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="bf103-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="bf103-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="bf103-174">conversationId</span></span>|<span data-ttu-id="bf103-175">String</span><span class="sxs-lookup"><span data-stu-id="bf103-175">String</span></span>|<span data-ttu-id="bf103-p103">Eindeutige ID der Unterhaltung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bf103-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="bf103-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="bf103-178">conversationThreadId</span></span>|<span data-ttu-id="bf103-179">String</span><span class="sxs-lookup"><span data-stu-id="bf103-179">String</span></span>|<span data-ttu-id="bf103-p104">Eindeutige ID des Unterhaltungsthreads. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bf103-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="bf103-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf103-182">createdDateTime</span></span>|<span data-ttu-id="bf103-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf103-183">DateTimeOffset</span></span>|<span data-ttu-id="bf103-p105">Gibt an, wann der Beitrag erstellt wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bf103-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bf103-187">Von</span><span class="sxs-lookup"><span data-stu-id="bf103-187">from</span></span>|[<span data-ttu-id="bf103-188">Empfänger</span><span class="sxs-lookup"><span data-stu-id="bf103-188">recipient</span></span>](recipient.md)|<span data-ttu-id="bf103-p106">Wird in Zugriffsszenarien mit Stellvertretungen verwendet. Gibt an, wer die Nachricht im Auftrag eines anderen Benutzers veröffentlicht hat. Dies ist eine Standardeigenschaft.</span><span class="sxs-lookup"><span data-stu-id="bf103-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="bf103-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="bf103-192">hasAttachments</span></span>|<span data-ttu-id="bf103-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bf103-193">Boolean</span></span>|<span data-ttu-id="bf103-p107">Gibt an, ob der Beitrag mindestens eine Anlage enthält. Dies ist eine Standardeigenschaft.</span><span class="sxs-lookup"><span data-stu-id="bf103-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="bf103-196">id</span><span class="sxs-lookup"><span data-stu-id="bf103-196">id</span></span>|<span data-ttu-id="bf103-197">String</span><span class="sxs-lookup"><span data-stu-id="bf103-197">String</span></span>| <span data-ttu-id="bf103-198">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bf103-198">Read-only.</span></span>|
|<span data-ttu-id="bf103-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf103-199">lastModifiedDateTime</span></span>|<span data-ttu-id="bf103-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf103-200">DateTimeOffset</span></span>|<span data-ttu-id="bf103-p108">Gibt an, wann der Beitrag zuletzt geändert wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bf103-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bf103-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="bf103-204">newParticipants</span></span>|<span data-ttu-id="bf103-205">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="bf103-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="bf103-206">Teilnehmer einer Unterhaltung, die im Rahmen des Beitrags zu dem Thread hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="bf103-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="bf103-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf103-207">receivedDateTime</span></span>|<span data-ttu-id="bf103-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf103-208">DateTimeOffset</span></span>|<span data-ttu-id="bf103-p109">Gibt an, wann der Beitrag empfangen wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bf103-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bf103-212">sender</span><span class="sxs-lookup"><span data-stu-id="bf103-212">sender</span></span>|[<span data-ttu-id="bf103-213">recipient</span><span class="sxs-lookup"><span data-stu-id="bf103-213">recipient</span></span>](recipient.md)|<span data-ttu-id="bf103-p110">Enthält die E-Mail-Adresse des Absenders. Bei dem Sender-Wert wird davon ausgegangen, dass dies die Adresse des authentifizierten Benutzers ist, wenn Absender nicht angegeben wurde. Dies ist eine Standardeigenschaft.</span><span class="sxs-lookup"><span data-stu-id="bf103-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf103-217">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bf103-217">Relationships</span></span>
| <span data-ttu-id="bf103-218">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bf103-218">Relationship</span></span> | <span data-ttu-id="bf103-219">Typ</span><span class="sxs-lookup"><span data-stu-id="bf103-219">Type</span></span>   |<span data-ttu-id="bf103-220">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf103-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf103-221">Anlagen</span><span class="sxs-lookup"><span data-stu-id="bf103-221">attachments</span></span>|<span data-ttu-id="bf103-222">[Anlagensammlung](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="bf103-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="bf103-p111">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bf103-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="bf103-225">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="bf103-225">extensions</span></span>|<span data-ttu-id="bf103-226">[Erweiterungssammlung](extension.md)</span><span class="sxs-lookup"><span data-stu-id="bf103-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="bf103-p112">Die Sammlung der für den Beitrag definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bf103-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bf103-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="bf103-230">inReplyTo</span></span>|[<span data-ttu-id="bf103-231">post</span><span class="sxs-lookup"><span data-stu-id="bf103-231">post</span></span>](post.md)| <span data-ttu-id="bf103-232">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bf103-232">Read-only.</span></span>|
|<span data-ttu-id="bf103-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bf103-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="bf103-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bf103-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bf103-p113">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="bf103-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bf103-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bf103-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="bf103-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bf103-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bf103-p114">Die Sammlung erweiterter einwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bf103-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf103-243">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bf103-243">JSON representation</span></span>

<span data-ttu-id="bf103-244">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bf103-244">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bf103-245">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="bf103-245">See also</span></span>

- [<span data-ttu-id="bf103-246">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="bf103-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bf103-247">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="bf103-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bf103-248">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="bf103-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
