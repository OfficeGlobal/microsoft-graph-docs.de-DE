---
title: Ressourcentyp teamsTab
description: 'Eine TeamsTab ist eine Registerkarte, hat fixiert an einen Kanal innerhalb eines Teams (angeschlossen). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574670"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="d148e-103">Ressourcentyp teamsTab</span><span class="sxs-lookup"><span data-stu-id="d148e-103">teamsTab resource type</span></span>



<span data-ttu-id="d148e-104">Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen).</span><span class="sxs-lookup"><span data-stu-id="d148e-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="d148e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d148e-105">Methods</span></span>

| <span data-ttu-id="d148e-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d148e-106">Method</span></span>       | <span data-ttu-id="d148e-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d148e-107">Return Type</span></span>  |<span data-ttu-id="d148e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d148e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d148e-109">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="d148e-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="d148e-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d148e-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d148e-111">Listen Registerkarten fixiert zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="d148e-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="d148e-112">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="d148e-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="d148e-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d148e-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d148e-114">Liest eine Registerkarte an einen Kanal fixiert.</span><span class="sxs-lookup"><span data-stu-id="d148e-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="d148e-115">Registerkarte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d148e-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="d148e-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d148e-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d148e-117">Fügt (Pins) einer Registerkarte zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="d148e-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="d148e-118">Registerkarte entfernen</span><span class="sxs-lookup"><span data-stu-id="d148e-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="d148e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="d148e-119">None</span></span> | <span data-ttu-id="d148e-120">Entfernt (löst) einer Registerkarte aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="d148e-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="d148e-121">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="d148e-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="d148e-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d148e-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d148e-123">Aktualisiert die Registerkarte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d148e-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="d148e-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d148e-124">Properties</span></span>

|<span data-ttu-id="d148e-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d148e-125">Property</span></span>|<span data-ttu-id="d148e-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d148e-126">Type</span></span>|<span data-ttu-id="d148e-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d148e-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="d148e-128">id</span><span class="sxs-lookup"><span data-stu-id="d148e-128">id</span></span>              |   <span data-ttu-id="d148e-129">string</span><span class="sxs-lookup"><span data-stu-id="d148e-129">string</span></span>                  |  <span data-ttu-id="d148e-130">Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.</span><span class="sxs-lookup"><span data-stu-id="d148e-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="d148e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d148e-131">displayName</span></span>            |   <span data-ttu-id="d148e-132">string</span><span class="sxs-lookup"><span data-stu-id="d148e-132">string</span></span>                  |  <span data-ttu-id="d148e-133">Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="d148e-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="d148e-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="d148e-134">webUrl</span></span>          |   <span data-ttu-id="d148e-135">string</span><span class="sxs-lookup"><span data-stu-id="d148e-135">string</span></span>                  |  <span data-ttu-id="d148e-136">Deep-Link-Url der Registerkarte-Instanz.</span><span class="sxs-lookup"><span data-stu-id="d148e-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="d148e-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d148e-137">Read only.</span></span>     |
|  <span data-ttu-id="d148e-138">Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d148e-138">configuration</span></span>        |   [<span data-ttu-id="d148e-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="d148e-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="d148e-140">Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="d148e-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="d148e-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d148e-141">Relationships</span></span>

| <span data-ttu-id="d148e-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d148e-142">Relationship</span></span> | <span data-ttu-id="d148e-143">Typ</span><span class="sxs-lookup"><span data-stu-id="d148e-143">Type</span></span>   | <span data-ttu-id="d148e-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d148e-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d148e-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d148e-145">teamsApp</span></span>|[<span data-ttu-id="d148e-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d148e-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d148e-147">Die Anwendung, die auf der Registerkarte verknüpft ist. Nach der Erstellung der Registerkarte werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="d148e-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d148e-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d148e-148">JSON representation</span></span>

<span data-ttu-id="d148e-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d148e-149">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
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

## <a name="see-also"></a><span data-ttu-id="d148e-150">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d148e-150">See also</span></span>

[<span data-ttu-id="d148e-151">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="d148e-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
