---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten in einem Team. '
author: nkramer
ms.openlocfilehash: f9ab71213180732a0c8c626d5b32b9074bd135d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337086"
---
# <a name="channel-resource-type"></a><span data-ttu-id="9274c-103">DDE-Kanal Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9274c-103">channel resource type</span></span>



<span data-ttu-id="9274c-104">Ein Kanal ist eine Auflistung von Nachrichten in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9274c-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="9274c-105">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="9274c-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="9274c-106">Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.</span><span class="sxs-lookup"><span data-stu-id="9274c-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="9274c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9274c-107">Methods</span></span>

| <span data-ttu-id="9274c-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9274c-108">Method</span></span>       | <span data-ttu-id="9274c-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9274c-109">Return Type</span></span>  |<span data-ttu-id="9274c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9274c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9274c-111">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="9274c-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="9274c-112">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9274c-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="9274c-113">Rufen Sie die Liste der Kanäle in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="9274c-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="9274c-114">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="9274c-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="9274c-115">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="9274c-115">channel</span></span>](channel.md) | <span data-ttu-id="9274c-116">Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="9274c-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="9274c-117">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="9274c-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="9274c-118">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="9274c-118">channel</span></span>](channel.md) | <span data-ttu-id="9274c-119">Lesen Sie Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="9274c-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="9274c-120">Aktualisieren der DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="9274c-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="9274c-121">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="9274c-121">channel</span></span>](channel.md) | <span data-ttu-id="9274c-122">Aktualisieren Sie die Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="9274c-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="9274c-123">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="9274c-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="9274c-124">Keines</span><span class="sxs-lookup"><span data-stu-id="9274c-124">None</span></span> | <span data-ttu-id="9274c-125">Löschen Sie einen Kanal.</span><span class="sxs-lookup"><span data-stu-id="9274c-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="9274c-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9274c-126">Properties</span></span>
| <span data-ttu-id="9274c-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9274c-127">Property</span></span>     | <span data-ttu-id="9274c-128">Typ</span><span class="sxs-lookup"><span data-stu-id="9274c-128">Type</span></span>   |<span data-ttu-id="9274c-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9274c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9274c-130">description</span><span class="sxs-lookup"><span data-stu-id="9274c-130">description</span></span>|<span data-ttu-id="9274c-131">String</span><span class="sxs-lookup"><span data-stu-id="9274c-131">String</span></span>|<span data-ttu-id="9274c-132">Optionale Beschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="9274c-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="9274c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9274c-133">displayName</span></span>|<span data-ttu-id="9274c-134">String</span><span class="sxs-lookup"><span data-stu-id="9274c-134">String</span></span>|<span data-ttu-id="9274c-135">Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.</span><span class="sxs-lookup"><span data-stu-id="9274c-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="9274c-136">id</span><span class="sxs-lookup"><span data-stu-id="9274c-136">id</span></span>|<span data-ttu-id="9274c-137">String</span><span class="sxs-lookup"><span data-stu-id="9274c-137">String</span></span>|<span data-ttu-id="9274c-138">Eindeutiger Bezeichner der Kanäle.</span><span class="sxs-lookup"><span data-stu-id="9274c-138">The channels's unique identifier.</span></span> <span data-ttu-id="9274c-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9274c-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9274c-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9274c-140">Relationships</span></span>
| <span data-ttu-id="9274c-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9274c-141">Relationship</span></span> | <span data-ttu-id="9274c-142">Typ</span><span class="sxs-lookup"><span data-stu-id="9274c-142">Type</span></span>   |<span data-ttu-id="9274c-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9274c-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9274c-144">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="9274c-144">tabs</span></span>|<span data-ttu-id="9274c-145">[TeamsTab](../resources/teamstab.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9274c-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="9274c-146">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="9274c-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="9274c-147">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="9274c-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9274c-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9274c-148">JSON representation</span></span>

<span data-ttu-id="9274c-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9274c-149">Here is a JSON representation of the resource</span></span>

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
