---
title: Ressourcentyp teamsTab
description: 'Eine TeamsTab ist eine Registerkarte, hat fixiert an einen Kanal innerhalb eines Teams (angeschlossen). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2db59065f139e2e704c3394f7afb82cba91c33fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509287"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="6e95d-103">Ressourcentyp teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e95d-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e95d-104">Eine TeamsTab ist eine [Registerkarte](../resources/teamstab.md) , hat fixiert an einen [DDE-Kanal](channel.md) in einem [Team](team.md)(angeschlossen).</span><span class="sxs-lookup"><span data-stu-id="6e95d-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="6e95d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="6e95d-105">Methods</span></span>

| <span data-ttu-id="6e95d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="6e95d-106">Method</span></span>       | <span data-ttu-id="6e95d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6e95d-107">Return Type</span></span>  |<span data-ttu-id="6e95d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e95d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e95d-109">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="6e95d-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="6e95d-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e95d-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e95d-111">Listen Registerkarten fixiert zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="6e95d-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="6e95d-112">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="6e95d-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="6e95d-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e95d-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e95d-114">Liest eine Registerkarte an einen Kanal fixiert.</span><span class="sxs-lookup"><span data-stu-id="6e95d-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="6e95d-115">Registerkarte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="6e95d-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="6e95d-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e95d-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e95d-117">Fügt (Pins) einer Registerkarte zu einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="6e95d-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="6e95d-118">Registerkarte entfernen</span><span class="sxs-lookup"><span data-stu-id="6e95d-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="6e95d-119">Keine</span><span class="sxs-lookup"><span data-stu-id="6e95d-119">None</span></span> | <span data-ttu-id="6e95d-120">Entfernt (löst) einer Registerkarte aus einem Kanal.</span><span class="sxs-lookup"><span data-stu-id="6e95d-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="6e95d-121">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="6e95d-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="6e95d-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e95d-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e95d-123">Aktualisiert die Registerkarte Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="6e95d-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="6e95d-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6e95d-124">Properties</span></span>

|<span data-ttu-id="6e95d-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6e95d-125">Property</span></span>|<span data-ttu-id="6e95d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="6e95d-126">Type</span></span>|<span data-ttu-id="6e95d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e95d-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="6e95d-128">id</span><span class="sxs-lookup"><span data-stu-id="6e95d-128">id</span></span>              |   <span data-ttu-id="6e95d-129">string</span><span class="sxs-lookup"><span data-stu-id="6e95d-129">string</span></span>                  |  <span data-ttu-id="6e95d-130">Bezeichner, die eine bestimmte Instanz von einer DDE-Kanal Registerkarte Lesen nur eindeutig identifiziert.</span><span class="sxs-lookup"><span data-stu-id="6e95d-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="6e95d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6e95d-131">displayName</span></span>            |   <span data-ttu-id="6e95d-132">string</span><span class="sxs-lookup"><span data-stu-id="6e95d-132">string</span></span>                  |  <span data-ttu-id="6e95d-133">Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="6e95d-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="6e95d-134">name</span><span class="sxs-lookup"><span data-stu-id="6e95d-134">name</span></span>            |   <span data-ttu-id="6e95d-135">string</span><span class="sxs-lookup"><span data-stu-id="6e95d-135">string</span></span>                  |  <span data-ttu-id="6e95d-136">(Veraltet) Der Name der Registerkarte.</span><span class="sxs-lookup"><span data-stu-id="6e95d-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="6e95d-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="6e95d-137">teamsAppId</span></span>           |   <span data-ttu-id="6e95d-138">string</span><span class="sxs-lookup"><span data-stu-id="6e95d-138">string</span></span>             |  <span data-ttu-id="6e95d-139">App-Definition-Bezeichner der Registerkarte. Dieser Wert kann nach der Erstellung der Registerkarte geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6e95d-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="6e95d-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="6e95d-140">sortOrderIndex</span></span>  |   <span data-ttu-id="6e95d-141">int</span><span class="sxs-lookup"><span data-stu-id="6e95d-141">int</span></span>                     |  <span data-ttu-id="6e95d-142">Index der Reihenfolge für die Sortierung von Registerkarten verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="6e95d-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="6e95d-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="6e95d-143">webUrl</span></span>          |   <span data-ttu-id="6e95d-144">string</span><span class="sxs-lookup"><span data-stu-id="6e95d-144">string</span></span>                  |  <span data-ttu-id="6e95d-145">Deep-Link-Url der Registerkarte-Instanz.</span><span class="sxs-lookup"><span data-stu-id="6e95d-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="6e95d-146">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6e95d-146">Read only.</span></span>     |
|  <span data-ttu-id="6e95d-147">Konfiguration</span><span class="sxs-lookup"><span data-stu-id="6e95d-147">configuration</span></span>        |   [<span data-ttu-id="6e95d-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e95d-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="6e95d-149">Container für benutzerdefinierte Einstellungen angewendet auf die Registerkarte an. Die Registerkarte gilt nur, wenn diese Eigenschaft festgelegt ist konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="6e95d-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="6e95d-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6e95d-150">Relationships</span></span>

| <span data-ttu-id="6e95d-151">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6e95d-151">Relationship</span></span> | <span data-ttu-id="6e95d-152">Typ</span><span class="sxs-lookup"><span data-stu-id="6e95d-152">Type</span></span>   | <span data-ttu-id="6e95d-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e95d-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6e95d-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6e95d-154">teamsApp</span></span>|[<span data-ttu-id="6e95d-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6e95d-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="6e95d-156">Die Anwendung, die auf der Registerkarte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="6e95d-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e95d-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6e95d-157">JSON representation</span></span>

<span data-ttu-id="6e95d-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6e95d-158">The following is a JSON representation of the resource.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="6e95d-159">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6e95d-159">See also</span></span>

[<span data-ttu-id="6e95d-160">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="6e95d-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
