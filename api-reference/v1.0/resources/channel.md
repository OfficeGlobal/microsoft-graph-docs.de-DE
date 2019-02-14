---
title: channel-Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten innerhalb eines Teams. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 052c6d8fc298e929dfd1c69e1b64debb7e14eb4a
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994454"
---
# <a name="channel-resource-type"></a><span data-ttu-id="40946-103">channel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="40946-103">channel resource type</span></span>



<span data-ttu-id="40946-104">Ein Kanal ist eine Auflistung von Nachrichten innerhalb eines [Teams](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="40946-104">A channel is a collection of chatMessages within a team.</span></span> <span data-ttu-id="40946-105">Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.</span><span class="sxs-lookup"><span data-stu-id="40946-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="40946-106">Beispiele sind der Kanal „Mittagessen mit dem Team am Freitag“ und „Besprechung der Architektur“.</span><span class="sxs-lookup"><span data-stu-id="40946-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="40946-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="40946-107">Methods</span></span>

| <span data-ttu-id="40946-108">Methode</span><span class="sxs-lookup"><span data-stu-id="40946-108">Method</span></span>       | <span data-ttu-id="40946-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="40946-109">Return Type</span></span>  |<span data-ttu-id="40946-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40946-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40946-111">List channels</span><span class="sxs-lookup"><span data-stu-id="40946-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="40946-112">[channel](channel.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="40946-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="40946-113">Abrufen der Liste von Kanälen in diesem Team.</span><span class="sxs-lookup"><span data-stu-id="40946-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="40946-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="40946-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="40946-115">channel</span><span class="sxs-lookup"><span data-stu-id="40946-115">channel</span></span>](channel.md) | <span data-ttu-id="40946-116">Erstellen eines neuen Kanals durch Einschließen des Anzeigenamen und der Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="40946-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="40946-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="40946-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="40946-118">channel</span><span class="sxs-lookup"><span data-stu-id="40946-118">channel</span></span>](channel.md) | <span data-ttu-id="40946-119">Lesen von Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="40946-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="40946-120">Updatekanal</span><span class="sxs-lookup"><span data-stu-id="40946-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="40946-121">channel</span><span class="sxs-lookup"><span data-stu-id="40946-121">channel</span></span>](channel.md) | <span data-ttu-id="40946-122">Aktualisieren der Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="40946-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="40946-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="40946-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="40946-124">Keine</span><span class="sxs-lookup"><span data-stu-id="40946-124">None</span></span> | <span data-ttu-id="40946-125">Löschen eines Kanals.</span><span class="sxs-lookup"><span data-stu-id="40946-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="40946-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40946-126">Properties</span></span>
| <span data-ttu-id="40946-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40946-127">Property</span></span>     | <span data-ttu-id="40946-128">Typ</span><span class="sxs-lookup"><span data-stu-id="40946-128">Type</span></span>   |<span data-ttu-id="40946-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40946-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40946-130">description</span><span class="sxs-lookup"><span data-stu-id="40946-130">description</span></span>|<span data-ttu-id="40946-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="40946-131">String</span></span>|<span data-ttu-id="40946-132">Optionale Textbeschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="40946-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="40946-133">displayName</span><span class="sxs-lookup"><span data-stu-id="40946-133">displayName</span></span>|<span data-ttu-id="40946-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="40946-134">String</span></span>|<span data-ttu-id="40946-135">Kanalname wie er in Microsoft Teams für den Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="40946-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="40946-136">id</span><span class="sxs-lookup"><span data-stu-id="40946-136">id</span></span>|<span data-ttu-id="40946-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="40946-137">String</span></span>|<span data-ttu-id="40946-138">Eindeutiger Bezeichner für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="40946-138">The channels's unique identifier.</span></span> <span data-ttu-id="40946-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40946-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40946-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="40946-140">Relationships</span></span>
| <span data-ttu-id="40946-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="40946-141">Relationship</span></span> | <span data-ttu-id="40946-142">Typ</span><span class="sxs-lookup"><span data-stu-id="40946-142">Type</span></span>   |<span data-ttu-id="40946-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40946-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40946-144">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="40946-144">tabs</span></span>|<span data-ttu-id="40946-145">[teamsTab](../resources/teamstab.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="40946-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="40946-146">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="40946-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="40946-147">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="40946-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="40946-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40946-148">JSON representation</span></span>

<span data-ttu-id="40946-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40946-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
