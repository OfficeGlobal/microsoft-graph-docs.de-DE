# <a name="channel-resource-type"></a><span data-ttu-id="08dbb-101">DDE-Kanal Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08dbb-101">channel resource type</span></span>



<span data-ttu-id="08dbb-102">Ein Kanal ist eine Auflistung von Nachrichten in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="08dbb-102">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="08dbb-103">Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.</span><span class="sxs-lookup"><span data-stu-id="08dbb-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="08dbb-104">Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.</span><span class="sxs-lookup"><span data-stu-id="08dbb-104">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="08dbb-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="08dbb-105">Methods</span></span>

| <span data-ttu-id="08dbb-106">Methode</span><span class="sxs-lookup"><span data-stu-id="08dbb-106">Method</span></span>       | <span data-ttu-id="08dbb-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="08dbb-107">Return Type</span></span>  |<span data-ttu-id="08dbb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08dbb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08dbb-109">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="08dbb-109">List channels</span></span>](../api/channel_list.md) | <span data-ttu-id="08dbb-110">[Kanal](channel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="08dbb-110">[channel](channel.md) collection</span></span> | <span data-ttu-id="08dbb-111">Rufen Sie die Liste der Kanäle in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="08dbb-111">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="08dbb-112">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="08dbb-112">Create channel</span></span>](../api/channel_post.md) | [<span data-ttu-id="08dbb-113">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="08dbb-113">channel</span></span>](channel.md) | <span data-ttu-id="08dbb-114">Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="08dbb-114">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="08dbb-115">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="08dbb-115">Get channel</span></span>](../api/channel_get.md) | [<span data-ttu-id="08dbb-116">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="08dbb-116">channel</span></span>](channel.md) | <span data-ttu-id="08dbb-117">Lesen Sie Eigenschaften und Beziehungen des Kanals.</span><span class="sxs-lookup"><span data-stu-id="08dbb-117">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="08dbb-118">Aktualisieren der DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="08dbb-118">Update channel</span></span>](../api/channel_patch.md) | [<span data-ttu-id="08dbb-119">DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="08dbb-119">channel</span></span>](channel.md) | <span data-ttu-id="08dbb-120">Aktualisieren Sie die Eigenschaften des Kanals.</span><span class="sxs-lookup"><span data-stu-id="08dbb-120">Update properties of the channel.</span></span>|
|[<span data-ttu-id="08dbb-121">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="08dbb-121">Delete channel</span></span>](../api/channel_delete.md) | <span data-ttu-id="08dbb-122">Keine</span><span class="sxs-lookup"><span data-stu-id="08dbb-122">None</span></span> | <span data-ttu-id="08dbb-123">Löschen Sie einen Kanal.</span><span class="sxs-lookup"><span data-stu-id="08dbb-123">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="08dbb-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08dbb-124">Properties</span></span>
| <span data-ttu-id="08dbb-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08dbb-125">Property</span></span>     | <span data-ttu-id="08dbb-126">Typ</span><span class="sxs-lookup"><span data-stu-id="08dbb-126">Type</span></span>   |<span data-ttu-id="08dbb-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08dbb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08dbb-128">description</span><span class="sxs-lookup"><span data-stu-id="08dbb-128">description</span></span>|<span data-ttu-id="08dbb-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08dbb-129">String</span></span>|<span data-ttu-id="08dbb-130">Optionale Beschreibung für den Kanal.</span><span class="sxs-lookup"><span data-stu-id="08dbb-130">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="08dbb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="08dbb-131">displayName</span></span>|<span data-ttu-id="08dbb-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08dbb-132">String</span></span>|<span data-ttu-id="08dbb-133">Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.</span><span class="sxs-lookup"><span data-stu-id="08dbb-133">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="08dbb-134">id</span><span class="sxs-lookup"><span data-stu-id="08dbb-134">id</span></span>|<span data-ttu-id="08dbb-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08dbb-135">String</span></span>|<span data-ttu-id="08dbb-136">Eindeutiger Bezeichner der Kanäle.</span><span class="sxs-lookup"><span data-stu-id="08dbb-136">The channels's unique identifier.</span></span> <span data-ttu-id="08dbb-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08dbb-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08dbb-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08dbb-138">Relationships</span></span>
| <span data-ttu-id="08dbb-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="08dbb-139">Relationship</span></span> | <span data-ttu-id="08dbb-140">Typ</span><span class="sxs-lookup"><span data-stu-id="08dbb-140">Type</span></span>   |<span data-ttu-id="08dbb-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08dbb-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08dbb-142">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="08dbb-142">tabs</span></span>|<span data-ttu-id="08dbb-143">[TeamsTab](../resources/teamstab.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="08dbb-143">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="08dbb-144">Eine Auflistung aller Registerkarten im Kanal.</span><span class="sxs-lookup"><span data-stu-id="08dbb-144">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="08dbb-145">Eine Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="08dbb-145">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="08dbb-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08dbb-146">JSON representation</span></span>

<span data-ttu-id="08dbb-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08dbb-147">Here is a JSON representation of the resource</span></span>

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
