---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: a29bdad0ae5e06d3d1b55f1fb7ceb630bec1b564
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819670"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="60c84-102">ItemActivity-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60c84-102">ItemActivity resource type</span></span>

> <span data-ttu-id="60c84-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60c84-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60c84-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60c84-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60c84-105">Die **ItemActivity**-Ressource stellt Informationen zu Aktivitäten bereit, die zu einem Element oder innerhalb eines Containers stattfanden.</span><span class="sxs-lookup"><span data-stu-id="60c84-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="60c84-106">Zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="60c84-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60c84-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60c84-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="60c84-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60c84-108">Properties</span></span>

| <span data-ttu-id="60c84-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60c84-109">Property</span></span> | <span data-ttu-id="60c84-110">Typ</span><span class="sxs-lookup"><span data-stu-id="60c84-110">Type</span></span>                    | <span data-ttu-id="60c84-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60c84-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="60c84-112">id</span><span class="sxs-lookup"><span data-stu-id="60c84-112">id</span></span>       | <span data-ttu-id="60c84-113">string</span><span class="sxs-lookup"><span data-stu-id="60c84-113">string</span></span>                  | <span data-ttu-id="60c84-114">Der eindeutige Bezeichner der Aktivität.</span><span class="sxs-lookup"><span data-stu-id="60c84-114">The unique identifier of the activity.</span></span> <span data-ttu-id="60c84-115">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="60c84-115">Read-only.</span></span>
| <span data-ttu-id="60c84-116">access</span><span class="sxs-lookup"><span data-stu-id="60c84-116">access</span></span>   | <span data-ttu-id="60c84-117">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-117">[accessAction][]</span></span>        | <span data-ttu-id="60c84-118">Ein Element wurde zugegriffen.</span><span class="sxs-lookup"><span data-stu-id="60c84-118">An item was accessed.</span></span>
| <span data-ttu-id="60c84-119">Aktion</span><span class="sxs-lookup"><span data-stu-id="60c84-119">action</span></span>   | <span data-ttu-id="60c84-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="60c84-120">[itemActionSet][]</span></span>       | <span data-ttu-id="60c84-121">Details zu der Aktion, die durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="60c84-121">Details about the action that took place.</span></span> <span data-ttu-id="60c84-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="60c84-122">Read-only.</span></span>
| <span data-ttu-id="60c84-123">Akteur</span><span class="sxs-lookup"><span data-stu-id="60c84-123">actor</span></span>    | <span data-ttu-id="60c84-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="60c84-124">[identitySet][]</span></span>         | <span data-ttu-id="60c84-125">Die Identität der Person, die die Aktion ausgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="60c84-125">Identity of who performed the action.</span></span> <span data-ttu-id="60c84-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="60c84-126">Read-only.</span></span>
| <span data-ttu-id="60c84-127">location</span><span class="sxs-lookup"><span data-stu-id="60c84-127">location</span></span> | <span data-ttu-id="60c84-128">[location][]</span><span class="sxs-lookup"><span data-stu-id="60c84-128">[location][]</span></span>            | <span data-ttu-id="60c84-129">Physischen Standort, auf dem die Aktion ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="60c84-129">Physical location where the action was performed.</span></span> <span data-ttu-id="60c84-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="60c84-130">Read-only.</span></span>
| <span data-ttu-id="60c84-131">Mal</span><span class="sxs-lookup"><span data-stu-id="60c84-131">times</span></span>    | <span data-ttu-id="60c84-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="60c84-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="60c84-133">Details zum Zeitpunkt der Ausführung der Aktivität.</span><span class="sxs-lookup"><span data-stu-id="60c84-133">Details about when the activity took place.</span></span> <span data-ttu-id="60c84-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="60c84-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="60c84-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="60c84-138">Relationships</span></span>

| <span data-ttu-id="60c84-139">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="60c84-139">Relationship name</span></span> | <span data-ttu-id="60c84-140">Typ</span><span class="sxs-lookup"><span data-stu-id="60c84-140">Type</span></span>          | <span data-ttu-id="60c84-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60c84-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="60c84-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="60c84-142">driveItem</span></span>         | <span data-ttu-id="60c84-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="60c84-143">[driveItem][]</span></span> | <span data-ttu-id="60c84-144">Macht das **DriveItem** verfügbar, das Ziel dieser Aktivität war.</span><span class="sxs-lookup"><span data-stu-id="60c84-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="60c84-145">listItem</span><span class="sxs-lookup"><span data-stu-id="60c84-145">listItem</span></span>          | <span data-ttu-id="60c84-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="60c84-146">[listItem][]</span></span>  | <span data-ttu-id="60c84-147">Macht das **listItem** verfügbar, das Ziel dieser Aktivität war.</span><span class="sxs-lookup"><span data-stu-id="60c84-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="60c84-150">Aktionen</span><span class="sxs-lookup"><span data-stu-id="60c84-150">Actions</span></span>

<span data-ttu-id="60c84-151">Die Aktionen, die innerhalb einer Aktivität ausgeführt werden, sind detailliert in der **action**-Eigenschaft angegeben.</span><span class="sxs-lookup"><span data-stu-id="60c84-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="60c84-152">Nachstehend finden Sie die aktuell verfügbaren Aktionen.</span><span class="sxs-lookup"><span data-stu-id="60c84-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="60c84-153">Zukünftig werden möglicherweise neue Aktionen protokolliert, vergewissern Sie sich deshalb, ob Ihre App die Toleranz vonn **ItemActivity** ohne Aktionen unterstützt, die Ihre App versteht.</span><span class="sxs-lookup"><span data-stu-id="60c84-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="60c84-154">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="60c84-154">Action name</span></span> | <span data-ttu-id="60c84-155">Typ</span><span class="sxs-lookup"><span data-stu-id="60c84-155">Type</span></span>              | <span data-ttu-id="60c84-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60c84-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="60c84-157">Kommentar</span><span class="sxs-lookup"><span data-stu-id="60c84-157">comment</span></span>     | <span data-ttu-id="60c84-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-158">[commentAction][]</span></span> | <span data-ttu-id="60c84-159">Ein Kommentar wurde zu dem Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60c84-159">A comment was added to the item.</span></span>
| <span data-ttu-id="60c84-160">create</span><span class="sxs-lookup"><span data-stu-id="60c84-160">create</span></span>      | <span data-ttu-id="60c84-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-161">[createAction][]</span></span>  | <span data-ttu-id="60c84-162">Ein Element wurde erstellt.</span><span class="sxs-lookup"><span data-stu-id="60c84-162">An item was created.</span></span>
| <span data-ttu-id="60c84-163">Löschen</span><span class="sxs-lookup"><span data-stu-id="60c84-163">delete</span></span>      | <span data-ttu-id="60c84-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-164">[deleteAction][]</span></span>  | <span data-ttu-id="60c84-165">Ein Element wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="60c84-165">An item was deleted.</span></span>
| <span data-ttu-id="60c84-166">Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="60c84-166">edit</span></span>        | <span data-ttu-id="60c84-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-167">[editAction][]</span></span>    | <span data-ttu-id="60c84-168">Ein Element wurde bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="60c84-168">An item was edited.</span></span>
| <span data-ttu-id="60c84-169">Erwähnung</span><span class="sxs-lookup"><span data-stu-id="60c84-169">mention</span></span>     | <span data-ttu-id="60c84-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-170">[mentionAction][]</span></span> | <span data-ttu-id="60c84-171">Ein Benutzer wurde im Element erwähnt.</span><span class="sxs-lookup"><span data-stu-id="60c84-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="60c84-172">verschieben</span><span class="sxs-lookup"><span data-stu-id="60c84-172">move</span></span>        | <span data-ttu-id="60c84-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-173">[moveAction][]</span></span>    | <span data-ttu-id="60c84-174">Ein Element wurde verschoben.</span><span class="sxs-lookup"><span data-stu-id="60c84-174">An item was moved.</span></span>
| <span data-ttu-id="60c84-175">rename</span><span class="sxs-lookup"><span data-stu-id="60c84-175">rename</span></span>      | <span data-ttu-id="60c84-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-176">[renameAction][]</span></span>  | <span data-ttu-id="60c84-177">Ein Element wurde umbenannt.</span><span class="sxs-lookup"><span data-stu-id="60c84-177">An item was renamed.</span></span>
| <span data-ttu-id="60c84-178">wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="60c84-178">restore</span></span>     | <span data-ttu-id="60c84-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-179">[restoreAction][]</span></span> | <span data-ttu-id="60c84-180">Ein Element wurde wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="60c84-180">An item was restored.</span></span>
| <span data-ttu-id="60c84-181">freigeben</span><span class="sxs-lookup"><span data-stu-id="60c84-181">share</span></span>       | <span data-ttu-id="60c84-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-182">[shareAction][]</span></span>   | <span data-ttu-id="60c84-183">Ein Element wurde freigegeben.</span><span class="sxs-lookup"><span data-stu-id="60c84-183">An item was shared.</span></span>
| <span data-ttu-id="60c84-184">Version</span><span class="sxs-lookup"><span data-stu-id="60c84-184">version</span></span>     | <span data-ttu-id="60c84-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="60c84-185">[versionAction][]</span></span> | <span data-ttu-id="60c84-186">Ein Element wurde mit einer Versionsangabe versehen.</span><span class="sxs-lookup"><span data-stu-id="60c84-186">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="60c84-199">Hinweise</span><span class="sxs-lookup"><span data-stu-id="60c84-199">Remarks</span></span>

<span data-ttu-id="60c84-200">**ItemActivity** ist zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="60c84-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
