---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von ChatMessages innerhalb eines Teams. '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065290"
---
# <a name="channel-resource-type"></a><span data-ttu-id="6577d-103">DDE-Kanal Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6577d-103">channel resource type</span></span>

> <span data-ttu-id="6577d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6577d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6577d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6577d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6577d-106">Ein Kanal ist eine Auflistung von [ChatMessages](chatmessage.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="6577d-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="6577d-107">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="6577d-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="6577d-108">Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.</span><span class="sxs-lookup"><span data-stu-id="6577d-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="6577d-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="6577d-109">Methods</span></span>

| <span data-ttu-id="6577d-110">Methode</span><span class="sxs-lookup"><span data-stu-id="6577d-110">Method</span></span>       | <span data-ttu-id="6577d-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6577d-111">Return Type</span></span>  |<span data-ttu-id="6577d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6577d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6577d-113">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="6577d-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="6577d-114">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6577d-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="6577d-115">Rufen Sie die Liste der Kanäle in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="6577d-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="6577d-116">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="6577d-117">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-117">channel</span></span>](channel.md) | <span data-ttu-id="6577d-118">Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="6577d-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="6577d-119">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="6577d-120">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-120">channel</span></span>](channel.md) | <span data-ttu-id="6577d-121">Lesen Sie Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="6577d-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="6577d-122">Aktualisieren der DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="6577d-123">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-123">channel</span></span>](channel.md) | <span data-ttu-id="6577d-124">Aktualisieren Sie die Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="6577d-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="6577d-125">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="6577d-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="6577d-126">Keines</span><span class="sxs-lookup"><span data-stu-id="6577d-126">None</span></span> | <span data-ttu-id="6577d-127">Löschen Sie einen Kanal.</span><span class="sxs-lookup"><span data-stu-id="6577d-127">Delete a channel.</span></span>|
|[<span data-ttu-id="6577d-128">Liste Channel Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6577d-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="6577d-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6577d-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6577d-130">Abrufen von Nachrichten in einem Kanal</span><span class="sxs-lookup"><span data-stu-id="6577d-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="6577d-131">Chat Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="6577d-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="6577d-132">[ChatThread](chatthread.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6577d-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="6577d-133">Erstellen Sie einen Chat Thread in den angegebenen DDE-Kanal.</span><span class="sxs-lookup"><span data-stu-id="6577d-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="6577d-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6577d-134">Properties</span></span>
| <span data-ttu-id="6577d-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6577d-135">Property</span></span>     | <span data-ttu-id="6577d-136">Typ</span><span class="sxs-lookup"><span data-stu-id="6577d-136">Type</span></span>   |<span data-ttu-id="6577d-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6577d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6577d-138">description</span><span class="sxs-lookup"><span data-stu-id="6577d-138">description</span></span>|<span data-ttu-id="6577d-139">String</span><span class="sxs-lookup"><span data-stu-id="6577d-139">String</span></span>|<span data-ttu-id="6577d-140">Optionale Beschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="6577d-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="6577d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6577d-141">displayName</span></span>|<span data-ttu-id="6577d-142">String</span><span class="sxs-lookup"><span data-stu-id="6577d-142">String</span></span>|<span data-ttu-id="6577d-143">Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.</span><span class="sxs-lookup"><span data-stu-id="6577d-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="6577d-144">id</span><span class="sxs-lookup"><span data-stu-id="6577d-144">id</span></span>|<span data-ttu-id="6577d-145">String</span><span class="sxs-lookup"><span data-stu-id="6577d-145">String</span></span>|<span data-ttu-id="6577d-146">Eindeutiger Bezeichner der Kanäle.</span><span class="sxs-lookup"><span data-stu-id="6577d-146">The channels's unique identifier.</span></span> <span data-ttu-id="6577d-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6577d-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6577d-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6577d-148">Relationships</span></span>
| <span data-ttu-id="6577d-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6577d-149">Relationship</span></span> | <span data-ttu-id="6577d-150">Typ</span><span class="sxs-lookup"><span data-stu-id="6577d-150">Type</span></span>   |<span data-ttu-id="6577d-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6577d-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6577d-152">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6577d-152">messages</span></span>|<span data-ttu-id="6577d-153">[ChatMessage](chatmessage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6577d-153">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="6577d-154">Eine Auflistung aller Nachrichten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="6577d-154">A collection of all the messages in the channel.</span></span> <span data-ttu-id="6577d-155">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="6577d-155">A navigation property.</span></span> <span data-ttu-id="6577d-156">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6577d-156">Nullable.</span></span> <span data-ttu-id="6577d-157">Diese API wird derzeit nur Lesevorgänge unterstützt, aber der Verfassen von Nachrichten schließlich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6577d-157">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="6577d-158">chatThreads</span><span class="sxs-lookup"><span data-stu-id="6577d-158">chatThreads</span></span>|<span data-ttu-id="6577d-159">[ChatThread](chatthread.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6577d-159">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="6577d-160">(Dies ist wird phased durch die Eigenschaft Nachrichten) ChatThreads Erstellen neuer Nachrichten aber nicht lesen von Nachrichten unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6577d-160">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="6577d-161">ChatThreads ist eine Navigationseigenschaft und zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="6577d-161">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="6577d-162">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="6577d-162">tabs</span></span>|<span data-ttu-id="6577d-163">[TeamsTab](../resources/teamstab.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6577d-163">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="6577d-164">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="6577d-164">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="6577d-165">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="6577d-165">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6577d-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6577d-166">JSON representation</span></span>

<span data-ttu-id="6577d-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6577d-167">Here is a JSON representation of the resource</span></span>

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
