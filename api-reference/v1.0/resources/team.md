---
title: Team Ressourcentyp
description: 'Ein Team in Microsoft-Teams ist eine Auflistung der Kanäle. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7dff1bb05b2abe604963657d4691766eeeaae4ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976933"
---
# <a name="team-resource-type"></a><span data-ttu-id="f8e6a-103">Team Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8e6a-103">team resource type</span></span>



<span data-ttu-id="f8e6a-104">Ein Team in Microsoft-Teams ist eine Auflistung der [Kanäle](channel.md).</span><span class="sxs-lookup"><span data-stu-id="f8e6a-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="f8e6a-105">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="f8e6a-106">Jedes Team ist eine [Gruppe](../resources/group.md)zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="f8e6a-107">Die Gruppe verfügt über die gleiche ID wie die Team - beispielsweise /groups/ {Id} / Team ist identisch mit /teams/ {Id}.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="f8e6a-108">Weitere Informationen über das Arbeiten mit Gruppen und Membern im Teams finden Sie unter [Verwenden der Microsoft Graph-REST-API entwickelt Microsoft-Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="f8e6a-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f8e6a-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f8e6a-109">Methods</span></span>

| <span data-ttu-id="f8e6a-110">Methode</span><span class="sxs-lookup"><span data-stu-id="f8e6a-110">Method</span></span>       | <span data-ttu-id="f8e6a-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f8e6a-111">Return Type</span></span>  |<span data-ttu-id="f8e6a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8e6a-113">Erstellen von Teams</span><span class="sxs-lookup"><span data-stu-id="f8e6a-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="f8e6a-114">Team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-114">team</span></span>](team.md) | <span data-ttu-id="f8e6a-115">Erstellen Sie ein neues Team oder fügen Sie ein Team an eine vorhandene Gruppe hinzu.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="f8e6a-116">Get-team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="f8e6a-117">Team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-117">team</span></span>](team.md) | <span data-ttu-id="f8e6a-118">Abrufen der Eigenschaften und Beziehungen zwischen dem angegebenen Team.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="f8e6a-119">Update-team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="f8e6a-120">Team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-120">team</span></span>](team.md) |<span data-ttu-id="f8e6a-121">Aktualisieren Sie die Eigenschaften des angegebenen Teams.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="f8e6a-122">Team löschen</span><span class="sxs-lookup"><span data-stu-id="f8e6a-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="f8e6a-123">Keine</span><span class="sxs-lookup"><span data-stu-id="f8e6a-123">None</span></span> |<span data-ttu-id="f8e6a-124">Das Team und der zugeordneten Gruppe zu löschen.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="f8e6a-125">Wenn Sie den Klon-team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="f8e6a-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="f8e6a-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="f8e6a-127">Kopieren Sie das Team und dessen zugehörige Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="f8e6a-128">Archiv-team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="f8e6a-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="f8e6a-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="f8e6a-130">Platzieren Sie das Team in einem schreibgeschützten Zustand.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="f8e6a-131">Entpackt team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="f8e6a-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="f8e6a-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="f8e6a-133">Wiederherstellen Sie das Team eine Lese-/ Schreibzugriff Zustand.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="f8e6a-134">Listen Sie Ihren teams</span><span class="sxs-lookup"><span data-stu-id="f8e6a-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="f8e6a-135">[Team](team.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-135">[team](team.md) collection</span></span> | <span data-ttu-id="f8e6a-136">Listen Sie Teams, denen Sie Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="f8e6a-137">Listen Sie alle teams</span><span class="sxs-lookup"><span data-stu-id="f8e6a-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="f8e6a-138">[Gruppensammlung](group.md)</span><span class="sxs-lookup"><span data-stu-id="f8e6a-138">[group](group.md) collection</span></span> | <span data-ttu-id="f8e6a-139">Listen Sie alle Gruppen, bei die Teams haben.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="f8e6a-140">Veröffentlichen von apps in Ihrer Organisation</span><span class="sxs-lookup"><span data-stu-id="f8e6a-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="f8e6a-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f8e6a-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="f8e6a-142">Erstellen von Teams apps wird nur für Ihre Organisation angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="f8e6a-143">Team app hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f8e6a-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="f8e6a-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="f8e6a-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="f8e6a-145">Fügt (installiert) einer app zu einem Team.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="f8e6a-146">Registerkarte Channel hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f8e6a-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="f8e6a-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f8e6a-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="f8e6a-148">Fügt (installiert) eine Registerkarte, um ein Team des DDE-Kanal.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="f8e6a-149">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8e6a-149">Properties</span></span>

| <span data-ttu-id="f8e6a-150">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8e6a-150">Property</span></span> | <span data-ttu-id="f8e6a-151">Typ</span><span class="sxs-lookup"><span data-stu-id="f8e6a-151">Type</span></span>   | <span data-ttu-id="f8e6a-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f8e6a-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-153">funSettings</span></span>|[<span data-ttu-id="f8e6a-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="f8e6a-155">So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="f8e6a-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-156">guestSettings</span></span>|[<span data-ttu-id="f8e6a-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="f8e6a-158">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="f8e6a-159">isArchived</span><span class="sxs-lookup"><span data-stu-id="f8e6a-159">isArchived</span></span>|<span data-ttu-id="f8e6a-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f8e6a-160">Boolean</span></span>|<span data-ttu-id="f8e6a-161">Gibt an, ob dieses Team im schreibgeschützten Modus ist.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-161">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="f8e6a-162">memberSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-162">memberSettings</span></span>|[<span data-ttu-id="f8e6a-163">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-163">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="f8e6a-164">Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-164">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="f8e6a-165">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-165">messagingSettings</span></span>|[<span data-ttu-id="f8e6a-166">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="f8e6a-166">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="f8e6a-167">So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-167">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="f8e6a-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="f8e6a-168">webUrl</span></span>|<span data-ttu-id="f8e6a-169">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="f8e6a-169">string (readonly)</span></span> | <span data-ttu-id="f8e6a-170">Ein Hyperlink, der an das Team in der Microsoft-Teams, Client gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-170">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="f8e6a-171">Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten ein Team in der Microsoft-Teams, Client Maustaste und wählen Sie **Link an das Team abrufen**.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-171">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="f8e6a-172">Diese URL sollte als nicht transparentes Blob behandelt und nicht analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-172">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f8e6a-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f8e6a-173">Relationships</span></span>

| <span data-ttu-id="f8e6a-174">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-174">Relationship</span></span> | <span data-ttu-id="f8e6a-175">Typ</span><span class="sxs-lookup"><span data-stu-id="f8e6a-175">Type</span></span>   | <span data-ttu-id="f8e6a-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-176">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f8e6a-177">Kanäle</span><span class="sxs-lookup"><span data-stu-id="f8e6a-177">channels</span></span>|<span data-ttu-id="f8e6a-178">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-178">[channel](channel.md) collection</span></span>|<span data-ttu-id="f8e6a-179">Die Auflistung der Kanäle & Nachrichten, die dem Team zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-179">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="f8e6a-180">installedApps</span><span class="sxs-lookup"><span data-stu-id="f8e6a-180">installedApps</span></span>|<span data-ttu-id="f8e6a-181">[TeamsAppInstallation](teamsappinstallation.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-181">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="f8e6a-182">Die apps in dieser Gruppe installiert.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-182">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8e6a-183">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8e6a-183">JSON representation</span></span>

<span data-ttu-id="f8e6a-184">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8e6a-184">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f8e6a-185">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f8e6a-185">See Also</span></span>
- [<span data-ttu-id="f8e6a-186">Erstellen einer Gruppe mit einem team</span><span class="sxs-lookup"><span data-stu-id="f8e6a-186">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="f8e6a-187">Verwenden von Teams-APIs</span><span class="sxs-lookup"><span data-stu-id="f8e6a-187">Using Teams APIs</span></span>](teams-api-overview.md)
