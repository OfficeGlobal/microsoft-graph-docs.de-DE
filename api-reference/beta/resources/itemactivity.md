---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemActivity
localization_priority: Normal
ms.openlocfilehash: 5e2be549c3e3e9e799449679b605577ecd782a94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517295"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="ed98b-102">ItemActivity-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ed98b-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed98b-103">Die **ItemActivity**-Ressource stellt Informationen zu Aktivitäten bereit, die zu einem Element oder innerhalb eines Containers stattfanden.</span><span class="sxs-lookup"><span data-stu-id="ed98b-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="ed98b-104">Zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ed98b-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed98b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed98b-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a><span data-ttu-id="ed98b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed98b-106">Properties</span></span>

| <span data-ttu-id="ed98b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed98b-107">Property</span></span> | <span data-ttu-id="ed98b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ed98b-108">Type</span></span>                    | <span data-ttu-id="ed98b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed98b-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="ed98b-110">id</span><span class="sxs-lookup"><span data-stu-id="ed98b-110">id</span></span>       | <span data-ttu-id="ed98b-111">string</span><span class="sxs-lookup"><span data-stu-id="ed98b-111">string</span></span>                  | <span data-ttu-id="ed98b-112">Der eindeutige Bezeichner der Aktivität.</span><span class="sxs-lookup"><span data-stu-id="ed98b-112">The unique identifier of the activity.</span></span> <span data-ttu-id="ed98b-113">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-113">Read-only.</span></span>
| <span data-ttu-id="ed98b-114">access</span><span class="sxs-lookup"><span data-stu-id="ed98b-114">access</span></span>   | <span data-ttu-id="ed98b-115">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-115">[accessAction][]</span></span>        | <span data-ttu-id="ed98b-116">Ein Element wurde zugegriffen.</span><span class="sxs-lookup"><span data-stu-id="ed98b-116">An item was accessed.</span></span>
| <span data-ttu-id="ed98b-117">Aktion</span><span class="sxs-lookup"><span data-stu-id="ed98b-117">action</span></span>   | <span data-ttu-id="ed98b-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-118">[itemActionSet][]</span></span>       | <span data-ttu-id="ed98b-119">Details zu der Aktion, die durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="ed98b-119">Details about the action that took place.</span></span> <span data-ttu-id="ed98b-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-120">Read-only.</span></span>
| <span data-ttu-id="ed98b-121">Akteur</span><span class="sxs-lookup"><span data-stu-id="ed98b-121">actor</span></span>    | <span data-ttu-id="ed98b-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-122">[identitySet][]</span></span>         | <span data-ttu-id="ed98b-123">Die Identität der Person, die die Aktion ausgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="ed98b-123">Identity of who performed the action.</span></span> <span data-ttu-id="ed98b-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-124">Read-only.</span></span>
| <span data-ttu-id="ed98b-125">location</span><span class="sxs-lookup"><span data-stu-id="ed98b-125">location</span></span> | <span data-ttu-id="ed98b-126">[location][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-126">[location][]</span></span>            | <span data-ttu-id="ed98b-127">Physischen Standort, auf dem die Aktion ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="ed98b-127">Physical location where the action was performed.</span></span> <span data-ttu-id="ed98b-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-128">Read-only.</span></span>
| <span data-ttu-id="ed98b-129">Mal</span><span class="sxs-lookup"><span data-stu-id="ed98b-129">times</span></span>    | <span data-ttu-id="ed98b-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="ed98b-131">Details zum Zeitpunkt der Ausführung der Aktivität.</span><span class="sxs-lookup"><span data-stu-id="ed98b-131">Details about when the activity took place.</span></span> <span data-ttu-id="ed98b-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="ed98b-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ed98b-136">Relationships</span></span>

| <span data-ttu-id="ed98b-137">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="ed98b-137">Relationship name</span></span> | <span data-ttu-id="ed98b-138">Typ</span><span class="sxs-lookup"><span data-stu-id="ed98b-138">Type</span></span>          | <span data-ttu-id="ed98b-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed98b-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="ed98b-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="ed98b-140">driveItem</span></span>         | <span data-ttu-id="ed98b-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-141">[driveItem][]</span></span> | <span data-ttu-id="ed98b-142">Macht das **DriveItem** verfügbar, das Ziel dieser Aktivität war.</span><span class="sxs-lookup"><span data-stu-id="ed98b-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="ed98b-143">listItem</span><span class="sxs-lookup"><span data-stu-id="ed98b-143">listItem</span></span>          | <span data-ttu-id="ed98b-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-144">[listItem][]</span></span>  | <span data-ttu-id="ed98b-145">Macht das **listItem** verfügbar, das Ziel dieser Aktivität war.</span><span class="sxs-lookup"><span data-stu-id="ed98b-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="ed98b-148">Aktionen</span><span class="sxs-lookup"><span data-stu-id="ed98b-148">Actions</span></span>

<span data-ttu-id="ed98b-149">Die Aktionen, die innerhalb einer Aktivität ausgeführt werden, sind detailliert in der **action**-Eigenschaft angegeben.</span><span class="sxs-lookup"><span data-stu-id="ed98b-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="ed98b-150">Nachstehend finden Sie die aktuell verfügbaren Aktionen.</span><span class="sxs-lookup"><span data-stu-id="ed98b-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="ed98b-151">Zukünftig werden möglicherweise neue Aktionen protokolliert, vergewissern Sie sich deshalb, ob Ihre App die Toleranz vonn **ItemActivity** ohne Aktionen unterstützt, die Ihre App versteht.</span><span class="sxs-lookup"><span data-stu-id="ed98b-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="ed98b-152">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="ed98b-152">Action name</span></span> | <span data-ttu-id="ed98b-153">Typ</span><span class="sxs-lookup"><span data-stu-id="ed98b-153">Type</span></span>              | <span data-ttu-id="ed98b-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed98b-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="ed98b-155">Kommentar</span><span class="sxs-lookup"><span data-stu-id="ed98b-155">comment</span></span>     | <span data-ttu-id="ed98b-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-156">[commentAction][]</span></span> | <span data-ttu-id="ed98b-157">Ein Kommentar wurde zu dem Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-157">A comment was added to the item.</span></span>
| <span data-ttu-id="ed98b-158">create</span><span class="sxs-lookup"><span data-stu-id="ed98b-158">create</span></span>      | <span data-ttu-id="ed98b-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-159">[createAction][]</span></span>  | <span data-ttu-id="ed98b-160">Ein Element wurde erstellt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-160">An item was created.</span></span>
| <span data-ttu-id="ed98b-161">Löschen</span><span class="sxs-lookup"><span data-stu-id="ed98b-161">delete</span></span>      | <span data-ttu-id="ed98b-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-162">[deleteAction][]</span></span>  | <span data-ttu-id="ed98b-163">Ein Element wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="ed98b-163">An item was deleted.</span></span>
| <span data-ttu-id="ed98b-164">Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="ed98b-164">edit</span></span>        | <span data-ttu-id="ed98b-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-165">[editAction][]</span></span>    | <span data-ttu-id="ed98b-166">Ein Element wurde bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="ed98b-166">An item was edited.</span></span>
| <span data-ttu-id="ed98b-167">Erwähnung</span><span class="sxs-lookup"><span data-stu-id="ed98b-167">mention</span></span>     | <span data-ttu-id="ed98b-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-168">[mentionAction][]</span></span> | <span data-ttu-id="ed98b-169">Ein Benutzer wurde im Element erwähnt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="ed98b-170">verschieben</span><span class="sxs-lookup"><span data-stu-id="ed98b-170">move</span></span>        | <span data-ttu-id="ed98b-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-171">[moveAction][]</span></span>    | <span data-ttu-id="ed98b-172">Ein Element wurde verschoben.</span><span class="sxs-lookup"><span data-stu-id="ed98b-172">An item was moved.</span></span>
| <span data-ttu-id="ed98b-173">rename</span><span class="sxs-lookup"><span data-stu-id="ed98b-173">rename</span></span>      | <span data-ttu-id="ed98b-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-174">[renameAction][]</span></span>  | <span data-ttu-id="ed98b-175">Ein Element wurde umbenannt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-175">An item was renamed.</span></span>
| <span data-ttu-id="ed98b-176">wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="ed98b-176">restore</span></span>     | <span data-ttu-id="ed98b-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-177">[restoreAction][]</span></span> | <span data-ttu-id="ed98b-178">Ein Element wurde wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="ed98b-178">An item was restored.</span></span>
| <span data-ttu-id="ed98b-179">freigeben</span><span class="sxs-lookup"><span data-stu-id="ed98b-179">share</span></span>       | <span data-ttu-id="ed98b-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-180">[shareAction][]</span></span>   | <span data-ttu-id="ed98b-181">Ein Element wurde freigegeben.</span><span class="sxs-lookup"><span data-stu-id="ed98b-181">An item was shared.</span></span>
| <span data-ttu-id="ed98b-182">Version</span><span class="sxs-lookup"><span data-stu-id="ed98b-182">version</span></span>     | <span data-ttu-id="ed98b-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="ed98b-183">[versionAction][]</span></span> | <span data-ttu-id="ed98b-184">Ein Element wurde mit einer Versionsangabe versehen.</span><span class="sxs-lookup"><span data-stu-id="ed98b-184">An item was versioned.</span></span>

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="ed98b-197">Hinweise</span><span class="sxs-lookup"><span data-stu-id="ed98b-197">Remarks</span></span>

<span data-ttu-id="ed98b-198">**ItemActivity** ist zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ed98b-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
