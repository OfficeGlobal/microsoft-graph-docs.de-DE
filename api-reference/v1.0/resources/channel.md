---
title: channel-Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten innerhalb eines Teams. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163714"
---
# <a name="channel-resource-type"></a><span data-ttu-id="02445-103">channel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="02445-103">channel resource type</span></span>



<span data-ttu-id="02445-104">Ein Kanal ist eine Auflistung von Nachrichten innerhalb eines [Teams](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="02445-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="02445-105">Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.</span><span class="sxs-lookup"><span data-stu-id="02445-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="02445-106">Beispiele sind der Kanal „Mittagessen mit dem Team am Freitag“ und „Besprechung der Architektur“.</span><span class="sxs-lookup"><span data-stu-id="02445-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="02445-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="02445-107">Methods</span></span>

| <span data-ttu-id="02445-108">Methode</span><span class="sxs-lookup"><span data-stu-id="02445-108">Method</span></span>       | <span data-ttu-id="02445-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="02445-109">Return Type</span></span>  |<span data-ttu-id="02445-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02445-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02445-111">List channels</span><span class="sxs-lookup"><span data-stu-id="02445-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="02445-112">[channel](channel.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="02445-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="02445-113">Abrufen der Liste von Kanälen in diesem Team.</span><span class="sxs-lookup"><span data-stu-id="02445-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="02445-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="02445-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="02445-115">channel</span><span class="sxs-lookup"><span data-stu-id="02445-115">channel</span></span>](channel.md) | <span data-ttu-id="02445-116">Erstellen eines neuen Kanals durch Einschließen des Anzeigenamen und der Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="02445-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="02445-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="02445-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="02445-118">channel</span><span class="sxs-lookup"><span data-stu-id="02445-118">channel</span></span>](channel.md) | <span data-ttu-id="02445-119">Lesen von Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="02445-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="02445-120">Updatekanal</span><span class="sxs-lookup"><span data-stu-id="02445-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="02445-121">channel</span><span class="sxs-lookup"><span data-stu-id="02445-121">channel</span></span>](channel.md) | <span data-ttu-id="02445-122">Aktualisieren der Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="02445-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="02445-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="02445-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="02445-124">Keine</span><span class="sxs-lookup"><span data-stu-id="02445-124">None</span></span> | <span data-ttu-id="02445-125">Löschen eines Kanals.</span><span class="sxs-lookup"><span data-stu-id="02445-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="02445-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02445-126">Properties</span></span>
| <span data-ttu-id="02445-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02445-127">Property</span></span>     | <span data-ttu-id="02445-128">Typ</span><span class="sxs-lookup"><span data-stu-id="02445-128">Type</span></span>   |<span data-ttu-id="02445-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02445-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02445-130">description</span><span class="sxs-lookup"><span data-stu-id="02445-130">description</span></span>|<span data-ttu-id="02445-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02445-131">String</span></span>|<span data-ttu-id="02445-132">Optionale Textbeschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="02445-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="02445-133">displayName</span><span class="sxs-lookup"><span data-stu-id="02445-133">displayName</span></span>|<span data-ttu-id="02445-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02445-134">String</span></span>|<span data-ttu-id="02445-135">Kanalname wie er in Microsoft Teams für den Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="02445-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="02445-136">id</span><span class="sxs-lookup"><span data-stu-id="02445-136">id</span></span>|<span data-ttu-id="02445-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02445-137">String</span></span>|<span data-ttu-id="02445-138">Eindeutiger Bezeichner für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="02445-138">The channels's unique identifier.</span></span> <span data-ttu-id="02445-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="02445-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02445-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="02445-140">Relationships</span></span>
| <span data-ttu-id="02445-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="02445-141">Relationship</span></span> | <span data-ttu-id="02445-142">Typ</span><span class="sxs-lookup"><span data-stu-id="02445-142">Type</span></span>   |<span data-ttu-id="02445-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02445-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02445-144">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="02445-144">tabs</span></span>|<span data-ttu-id="02445-145">[teamsTab](../resources/teamstab.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="02445-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="02445-146">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="02445-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="02445-147">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="02445-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="02445-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02445-148">JSON representation</span></span>

<span data-ttu-id="02445-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02445-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
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
