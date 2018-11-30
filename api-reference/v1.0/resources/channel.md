---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten in einem Team. '
ms.openlocfilehash: 17a2e2edb86bfe7e107e69414a70dbe92fe4d3bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017420"
---
# <a name="channel-resource-type"></a><span data-ttu-id="b59fe-103">DDE-Kanal Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b59fe-103">channel resource type</span></span>



<span data-ttu-id="b59fe-104">Ein Kanal ist eine Auflistung von Nachrichten in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b59fe-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="b59fe-105">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="b59fe-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="b59fe-106">Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.</span><span class="sxs-lookup"><span data-stu-id="b59fe-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="b59fe-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="b59fe-107">Methods</span></span>

| <span data-ttu-id="b59fe-108">Methode</span><span class="sxs-lookup"><span data-stu-id="b59fe-108">Method</span></span>       | <span data-ttu-id="b59fe-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b59fe-109">Return Type</span></span>  |<span data-ttu-id="b59fe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b59fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b59fe-111">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="b59fe-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="b59fe-112">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b59fe-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="b59fe-113">Rufen Sie die Liste der Kanäle in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="b59fe-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="b59fe-114">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b59fe-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="b59fe-115">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b59fe-115">channel</span></span>](channel.md) | <span data-ttu-id="b59fe-116">Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="b59fe-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="b59fe-117">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b59fe-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="b59fe-118">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b59fe-118">channel</span></span>](channel.md) | <span data-ttu-id="b59fe-119">Lesen Sie Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="b59fe-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="b59fe-120">Aktualisieren der DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b59fe-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="b59fe-121">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b59fe-121">channel</span></span>](channel.md) | <span data-ttu-id="b59fe-122">Aktualisieren Sie die Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="b59fe-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="b59fe-123">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="b59fe-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="b59fe-124">Keines</span><span class="sxs-lookup"><span data-stu-id="b59fe-124">None</span></span> | <span data-ttu-id="b59fe-125">Löschen Sie einen Kanal.</span><span class="sxs-lookup"><span data-stu-id="b59fe-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="b59fe-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b59fe-126">Properties</span></span>
| <span data-ttu-id="b59fe-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b59fe-127">Property</span></span>     | <span data-ttu-id="b59fe-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b59fe-128">Type</span></span>   |<span data-ttu-id="b59fe-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b59fe-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b59fe-130">description</span><span class="sxs-lookup"><span data-stu-id="b59fe-130">description</span></span>|<span data-ttu-id="b59fe-131">String</span><span class="sxs-lookup"><span data-stu-id="b59fe-131">String</span></span>|<span data-ttu-id="b59fe-132">Optionale Beschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="b59fe-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="b59fe-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b59fe-133">displayName</span></span>|<span data-ttu-id="b59fe-134">String</span><span class="sxs-lookup"><span data-stu-id="b59fe-134">String</span></span>|<span data-ttu-id="b59fe-135">Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.</span><span class="sxs-lookup"><span data-stu-id="b59fe-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="b59fe-136">id</span><span class="sxs-lookup"><span data-stu-id="b59fe-136">id</span></span>|<span data-ttu-id="b59fe-137">String</span><span class="sxs-lookup"><span data-stu-id="b59fe-137">String</span></span>|<span data-ttu-id="b59fe-138">Eindeutiger Bezeichner der Kanäle.</span><span class="sxs-lookup"><span data-stu-id="b59fe-138">The channels's unique identifier.</span></span> <span data-ttu-id="b59fe-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b59fe-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b59fe-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b59fe-140">Relationships</span></span>
| <span data-ttu-id="b59fe-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b59fe-141">Relationship</span></span> | <span data-ttu-id="b59fe-142">Typ</span><span class="sxs-lookup"><span data-stu-id="b59fe-142">Type</span></span>   |<span data-ttu-id="b59fe-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b59fe-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b59fe-144">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="b59fe-144">tabs</span></span>|<span data-ttu-id="b59fe-145">[TeamsTab](../resources/teamstab.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b59fe-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="b59fe-146">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="b59fe-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="b59fe-147">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b59fe-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b59fe-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b59fe-148">JSON representation</span></span>

<span data-ttu-id="b59fe-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b59fe-149">Here is a JSON representation of the resource</span></span>

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
