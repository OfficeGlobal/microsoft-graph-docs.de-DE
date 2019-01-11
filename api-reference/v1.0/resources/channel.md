---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten in einem Team. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 9a7b12646f36152bef17cec2d206e8e84abdcbbe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826565"
---
# <a name="channel-resource-type"></a><span data-ttu-id="d3c3a-103">DDE-Kanal Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d3c3a-103">channel resource type</span></span>



<span data-ttu-id="d3c3a-104">Ein Kanal ist eine Auflistung von Nachrichten in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d3c3a-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="d3c3a-105">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="d3c3a-106">Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="d3c3a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d3c3a-107">Methods</span></span>

| <span data-ttu-id="d3c3a-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d3c3a-108">Method</span></span>       | <span data-ttu-id="d3c3a-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d3c3a-109">Return Type</span></span>  |<span data-ttu-id="d3c3a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3c3a-111">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="d3c3a-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="d3c3a-112">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="d3c3a-113">Rufen Sie die Liste der Kanäle in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="d3c3a-114">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="d3c3a-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="d3c3a-115">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="d3c3a-115">channel</span></span>](channel.md) | <span data-ttu-id="d3c3a-116">Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="d3c3a-117">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="d3c3a-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="d3c3a-118">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="d3c3a-118">channel</span></span>](channel.md) | <span data-ttu-id="d3c3a-119">Lesen Sie Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="d3c3a-120">Aktualisieren der DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="d3c3a-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="d3c3a-121">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="d3c3a-121">channel</span></span>](channel.md) | <span data-ttu-id="d3c3a-122">Aktualisieren Sie die Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="d3c3a-123">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="d3c3a-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="d3c3a-124">Keine</span><span class="sxs-lookup"><span data-stu-id="d3c3a-124">None</span></span> | <span data-ttu-id="d3c3a-125">Löschen Sie einen Kanal.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3c3a-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3c3a-126">Properties</span></span>
| <span data-ttu-id="d3c3a-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3c3a-127">Property</span></span>     | <span data-ttu-id="d3c3a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="d3c3a-128">Type</span></span>   |<span data-ttu-id="d3c3a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c3a-130">description</span><span class="sxs-lookup"><span data-stu-id="d3c3a-130">description</span></span>|<span data-ttu-id="d3c3a-131">String</span><span class="sxs-lookup"><span data-stu-id="d3c3a-131">String</span></span>|<span data-ttu-id="d3c3a-132">Optionale Beschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="d3c3a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d3c3a-133">displayName</span></span>|<span data-ttu-id="d3c3a-134">String</span><span class="sxs-lookup"><span data-stu-id="d3c3a-134">String</span></span>|<span data-ttu-id="d3c3a-135">Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="d3c3a-136">id</span><span class="sxs-lookup"><span data-stu-id="d3c3a-136">id</span></span>|<span data-ttu-id="d3c3a-137">String</span><span class="sxs-lookup"><span data-stu-id="d3c3a-137">String</span></span>|<span data-ttu-id="d3c3a-138">Eindeutiger Bezeichner der Kanäle.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-138">The channels's unique identifier.</span></span> <span data-ttu-id="d3c3a-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3c3a-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d3c3a-140">Relationships</span></span>
| <span data-ttu-id="d3c3a-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-141">Relationship</span></span> | <span data-ttu-id="d3c3a-142">Typ</span><span class="sxs-lookup"><span data-stu-id="d3c3a-142">Type</span></span>   |<span data-ttu-id="d3c3a-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c3a-144">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="d3c3a-144">tabs</span></span>|<span data-ttu-id="d3c3a-145">[TeamsTab](../resources/teamstab.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="d3c3a-146">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="d3c3a-147">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d3c3a-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3c3a-148">JSON representation</span></span>

<span data-ttu-id="d3c3a-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3c3a-149">Here is a JSON representation of the resource</span></span>

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
