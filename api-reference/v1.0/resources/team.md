---
title: team-Ressourcentyp
description: 'Ein Team in Microsoft Teams ist eine Sammlung von Kanälen. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 692f0d12c172fb6b7088912eec952b519d852cac
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735572"
---
# <a name="team-resource-type"></a><span data-ttu-id="e0a05-103">team-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0a05-103">team resource type</span></span>



<span data-ttu-id="e0a05-104">Ein Team in Microsoft Teams ist eine Sammlung von [Kanälen](channel.md).</span><span class="sxs-lookup"><span data-stu-id="e0a05-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="e0a05-105">Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.</span><span class="sxs-lookup"><span data-stu-id="e0a05-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="e0a05-106">Jedes Team wird einer [Gruppe](../resources/group.md) zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="e0a05-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="e0a05-107">Die Gruppe hat die gleiche ID wie das Team – z. B. ist /groups/{id}/team identisch mit /teams/{id}.</span><span class="sxs-lookup"><span data-stu-id="e0a05-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="e0a05-108">Weitere Informationen zum Arbeiten mit Gruppen und Mitgliedern in Teams finden Sie unter [Verwenden der Microsoft Graph REST-API zum Arbeiten mit Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e0a05-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e0a05-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="e0a05-109">Methods</span></span>

| <span data-ttu-id="e0a05-110">Methode</span><span class="sxs-lookup"><span data-stu-id="e0a05-110">Method</span></span>       | <span data-ttu-id="e0a05-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e0a05-111">Return Type</span></span>  |<span data-ttu-id="e0a05-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0a05-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0a05-113">Team erstellen</span><span class="sxs-lookup"><span data-stu-id="e0a05-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="e0a05-114">team</span><span class="sxs-lookup"><span data-stu-id="e0a05-114">team</span></span>](team.md) | <span data-ttu-id="e0a05-115">Erstellen eines neuen Teams oder Hinzufügen eines Teams zu einer vorhandenen Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e0a05-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="e0a05-116">Team abrufen</span><span class="sxs-lookup"><span data-stu-id="e0a05-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="e0a05-117">team</span><span class="sxs-lookup"><span data-stu-id="e0a05-117">team</span></span>](team.md) | <span data-ttu-id="e0a05-118">Abrufen der Eigenschaften und Beziehungen des angegebenen Teams.</span><span class="sxs-lookup"><span data-stu-id="e0a05-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="e0a05-119">Team aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e0a05-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="e0a05-120">team</span><span class="sxs-lookup"><span data-stu-id="e0a05-120">team</span></span>](team.md) |<span data-ttu-id="e0a05-121">Aktualisieren der Eigenschaften des angegebenen Teams.</span><span class="sxs-lookup"><span data-stu-id="e0a05-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="e0a05-122">Team löschen</span><span class="sxs-lookup"><span data-stu-id="e0a05-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="e0a05-123">Keine</span><span class="sxs-lookup"><span data-stu-id="e0a05-123">None</span></span> |<span data-ttu-id="e0a05-124">Löschen des Teams und der zugehörigen Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e0a05-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="e0a05-125">Team klonen</span><span class="sxs-lookup"><span data-stu-id="e0a05-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="e0a05-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e0a05-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e0a05-127">Kopieren des Teams und der zugehörigen Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e0a05-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="e0a05-128">Team archivieren</span><span class="sxs-lookup"><span data-stu-id="e0a05-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="e0a05-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e0a05-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e0a05-130">Versetzen des Teams in einen schreibgeschützten Zustand.</span><span class="sxs-lookup"><span data-stu-id="e0a05-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="e0a05-131">Archivierung von Team aufheben</span><span class="sxs-lookup"><span data-stu-id="e0a05-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="e0a05-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e0a05-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e0a05-133">Zurückversetzen des Teams in den Zustand Lesen/Schreiben.</span><span class="sxs-lookup"><span data-stu-id="e0a05-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="e0a05-134">Ihre Teams auflisten</span><span class="sxs-lookup"><span data-stu-id="e0a05-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="e0a05-135">[team](team.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e0a05-135">[team](team.md) collection</span></span> | <span data-ttu-id="e0a05-136">Auflisten der Teams, in denen Sie Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="e0a05-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="e0a05-137">Auflisten aller Teams</span><span class="sxs-lookup"><span data-stu-id="e0a05-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="e0a05-138">[group](group.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e0a05-138">[group](group.md) collection</span></span> | <span data-ttu-id="e0a05-139">Auflisten aller Gruppen, die über Teams verfügen.</span><span class="sxs-lookup"><span data-stu-id="e0a05-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="e0a05-140">Apps in Ihrer Organisation veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="e0a05-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="e0a05-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e0a05-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="e0a05-142">Erstellen von Teams-Apps, die nur für Ihre Organisation sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="e0a05-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="e0a05-143">App zu Team hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e0a05-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="e0a05-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="e0a05-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="e0a05-145">Hinzufügen (Installieren) einer App zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="e0a05-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="e0a05-146">Registerkarte zu Kanal hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e0a05-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e0a05-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e0a05-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="e0a05-148">Hinzufügen (Installieren) einer Registerkarte zum Kanal des Teams.</span><span class="sxs-lookup"><span data-stu-id="e0a05-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0a05-149">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0a05-149">Properties</span></span>

| <span data-ttu-id="e0a05-150">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0a05-150">Property</span></span> | <span data-ttu-id="e0a05-151">Typ</span><span class="sxs-lookup"><span data-stu-id="e0a05-151">Type</span></span>   | <span data-ttu-id="e0a05-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0a05-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a05-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-153">funSettings</span></span>|[<span data-ttu-id="e0a05-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="e0a05-155">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memen und Aufklebern im Team.</span><span class="sxs-lookup"><span data-stu-id="e0a05-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="e0a05-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-156">guestSettings</span></span>|[<span data-ttu-id="e0a05-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="e0a05-158">Einstellungen zum Konfigurieren, ob Gäste Kanäle im Team erstellen, aktualisieren oder löschen können.</span><span class="sxs-lookup"><span data-stu-id="e0a05-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="e0a05-159">internalId</span><span class="sxs-lookup"><span data-stu-id="e0a05-159">InternalId</span></span> | <span data-ttu-id="e0a05-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0a05-160">string</span></span> | <span data-ttu-id="e0a05-161">Eine eindeutige ID für das Team, das an einigen Stellen verwendet wurde, zum Beispiel Überwachungsprotokoll/[Office 365-Verwaltungsaktivitäts-API](https://docs.microsoft.com/de-DE/office/office-365-management-api/office-365-management-activity-api-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a05-161">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/de-DE/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="e0a05-162">isArchived</span><span class="sxs-lookup"><span data-stu-id="e0a05-162">isArchived</span></span>|<span data-ttu-id="e0a05-163">Boolesch</span><span class="sxs-lookup"><span data-stu-id="e0a05-163">Boolean</span></span>|<span data-ttu-id="e0a05-164">Gibt an, ob sich das Team im schreibgeschützten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="e0a05-164">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="e0a05-165">memberSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-165">memberSettings</span></span>|[<span data-ttu-id="e0a05-166">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-166">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="e0a05-167">Einstellungen zum Konfigurieren, ob Mitglieder bestimmte Aktionen, z. B. Kanäle erstellen und Bots hinzufügen, im Team ausführen können.</span><span class="sxs-lookup"><span data-stu-id="e0a05-167">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="e0a05-168">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-168">messagingSettings</span></span>|[<span data-ttu-id="e0a05-169">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="e0a05-169">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="e0a05-170">Einstellungen zum Konfigurieren von Messaging und Erwähnungen im Team.</span><span class="sxs-lookup"><span data-stu-id="e0a05-170">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="e0a05-171">webUrl</span><span class="sxs-lookup"><span data-stu-id="e0a05-171">webUrl</span></span>|<span data-ttu-id="e0a05-172">string (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="e0a05-172">string (readonly)</span></span> | <span data-ttu-id="e0a05-173">Ein Link, der im Microsoft Teams-Client zu dem Team führt.</span><span class="sxs-lookup"><span data-stu-id="e0a05-173">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="e0a05-174">Dies ist die URL, die Sie erhalten, wenn Sie im Microsoft Teams-Client mit der rechten Maustaste auf ein Team klicken und **Link zum Team abrufen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="e0a05-174">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="e0a05-175">Diese URL sollte als nicht transparenter Blob behandelt und nicht analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="e0a05-175">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e0a05-176">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e0a05-176">Relationships</span></span>

| <span data-ttu-id="e0a05-177">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e0a05-177">Relationship</span></span> | <span data-ttu-id="e0a05-178">Typ</span><span class="sxs-lookup"><span data-stu-id="e0a05-178">Type</span></span>   | <span data-ttu-id="e0a05-179">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0a05-179">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a05-180">channels</span><span class="sxs-lookup"><span data-stu-id="e0a05-180">channels</span></span>|<span data-ttu-id="e0a05-181">[channel](channel.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e0a05-181">[channel](channel.md) collection</span></span>|<span data-ttu-id="e0a05-182">Die Sammlung von Kanälen und Nachrichten, die mit dem Team verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="e0a05-182">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="e0a05-183">installedApps</span><span class="sxs-lookup"><span data-stu-id="e0a05-183">installedApps</span></span>|<span data-ttu-id="e0a05-184">[teamsAppInstallation](teamsappinstallation.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e0a05-184">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="e0a05-185">Die in diesem Team installierten Apps.</span><span class="sxs-lookup"><span data-stu-id="e0a05-185">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0a05-186">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0a05-186">JSON representation</span></span>

<span data-ttu-id="e0a05-187">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0a05-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{  
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "internalId": "19:...big.number...@thread.skype",
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="e0a05-188">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e0a05-188">See Also</span></span>
- [<span data-ttu-id="e0a05-189">Erstellen einer Gruppe mit einem Team</span><span class="sxs-lookup"><span data-stu-id="e0a05-189">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="e0a05-190">Verwenden der Teams-API</span><span class="sxs-lookup"><span data-stu-id="e0a05-190">Using Teams APIs</span></span>](teams-api-overview.md)
