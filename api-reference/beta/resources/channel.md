---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von ChatMessages innerhalb eines Teams. '
author: nkramer
ms.openlocfilehash: 18a3293b757e641eab98b166a43ce023762ccc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326775"
---
# <a name="channel-resource-type"></a><span data-ttu-id="f5d48-103">DDE-Kanal Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f5d48-103">channel resource type</span></span>

> <span data-ttu-id="f5d48-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f5d48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5d48-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5d48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5d48-106">Ein Kanal ist eine Auflistung von [ChatMessages](chatmessage.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f5d48-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="f5d48-107">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="f5d48-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="f5d48-108">Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.</span><span class="sxs-lookup"><span data-stu-id="f5d48-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="f5d48-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f5d48-109">Methods</span></span>

| <span data-ttu-id="f5d48-110">Methode</span><span class="sxs-lookup"><span data-stu-id="f5d48-110">Method</span></span>       | <span data-ttu-id="f5d48-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f5d48-111">Return Type</span></span>  |<span data-ttu-id="f5d48-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5d48-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5d48-113">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="f5d48-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="f5d48-114">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f5d48-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="f5d48-115">Rufen Sie die Liste der Kanäle in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f5d48-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="f5d48-116">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="f5d48-117">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-117">channel</span></span>](channel.md) | <span data-ttu-id="f5d48-118">Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="f5d48-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="f5d48-119">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="f5d48-120">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-120">channel</span></span>](channel.md) | <span data-ttu-id="f5d48-121">Lesen Sie Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="f5d48-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="f5d48-122">Aktualisieren der DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="f5d48-123">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-123">channel</span></span>](channel.md) | <span data-ttu-id="f5d48-124">Aktualisieren Sie die Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="f5d48-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="f5d48-125">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="f5d48-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="f5d48-126">Keines</span><span class="sxs-lookup"><span data-stu-id="f5d48-126">None</span></span> | <span data-ttu-id="f5d48-127">Löschen Sie einen Kanal.</span><span class="sxs-lookup"><span data-stu-id="f5d48-127">Delete a channel.</span></span>|
|[<span data-ttu-id="f5d48-128">Liste Channel Nachrichten</span><span class="sxs-lookup"><span data-stu-id="f5d48-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="f5d48-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f5d48-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f5d48-130">Abrufen von Nachrichten in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="f5d48-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="f5d48-131">Chat Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="f5d48-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="f5d48-132">[ChatThread](chatthread.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f5d48-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="f5d48-133">Erstellen Sie einen Chat Thread in den angegebenen DDE-Kanal.</span><span class="sxs-lookup"><span data-stu-id="f5d48-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5d48-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f5d48-134">Properties</span></span>
| <span data-ttu-id="f5d48-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f5d48-135">Property</span></span>     | <span data-ttu-id="f5d48-136">Typ</span><span class="sxs-lookup"><span data-stu-id="f5d48-136">Type</span></span>   |<span data-ttu-id="f5d48-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5d48-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5d48-138">description</span><span class="sxs-lookup"><span data-stu-id="f5d48-138">description</span></span>|<span data-ttu-id="f5d48-139">String</span><span class="sxs-lookup"><span data-stu-id="f5d48-139">String</span></span>|<span data-ttu-id="f5d48-140">Optionale Beschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="f5d48-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="f5d48-141">displayName</span><span class="sxs-lookup"><span data-stu-id="f5d48-141">displayName</span></span>|<span data-ttu-id="f5d48-142">String</span><span class="sxs-lookup"><span data-stu-id="f5d48-142">String</span></span>|<span data-ttu-id="f5d48-143">Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.</span><span class="sxs-lookup"><span data-stu-id="f5d48-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="f5d48-144">id</span><span class="sxs-lookup"><span data-stu-id="f5d48-144">id</span></span>|<span data-ttu-id="f5d48-145">String</span><span class="sxs-lookup"><span data-stu-id="f5d48-145">String</span></span>|<span data-ttu-id="f5d48-146">Eindeutiger Bezeichner der Kanäle.</span><span class="sxs-lookup"><span data-stu-id="f5d48-146">The channels's unique identifier.</span></span> <span data-ttu-id="f5d48-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f5d48-147">Read-only.</span></span>|
|<span data-ttu-id="f5d48-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="f5d48-148">isFavoriteByDefault</span></span>|<span data-ttu-id="f5d48-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f5d48-149">Boolean</span></span>|<span data-ttu-id="f5d48-150">Gibt an, ob der Kanal automatisch "Favoriten" für alle Mitglieder des Teams gekennzeichnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f5d48-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="f5d48-151">Standard: `false`.</span><span class="sxs-lookup"><span data-stu-id="f5d48-151">Default: `false`.</span></span>|
|<span data-ttu-id="f5d48-152">E-Mail</span><span class="sxs-lookup"><span data-stu-id="f5d48-152">email</span></span>|<span data-ttu-id="f5d48-153">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f5d48-153">Boolean</span></span>| <span data-ttu-id="f5d48-154">Die e-Mail-Adresse zum Senden von Nachrichten an den Kanal.</span><span class="sxs-lookup"><span data-stu-id="f5d48-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="f5d48-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f5d48-155">Read-only.</span></span>|
|<span data-ttu-id="f5d48-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="f5d48-156">webUrl</span></span>|<span data-ttu-id="f5d48-157">String</span><span class="sxs-lookup"><span data-stu-id="f5d48-157">String</span></span>|<span data-ttu-id="f5d48-158">Ein Hyperlink, zu dem navigiert an den Kanal in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="f5d48-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="f5d48-159">Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten Maustaste in eines Kanals in Microsoft-Teams, und wählen Sie Get-Link Kanal aus.</span><span class="sxs-lookup"><span data-stu-id="f5d48-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="f5d48-160">Diese URL sollte als nicht transparentes Blob behandelt und nicht analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="f5d48-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="f5d48-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f5d48-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f5d48-162">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f5d48-162">Relationships</span></span>
| <span data-ttu-id="f5d48-163">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f5d48-163">Relationship</span></span> | <span data-ttu-id="f5d48-164">Typ</span><span class="sxs-lookup"><span data-stu-id="f5d48-164">Type</span></span>   |<span data-ttu-id="f5d48-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5d48-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5d48-166">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="f5d48-166">messages</span></span>|<span data-ttu-id="f5d48-167">[ChatMessage](chatmessage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f5d48-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="f5d48-168">Eine Auflistung aller Nachrichten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="f5d48-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="f5d48-169">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="f5d48-169">A navigation property.</span></span> <span data-ttu-id="f5d48-170">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f5d48-170">Nullable.</span></span> <span data-ttu-id="f5d48-171">Diese API wird derzeit nur Lesevorgänge unterstützt, aber der Verfassen von Nachrichten schließlich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f5d48-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="f5d48-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="f5d48-172">chatThreads</span></span>|<span data-ttu-id="f5d48-173">[ChatThread](chatthread.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f5d48-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="f5d48-174">(Dies ist wird phased durch die Eigenschaft Nachrichten) ChatThreads Erstellen neuer Nachrichten aber nicht lesen von Nachrichten unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5d48-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="f5d48-175">ChatThreads ist eine Navigationseigenschaft und zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f5d48-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="f5d48-176">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="f5d48-176">tabs</span></span>|<span data-ttu-id="f5d48-177">[TeamsTab](../resources/teamstab.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f5d48-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="f5d48-178">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="f5d48-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="f5d48-179">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="f5d48-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f5d48-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f5d48-180">JSON representation</span></span>

<span data-ttu-id="f5d48-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f5d48-181">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
