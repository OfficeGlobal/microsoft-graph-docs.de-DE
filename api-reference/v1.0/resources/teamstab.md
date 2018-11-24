# <a name="teamstab-resource-type"></a><span data-ttu-id="a4182-101">Ressourcentyp teamsTab</span><span class="sxs-lookup"><span data-stu-id="a4182-101">teamsTab resource type</span></span>



<span data-ttu-id="a4182-102">Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen).</span><span class="sxs-lookup"><span data-stu-id="a4182-102">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a4182-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="a4182-103">Methods</span></span>

| <span data-ttu-id="a4182-104">Methode</span><span class="sxs-lookup"><span data-stu-id="a4182-104">Method</span></span>       | <span data-ttu-id="a4182-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a4182-105">Return Type</span></span>  |<span data-ttu-id="a4182-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4182-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4182-107">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="a4182-107">List tabs</span></span>](../api/teamstab_list.md) | [<span data-ttu-id="a4182-108">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a4182-108">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a4182-109">Listen Registerkarten fixiert zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="a4182-109">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a4182-110">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="a4182-110">Get tab</span></span>](../api/teamstab_get.md) | [<span data-ttu-id="a4182-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a4182-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a4182-112">Liest eine Registerkarte an einen Kanal fixiert.</span><span class="sxs-lookup"><span data-stu-id="a4182-112">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a4182-113">Registerkarte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a4182-113">Add tab</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="a4182-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a4182-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a4182-115">Fügt (Pins) einer Registerkarte zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="a4182-115">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a4182-116">Registerkarte entfernen</span><span class="sxs-lookup"><span data-stu-id="a4182-116">Remove tab</span></span>](../api/teamstab_delete.md) | <span data-ttu-id="a4182-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a4182-117">None</span></span> | <span data-ttu-id="a4182-118">Entfernt (löst) einer Registerkarte aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="a4182-118">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="a4182-119">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="a4182-119">Update tab</span></span>](../api/teamstab_update.md) | [<span data-ttu-id="a4182-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a4182-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a4182-121">Aktualisiert die Registerkarte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="a4182-121">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a4182-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a4182-122">Properties</span></span>

|<span data-ttu-id="a4182-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4182-123">Property</span></span>|<span data-ttu-id="a4182-124">Typ</span><span class="sxs-lookup"><span data-stu-id="a4182-124">Type</span></span>|<span data-ttu-id="a4182-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4182-125">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a4182-126">id</span><span class="sxs-lookup"><span data-stu-id="a4182-126">id</span></span>              |   <span data-ttu-id="a4182-127">string</span><span class="sxs-lookup"><span data-stu-id="a4182-127">string</span></span>                  |  <span data-ttu-id="a4182-128">Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.</span><span class="sxs-lookup"><span data-stu-id="a4182-128">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a4182-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a4182-129">displayName</span></span>            |   <span data-ttu-id="a4182-130">string</span><span class="sxs-lookup"><span data-stu-id="a4182-130">string</span></span>                  |  <span data-ttu-id="a4182-131">Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="a4182-131">Name of the tab.</span></span>     |
|  <span data-ttu-id="a4182-132">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="a4182-132">sortOrderIndex</span></span>  |   <span data-ttu-id="a4182-133">Int</span><span class="sxs-lookup"><span data-stu-id="a4182-133">int</span></span>                     |  <span data-ttu-id="a4182-134">Index der Reihenfolge für die Sortierung von Registerkarten</span><span class="sxs-lookup"><span data-stu-id="a4182-134">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="a4182-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="a4182-135">webUrl</span></span>          |   <span data-ttu-id="a4182-136">string</span><span class="sxs-lookup"><span data-stu-id="a4182-136">string</span></span>                  |  <span data-ttu-id="a4182-137">Deep-Link-Url der Registerkarte-Instanz.</span><span class="sxs-lookup"><span data-stu-id="a4182-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="a4182-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4182-138">Read only.</span></span>     |
|  <span data-ttu-id="a4182-139">Konfiguration</span><span class="sxs-lookup"><span data-stu-id="a4182-139">configuration</span></span>        |   [<span data-ttu-id="a4182-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4182-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a4182-141">Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="a4182-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a4182-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a4182-142">Relationships</span></span>

| <span data-ttu-id="a4182-143">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a4182-143">Relationship</span></span> | <span data-ttu-id="a4182-144">Typ</span><span class="sxs-lookup"><span data-stu-id="a4182-144">Type</span></span>   | <span data-ttu-id="a4182-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4182-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a4182-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a4182-146">teamsApp</span></span>|[<span data-ttu-id="a4182-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a4182-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a4182-148">Die Anwendung, die auf der Registerkarte verknüpft ist. Nach der Erstellung der Registerkarte werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="a4182-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4182-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a4182-149">JSON representation</span></span>

<span data-ttu-id="a4182-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a4182-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="a4182-151">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a4182-151">See also</span></span>

[<span data-ttu-id="a4182-152">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="a4182-152">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)
