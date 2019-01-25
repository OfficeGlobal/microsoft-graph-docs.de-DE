---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: 3fab75c6a63630f57dae8d0578691ba10622231d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518800"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="08ce0-102">ItemActionSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08ce0-102">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08ce0-103">Die **ItemActionSet**-Ressource enthält Informationen zu den Aktionen, die eine [Aktivität][itemActivity] zu einem Element bilden.</span><span class="sxs-lookup"><span data-stu-id="08ce0-103">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="08ce0-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08ce0-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

## <a name="properties"></a><span data-ttu-id="08ce0-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08ce0-105">Properties</span></span>

<span data-ttu-id="08ce0-106">Nachstehend finden Sie die aktuell verfügbaren Aktionen.</span><span class="sxs-lookup"><span data-stu-id="08ce0-106">Below are the actions that are available today.</span></span>
<span data-ttu-id="08ce0-107">Zukünftig werden möglicherweise neue Aktionen protokolliert, vergewissern Sie sich deshalb, ob Ihre App die Toleranz vonn **itemActionSet** ohne Aktionen unterstützt, die Ihre App versteht.</span><span class="sxs-lookup"><span data-stu-id="08ce0-107">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="08ce0-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="08ce0-108">Property name</span></span> | <span data-ttu-id="08ce0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="08ce0-109">Type</span></span>              | <span data-ttu-id="08ce0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08ce0-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="08ce0-111">Kommentar</span><span class="sxs-lookup"><span data-stu-id="08ce0-111">comment</span></span>       | <span data-ttu-id="08ce0-112">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-112">[commentAction][]</span></span> | <span data-ttu-id="08ce0-113">Ein Kommentar wurde zu dem Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08ce0-113">A comment was added to the item.</span></span>
| <span data-ttu-id="08ce0-114">create</span><span class="sxs-lookup"><span data-stu-id="08ce0-114">create</span></span>        | <span data-ttu-id="08ce0-115">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-115">[createAction][]</span></span>  | <span data-ttu-id="08ce0-116">Ein Element wurde erstellt.</span><span class="sxs-lookup"><span data-stu-id="08ce0-116">An item was created.</span></span>
| <span data-ttu-id="08ce0-117">Löschen</span><span class="sxs-lookup"><span data-stu-id="08ce0-117">delete</span></span>        | <span data-ttu-id="08ce0-118">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-118">[deleteAction][]</span></span>  | <span data-ttu-id="08ce0-119">Ein Element wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="08ce0-119">An item was deleted.</span></span>
| <span data-ttu-id="08ce0-120">Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="08ce0-120">edit</span></span>          | <span data-ttu-id="08ce0-121">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-121">[editAction][]</span></span>    | <span data-ttu-id="08ce0-122">Ein Element wurde bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="08ce0-122">An item was edited.</span></span>
| <span data-ttu-id="08ce0-123">Erwähnung</span><span class="sxs-lookup"><span data-stu-id="08ce0-123">mention</span></span>       | <span data-ttu-id="08ce0-124">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-124">[mentionAction][]</span></span> | <span data-ttu-id="08ce0-125">Ein Benutzer wurde im Element erwähnt.</span><span class="sxs-lookup"><span data-stu-id="08ce0-125">A user was mentioned in the item.</span></span>
| <span data-ttu-id="08ce0-126">verschieben</span><span class="sxs-lookup"><span data-stu-id="08ce0-126">move</span></span>          | <span data-ttu-id="08ce0-127">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-127">[moveAction][]</span></span>    | <span data-ttu-id="08ce0-128">Ein Element wurde verschoben.</span><span class="sxs-lookup"><span data-stu-id="08ce0-128">An item was moved.</span></span>
| <span data-ttu-id="08ce0-129">rename</span><span class="sxs-lookup"><span data-stu-id="08ce0-129">rename</span></span>        | <span data-ttu-id="08ce0-130">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-130">[renameAction][]</span></span>  | <span data-ttu-id="08ce0-131">Ein Element wurde umbenannt.</span><span class="sxs-lookup"><span data-stu-id="08ce0-131">An item was renamed.</span></span>
| <span data-ttu-id="08ce0-132">wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="08ce0-132">restore</span></span>       | <span data-ttu-id="08ce0-133">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-133">[restoreAction][]</span></span> | <span data-ttu-id="08ce0-134">Ein Element wurde wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="08ce0-134">An item was restored.</span></span>
| <span data-ttu-id="08ce0-135">freigeben</span><span class="sxs-lookup"><span data-stu-id="08ce0-135">share</span></span>         | <span data-ttu-id="08ce0-136">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-136">[shareAction][]</span></span>   | <span data-ttu-id="08ce0-137">Ein Element wurde freigegeben.</span><span class="sxs-lookup"><span data-stu-id="08ce0-137">An item was shared.</span></span>
| <span data-ttu-id="08ce0-138">Version</span><span class="sxs-lookup"><span data-stu-id="08ce0-138">version</span></span>       | <span data-ttu-id="08ce0-139">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="08ce0-139">[versionAction][]</span></span> | <span data-ttu-id="08ce0-140">Ein Element wurde mit einer Versionsangabe versehen.</span><span class="sxs-lookup"><span data-stu-id="08ce0-140">An item was versioned.</span></span>

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="08ce0-151">Hinweise</span><span class="sxs-lookup"><span data-stu-id="08ce0-151">Remarks</span></span>

<span data-ttu-id="08ce0-152">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="08ce0-152">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactionset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
