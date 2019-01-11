---
title: Ressourcentyp teamsTab
description: 'Eine TeamsTab ist eine Registerkarte, hat fixiert an einen Kanal innerhalb eines Teams (angeschlossen). '
localization_priority: Normal
ms.openlocfilehash: a1c3302251ac9b68be1cd8d6a011b7e0a7d216b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860844"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="ada86-103">Ressourcentyp teamsTab</span><span class="sxs-lookup"><span data-stu-id="ada86-103">teamsTab resource type</span></span>



<span data-ttu-id="ada86-104">Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen).</span><span class="sxs-lookup"><span data-stu-id="ada86-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ada86-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="ada86-105">Methods</span></span>

| <span data-ttu-id="ada86-106">Methode</span><span class="sxs-lookup"><span data-stu-id="ada86-106">Method</span></span>       | <span data-ttu-id="ada86-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ada86-107">Return Type</span></span>  |<span data-ttu-id="ada86-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ada86-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ada86-109">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="ada86-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="ada86-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ada86-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ada86-111">Listen Registerkarten fixiert zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="ada86-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="ada86-112">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="ada86-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="ada86-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ada86-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ada86-114">Liest eine Registerkarte an einen Kanal fixiert.</span><span class="sxs-lookup"><span data-stu-id="ada86-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="ada86-115">Registerkarte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ada86-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="ada86-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ada86-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ada86-117">Fügt (Pins) einer Registerkarte zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="ada86-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="ada86-118">Registerkarte entfernen</span><span class="sxs-lookup"><span data-stu-id="ada86-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="ada86-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ada86-119">None</span></span> | <span data-ttu-id="ada86-120">Entfernt (löst) einer Registerkarte aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="ada86-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="ada86-121">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="ada86-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="ada86-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ada86-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ada86-123">Aktualisiert die Registerkarte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="ada86-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ada86-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ada86-124">Properties</span></span>

|<span data-ttu-id="ada86-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ada86-125">Property</span></span>|<span data-ttu-id="ada86-126">Typ</span><span class="sxs-lookup"><span data-stu-id="ada86-126">Type</span></span>|<span data-ttu-id="ada86-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ada86-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="ada86-128">id</span><span class="sxs-lookup"><span data-stu-id="ada86-128">id</span></span>              |   <span data-ttu-id="ada86-129">string</span><span class="sxs-lookup"><span data-stu-id="ada86-129">string</span></span>                  |  <span data-ttu-id="ada86-130">Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.</span><span class="sxs-lookup"><span data-stu-id="ada86-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="ada86-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ada86-131">displayName</span></span>            |   <span data-ttu-id="ada86-132">string</span><span class="sxs-lookup"><span data-stu-id="ada86-132">string</span></span>                  |  <span data-ttu-id="ada86-133">Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="ada86-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="ada86-134">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="ada86-134">sortOrderIndex</span></span>  |   <span data-ttu-id="ada86-135">int</span><span class="sxs-lookup"><span data-stu-id="ada86-135">int</span></span>                     |  <span data-ttu-id="ada86-136">Index der Reihenfolge für die Sortierung von Registerkarten</span><span class="sxs-lookup"><span data-stu-id="ada86-136">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="ada86-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="ada86-137">webUrl</span></span>          |   <span data-ttu-id="ada86-138">string</span><span class="sxs-lookup"><span data-stu-id="ada86-138">string</span></span>                  |  <span data-ttu-id="ada86-139">Deep-Link-Url der Registerkarte-Instanz.</span><span class="sxs-lookup"><span data-stu-id="ada86-139">Deep link url of the tab instance.</span></span> <span data-ttu-id="ada86-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ada86-140">Read only.</span></span>     |
|  <span data-ttu-id="ada86-141">Konfiguration</span><span class="sxs-lookup"><span data-stu-id="ada86-141">configuration</span></span>        |   [<span data-ttu-id="ada86-142">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada86-142">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="ada86-143">Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="ada86-143">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="ada86-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ada86-144">Relationships</span></span>

| <span data-ttu-id="ada86-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ada86-145">Relationship</span></span> | <span data-ttu-id="ada86-146">Typ</span><span class="sxs-lookup"><span data-stu-id="ada86-146">Type</span></span>   | <span data-ttu-id="ada86-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ada86-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ada86-148">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ada86-148">teamsApp</span></span>|[<span data-ttu-id="ada86-149">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ada86-149">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ada86-150">Die Anwendung, die auf der Registerkarte verknüpft ist. Nach der Erstellung der Registerkarte werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="ada86-150">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ada86-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ada86-151">JSON representation</span></span>

<span data-ttu-id="ada86-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ada86-152">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="ada86-153">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ada86-153">See also</span></span>

[<span data-ttu-id="ada86-154">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="ada86-154">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
