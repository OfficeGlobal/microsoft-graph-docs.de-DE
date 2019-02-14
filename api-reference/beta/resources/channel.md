---
title: channel-Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von chatMessages innerhalb eines Teams. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994468"
---
# <a name="channel-resource-type"></a><span data-ttu-id="35431-103">channel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="35431-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35431-104">Ein Kanal ist eine Auflistung von [chatMessages](chatmessage.md) innerhalb eines [Teams](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="35431-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="35431-105">Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.</span><span class="sxs-lookup"><span data-stu-id="35431-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="35431-106">Beispiele sind der Kanal „Mittagessen mit dem Team am Freitag“ und „Besprechung der Architektur“.</span><span class="sxs-lookup"><span data-stu-id="35431-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="35431-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="35431-107">Methods</span></span>

| <span data-ttu-id="35431-108">Methode</span><span class="sxs-lookup"><span data-stu-id="35431-108">Method</span></span>       | <span data-ttu-id="35431-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="35431-109">Return Type</span></span>  |<span data-ttu-id="35431-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35431-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35431-111">List channels</span><span class="sxs-lookup"><span data-stu-id="35431-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="35431-112">[channel](channel.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="35431-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="35431-113">Abrufen der Liste von Kanälen in diesem Team.</span><span class="sxs-lookup"><span data-stu-id="35431-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="35431-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="35431-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="35431-115">channel</span><span class="sxs-lookup"><span data-stu-id="35431-115">channel</span></span>](channel.md) | <span data-ttu-id="35431-116">Erstellen eines neuen Kanals durch Einschließen des Anzeigenamen und der Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="35431-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="35431-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="35431-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="35431-118">channel</span><span class="sxs-lookup"><span data-stu-id="35431-118">channel</span></span>](channel.md) | <span data-ttu-id="35431-119">Lesen von Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="35431-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="35431-120">Updatekanal</span><span class="sxs-lookup"><span data-stu-id="35431-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="35431-121">channel</span><span class="sxs-lookup"><span data-stu-id="35431-121">channel</span></span>](channel.md) | <span data-ttu-id="35431-122">Aktualisieren der Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="35431-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="35431-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="35431-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="35431-124">Keine</span><span class="sxs-lookup"><span data-stu-id="35431-124">None</span></span> | <span data-ttu-id="35431-125">Löschen eines Kanals.</span><span class="sxs-lookup"><span data-stu-id="35431-125">Delete a channel.</span></span>|
|[<span data-ttu-id="35431-126">List channel messages</span><span class="sxs-lookup"><span data-stu-id="35431-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="35431-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="35431-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="35431-128">Abrufen von Nachrichten in einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="35431-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="35431-129">Kanalnachricht senden</span><span class="sxs-lookup"><span data-stu-id="35431-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="35431-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="35431-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="35431-131">Senden einer Nachricht an einen Kanal</span><span class="sxs-lookup"><span data-stu-id="35431-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |


## <a name="properties"></a><span data-ttu-id="35431-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35431-132">Properties</span></span>
| <span data-ttu-id="35431-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35431-133">Property</span></span>     | <span data-ttu-id="35431-134">Typ</span><span class="sxs-lookup"><span data-stu-id="35431-134">Type</span></span>   |<span data-ttu-id="35431-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35431-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35431-136">description</span><span class="sxs-lookup"><span data-stu-id="35431-136">description</span></span>|<span data-ttu-id="35431-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35431-137">String</span></span>|<span data-ttu-id="35431-138">Optionale Textbeschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="35431-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="35431-139">displayName</span><span class="sxs-lookup"><span data-stu-id="35431-139">displayName</span></span>|<span data-ttu-id="35431-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35431-140">String</span></span>|<span data-ttu-id="35431-141">Kanalname wie er in Microsoft Teams für den Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="35431-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="35431-142">id</span><span class="sxs-lookup"><span data-stu-id="35431-142">id</span></span>|<span data-ttu-id="35431-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35431-143">String</span></span>|<span data-ttu-id="35431-144">Eindeutiger Bezeichner für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="35431-144">The channels's unique identifier.</span></span> <span data-ttu-id="35431-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35431-145">Read-only.</span></span>|
|<span data-ttu-id="35431-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="35431-146">isFavoriteByDefault</span></span>|<span data-ttu-id="35431-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="35431-147">Boolean</span></span>|<span data-ttu-id="35431-148">Gibt an, ob der Kanal automatisch für alle Mitglieder des Teams als „Favorit“ gekennzeichnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="35431-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="35431-149">Standard: `false`.</span><span class="sxs-lookup"><span data-stu-id="35431-149">Default: `false`.</span></span>|
|<span data-ttu-id="35431-150">email</span><span class="sxs-lookup"><span data-stu-id="35431-150">email</span></span>|<span data-ttu-id="35431-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="35431-151">Boolean</span></span>| <span data-ttu-id="35431-152">Die E-Mail-Adresse zum Senden von Nachrichten an den Kanal.</span><span class="sxs-lookup"><span data-stu-id="35431-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="35431-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35431-153">Read-only.</span></span>|
|<span data-ttu-id="35431-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="35431-154">webUrl</span></span>|<span data-ttu-id="35431-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35431-155">String</span></span>|<span data-ttu-id="35431-156">Ein Link, der in Microsoft Teams zum Kanal navigiert.</span><span class="sxs-lookup"><span data-stu-id="35431-156">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="35431-157">Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten Maustaste in Microsoft Teams auf einen Kanal klicken, und auf die Option zum Abrufen des Links zum Kanal klicken.</span><span class="sxs-lookup"><span data-stu-id="35431-157">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="35431-158">Diese URL sollte als nicht transparenter Blob behandelt und nicht analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="35431-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="35431-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35431-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="35431-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="35431-160">Relationships</span></span>
| <span data-ttu-id="35431-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="35431-161">Relationship</span></span> | <span data-ttu-id="35431-162">Typ</span><span class="sxs-lookup"><span data-stu-id="35431-162">Type</span></span>   |<span data-ttu-id="35431-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35431-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35431-164">messages</span><span class="sxs-lookup"><span data-stu-id="35431-164">messages</span></span>|<span data-ttu-id="35431-165">[chatMessage](chatmessage.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="35431-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="35431-166">Eine Auflistung aller Nachrichten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="35431-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="35431-167">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="35431-167">A navigation property.</span></span> <span data-ttu-id="35431-168">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="35431-168">Nullable.</span></span> <span data-ttu-id="35431-169">Diese API unterstützt derzeit nur das Lesen von Nachrichten, das Schreiben wird aber auch bald unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35431-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="35431-170">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="35431-170">tabs</span></span>|<span data-ttu-id="35431-171">[teamsTab](../resources/teamstab.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="35431-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="35431-172">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="35431-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="35431-173">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="35431-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="35431-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35431-174">JSON representation</span></span>

<span data-ttu-id="35431-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35431-175">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
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
