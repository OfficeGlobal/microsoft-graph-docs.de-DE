---
title: channel-Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von chatMessages innerhalb eines Teams. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 73775cb446e9cd90eaf31ade28f25638465c884e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511002"
---
# <a name="channel-resource-type"></a><span data-ttu-id="b6b9e-103">channel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b6b9e-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6b9e-104">Ein Kanal ist eine Auflistung von [chatMessages](chatmessage.md) innerhalb eines [Teams](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b6b9e-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="b6b9e-105">Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="b6b9e-106">Beispiele sind der Kanal „Mittagessen mit dem Team am Freitag“ und „Besprechung der Architektur“.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="b6b9e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="b6b9e-107">Methods</span></span>

| <span data-ttu-id="b6b9e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="b6b9e-108">Method</span></span>       | <span data-ttu-id="b6b9e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b6b9e-109">Return Type</span></span>  |<span data-ttu-id="b6b9e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6b9e-111">List channels</span><span class="sxs-lookup"><span data-stu-id="b6b9e-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="b6b9e-112">[channel](channel.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="b6b9e-113">Abrufen der Liste von Kanälen in diesem Team.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="b6b9e-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="b6b9e-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="b6b9e-115">channel</span><span class="sxs-lookup"><span data-stu-id="b6b9e-115">channel</span></span>](channel.md) | <span data-ttu-id="b6b9e-116">Erstellen eines neuen Kanals durch Einschließen des Anzeigenamen und der Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="b6b9e-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="b6b9e-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="b6b9e-118">channel</span><span class="sxs-lookup"><span data-stu-id="b6b9e-118">channel</span></span>](channel.md) | <span data-ttu-id="b6b9e-119">Lesen von Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="b6b9e-120">Updatekanal</span><span class="sxs-lookup"><span data-stu-id="b6b9e-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="b6b9e-121">channel</span><span class="sxs-lookup"><span data-stu-id="b6b9e-121">channel</span></span>](channel.md) | <span data-ttu-id="b6b9e-122">Aktualisieren der Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="b6b9e-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="b6b9e-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="b6b9e-124">Keine</span><span class="sxs-lookup"><span data-stu-id="b6b9e-124">None</span></span> | <span data-ttu-id="b6b9e-125">Löschen eines Kanals.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-125">Delete a channel.</span></span>|
|[<span data-ttu-id="b6b9e-126">List channel messages</span><span class="sxs-lookup"><span data-stu-id="b6b9e-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="b6b9e-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b6b9e-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b6b9e-128">Abrufen von Nachrichten in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="b6b9e-129">Create chat thread</span><span class="sxs-lookup"><span data-stu-id="b6b9e-129">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="b6b9e-130">[chatThread](chatthread.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-130">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="b6b9e-131">Dient zum Erstellen eines Chatthreads in einem bestimmten Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-131">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6b9e-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b6b9e-132">Properties</span></span>
| <span data-ttu-id="b6b9e-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6b9e-133">Property</span></span>     | <span data-ttu-id="b6b9e-134">Typ</span><span class="sxs-lookup"><span data-stu-id="b6b9e-134">Type</span></span>   |<span data-ttu-id="b6b9e-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6b9e-136">description</span><span class="sxs-lookup"><span data-stu-id="b6b9e-136">description</span></span>|<span data-ttu-id="b6b9e-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6b9e-137">String</span></span>|<span data-ttu-id="b6b9e-138">Optionale Textbeschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="b6b9e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b6b9e-139">displayName</span></span>|<span data-ttu-id="b6b9e-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6b9e-140">String</span></span>|<span data-ttu-id="b6b9e-141">Kanalname wie er in Microsoft Teams für den Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="b6b9e-142">id</span><span class="sxs-lookup"><span data-stu-id="b6b9e-142">id</span></span>|<span data-ttu-id="b6b9e-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6b9e-143">String</span></span>|<span data-ttu-id="b6b9e-144">Eindeutiger Bezeichner für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-144">The channels's unique identifier.</span></span> <span data-ttu-id="b6b9e-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-145">Read-only.</span></span>|
|<span data-ttu-id="b6b9e-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="b6b9e-146">isFavoriteByDefault</span></span>|<span data-ttu-id="b6b9e-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6b9e-147">Boolean</span></span>|<span data-ttu-id="b6b9e-148">Gibt an, ob der Kanal automatisch für alle Mitglieder des Teams als „Favorit“ gekennzeichnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="b6b9e-149">Standard: `false`.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-149">Default: `false`.</span></span>|
|<span data-ttu-id="b6b9e-150">email</span><span class="sxs-lookup"><span data-stu-id="b6b9e-150">email</span></span>|<span data-ttu-id="b6b9e-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6b9e-151">Boolean</span></span>| <span data-ttu-id="b6b9e-152">Die E-Mail-Adresse zum Senden von Nachrichten an den Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="b6b9e-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-153">Read-only.</span></span>|
|<span data-ttu-id="b6b9e-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="b6b9e-154">webUrl</span></span>|<span data-ttu-id="b6b9e-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6b9e-155">String</span></span>|<span data-ttu-id="b6b9e-156">Ein Link, der in Microsoft Teams zum Kanal navigiert.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-156">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="b6b9e-157">Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten Maustaste in Microsoft Teams auf einen Kanal klicken, und auf die Option zum Abrufen des Links zum Kanal klicken.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-157">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="b6b9e-158">Diese URL sollte als nicht transparenter Blob behandelt und nicht analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="b6b9e-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b6b9e-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b6b9e-160">Relationships</span></span>
| <span data-ttu-id="b6b9e-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-161">Relationship</span></span> | <span data-ttu-id="b6b9e-162">Typ</span><span class="sxs-lookup"><span data-stu-id="b6b9e-162">Type</span></span>   |<span data-ttu-id="b6b9e-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6b9e-164">messages</span><span class="sxs-lookup"><span data-stu-id="b6b9e-164">messages</span></span>|<span data-ttu-id="b6b9e-165">[chatMessage](chatmessage.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="b6b9e-166">Eine Auflistung aller Nachrichten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="b6b9e-167">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-167">A navigation property.</span></span> <span data-ttu-id="b6b9e-168">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-168">Nullable.</span></span> <span data-ttu-id="b6b9e-169">Diese API unterstützt derzeit nur das Lesen von Nachrichten, das Schreiben wird aber auch bald unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="b6b9e-170">chatThreads</span><span class="sxs-lookup"><span data-stu-id="b6b9e-170">chatThreads</span></span>|<span data-ttu-id="b6b9e-171">[chatThread](chatthread.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-171">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="b6b9e-172">(Dies wird zugunsten der messages-Eigenschaften abgeschafft). chatThreads unterstützt das Erstellen neuer Nachrichten, aber nicht das Lesen von Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-172">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="b6b9e-173">ChatThreads ist eine Navigationseigenschaft, die Nullwerte zulässt.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-173">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="b6b9e-174">tabs</span><span class="sxs-lookup"><span data-stu-id="b6b9e-174">tabs</span></span>|<span data-ttu-id="b6b9e-175">[teamsTab](../resources/teamstab.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-175">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="b6b9e-176">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-176">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="b6b9e-177">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-177">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6b9e-178">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b6b9e-178">JSON representation</span></span>

<span data-ttu-id="b6b9e-179">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b6b9e-179">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
