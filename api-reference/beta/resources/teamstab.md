---
title: Ressourcentyp teamsTab
description: 'Eine TeamsTab ist eine Registerkarte, hat fixiert an einen Kanal innerhalb eines Teams (angeschlossen). '
ms.openlocfilehash: 102d4c0b766d8a0d9bdf22cb2ed76f5e06d87ad5
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283619"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="908bb-103">Ressourcentyp teamsTab</span><span class="sxs-lookup"><span data-stu-id="908bb-103">teamsTab resource type</span></span>

> <span data-ttu-id="908bb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="908bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="908bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="908bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="908bb-106">Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen).</span><span class="sxs-lookup"><span data-stu-id="908bb-106">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="908bb-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="908bb-107">Methods</span></span>

| <span data-ttu-id="908bb-108">Methode</span><span class="sxs-lookup"><span data-stu-id="908bb-108">Method</span></span>       | <span data-ttu-id="908bb-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="908bb-109">Return Type</span></span>  |<span data-ttu-id="908bb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="908bb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="908bb-111">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="908bb-111">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="908bb-112">teamsTab</span><span class="sxs-lookup"><span data-stu-id="908bb-112">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="908bb-113">Listen Registerkarten fixiert zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="908bb-113">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="908bb-114">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="908bb-114">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="908bb-115">teamsTab</span><span class="sxs-lookup"><span data-stu-id="908bb-115">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="908bb-116">Liest eine Registerkarte an einen Kanal fixiert.</span><span class="sxs-lookup"><span data-stu-id="908bb-116">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="908bb-117">Registerkarte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="908bb-117">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="908bb-118">teamsTab</span><span class="sxs-lookup"><span data-stu-id="908bb-118">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="908bb-119">Fügt (Pins) einer Registerkarte zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="908bb-119">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="908bb-120">Registerkarte entfernen</span><span class="sxs-lookup"><span data-stu-id="908bb-120">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="908bb-121">Keines</span><span class="sxs-lookup"><span data-stu-id="908bb-121">None</span></span> | <span data-ttu-id="908bb-122">Entfernt (löst) einer Registerkarte aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="908bb-122">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="908bb-123">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="908bb-123">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="908bb-124">teamsTab</span><span class="sxs-lookup"><span data-stu-id="908bb-124">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="908bb-125">Aktualisiert die Registerkarte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="908bb-125">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="908bb-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="908bb-126">Properties</span></span>

|<span data-ttu-id="908bb-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="908bb-127">Property</span></span>|<span data-ttu-id="908bb-128">Typ</span><span class="sxs-lookup"><span data-stu-id="908bb-128">Type</span></span>|<span data-ttu-id="908bb-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="908bb-129">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="908bb-130">id</span><span class="sxs-lookup"><span data-stu-id="908bb-130">id</span></span>              |   <span data-ttu-id="908bb-131">string</span><span class="sxs-lookup"><span data-stu-id="908bb-131">string</span></span>                  |  <span data-ttu-id="908bb-132">Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.</span><span class="sxs-lookup"><span data-stu-id="908bb-132">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="908bb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="908bb-133">displayName</span></span>            |   <span data-ttu-id="908bb-134">string</span><span class="sxs-lookup"><span data-stu-id="908bb-134">string</span></span>                  |  <span data-ttu-id="908bb-135">Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="908bb-135">Name of the tab.</span></span>     |
|  <span data-ttu-id="908bb-136">name</span><span class="sxs-lookup"><span data-stu-id="908bb-136">name</span></span>            |   <span data-ttu-id="908bb-137">string</span><span class="sxs-lookup"><span data-stu-id="908bb-137">string</span></span>                  |  <span data-ttu-id="908bb-138">(Veraltet) Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="908bb-138">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="908bb-139">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="908bb-139">teamsAppId</span></span>           |   <span data-ttu-id="908bb-140">string</span><span class="sxs-lookup"><span data-stu-id="908bb-140">string</span></span>             |  <span data-ttu-id="908bb-141">App-Definition-Bezeichner der Registerkarte. Dieser Wert kann nach der Erstellung der Registerkarte geändert werden.</span><span class="sxs-lookup"><span data-stu-id="908bb-141">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="908bb-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="908bb-142">sortOrderIndex</span></span>  |   <span data-ttu-id="908bb-143">Int</span><span class="sxs-lookup"><span data-stu-id="908bb-143">int</span></span>                     |  <span data-ttu-id="908bb-144">Index der Reihenfolge für die Sortierung von Registerkarten verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="908bb-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="908bb-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="908bb-145">webUrl</span></span>          |   <span data-ttu-id="908bb-146">string</span><span class="sxs-lookup"><span data-stu-id="908bb-146">string</span></span>                  |  <span data-ttu-id="908bb-147">Deep-Link-Url der Registerkarte-Instanz.</span><span class="sxs-lookup"><span data-stu-id="908bb-147">Deep link url of the tab instance.</span></span> <span data-ttu-id="908bb-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="908bb-148">Read only.</span></span>     |
|  <span data-ttu-id="908bb-149">Konfiguration</span><span class="sxs-lookup"><span data-stu-id="908bb-149">configuration</span></span>        |   [<span data-ttu-id="908bb-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="908bb-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="908bb-151">Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="908bb-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="908bb-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="908bb-152">Relationships</span></span>

| <span data-ttu-id="908bb-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="908bb-153">Relationship</span></span> | <span data-ttu-id="908bb-154">Typ</span><span class="sxs-lookup"><span data-stu-id="908bb-154">Type</span></span>   | <span data-ttu-id="908bb-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="908bb-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="908bb-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="908bb-156">teamsApp</span></span>|[<span data-ttu-id="908bb-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="908bb-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="908bb-158">Die Anwendung, die auf der Registerkarte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="908bb-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="908bb-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="908bb-159">JSON representation</span></span>

<span data-ttu-id="908bb-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="908bb-160">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
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

## <a name="see-also"></a><span data-ttu-id="908bb-161">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="908bb-161">See also</span></span>

[<span data-ttu-id="908bb-162">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="908bb-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
