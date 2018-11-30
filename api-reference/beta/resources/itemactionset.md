---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
ms.openlocfilehash: 3b2f77ea21f2352b0a8fa647af84d9b0af08a2ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058456"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="e3a5e-102">ItemActionSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3a5e-102">ItemActionSet resource type</span></span>

> <span data-ttu-id="e3a5e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3a5e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3a5e-105">Die **ItemActionSet**-Ressource enthält Informationen zu den Aktionen, die eine [Aktivität][itemActivity] zu einem Element bilden.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e3a5e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3a5e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e3a5e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3a5e-107">Properties</span></span>

<span data-ttu-id="e3a5e-108">Nachstehend finden Sie die aktuell verfügbaren Aktionen.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="e3a5e-109">Zukünftig werden möglicherweise neue Aktionen protokolliert, vergewissern Sie sich deshalb, ob Ihre App die Toleranz vonn **itemActionSet** ohne Aktionen unterstützt, die Ihre App versteht.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="e3a5e-110">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="e3a5e-110">Property name</span></span> | <span data-ttu-id="e3a5e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e3a5e-111">Type</span></span>              | <span data-ttu-id="e3a5e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3a5e-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="e3a5e-113">Kommentar</span><span class="sxs-lookup"><span data-stu-id="e3a5e-113">comment</span></span>       | <span data-ttu-id="e3a5e-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-114">[commentAction][]</span></span> | <span data-ttu-id="e3a5e-115">Ein Kommentar wurde zu dem Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-115">A comment was added to the item.</span></span>
| <span data-ttu-id="e3a5e-116">create</span><span class="sxs-lookup"><span data-stu-id="e3a5e-116">create</span></span>        | <span data-ttu-id="e3a5e-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-117">[createAction][]</span></span>  | <span data-ttu-id="e3a5e-118">Ein Element wurde erstellt.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-118">An item was created.</span></span>
| <span data-ttu-id="e3a5e-119">Löschen</span><span class="sxs-lookup"><span data-stu-id="e3a5e-119">delete</span></span>        | <span data-ttu-id="e3a5e-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-120">[deleteAction][]</span></span>  | <span data-ttu-id="e3a5e-121">Ein Element wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-121">An item was deleted.</span></span>
| <span data-ttu-id="e3a5e-122">Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="e3a5e-122">edit</span></span>          | <span data-ttu-id="e3a5e-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-123">[editAction][]</span></span>    | <span data-ttu-id="e3a5e-124">Ein Element wurde bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-124">An item was edited.</span></span>
| <span data-ttu-id="e3a5e-125">Erwähnung</span><span class="sxs-lookup"><span data-stu-id="e3a5e-125">mention</span></span>       | <span data-ttu-id="e3a5e-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-126">[mentionAction][]</span></span> | <span data-ttu-id="e3a5e-127">Ein Benutzer wurde im Element erwähnt.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="e3a5e-128">verschieben</span><span class="sxs-lookup"><span data-stu-id="e3a5e-128">move</span></span>          | <span data-ttu-id="e3a5e-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-129">[moveAction][]</span></span>    | <span data-ttu-id="e3a5e-130">Ein Element wurde verschoben.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-130">An item was moved.</span></span>
| <span data-ttu-id="e3a5e-131">rename</span><span class="sxs-lookup"><span data-stu-id="e3a5e-131">rename</span></span>        | <span data-ttu-id="e3a5e-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-132">[renameAction][]</span></span>  | <span data-ttu-id="e3a5e-133">Ein Element wurde umbenannt.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-133">An item was renamed.</span></span>
| <span data-ttu-id="e3a5e-134">wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="e3a5e-134">restore</span></span>       | <span data-ttu-id="e3a5e-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-135">[restoreAction][]</span></span> | <span data-ttu-id="e3a5e-136">Ein Element wurde wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-136">An item was restored.</span></span>
| <span data-ttu-id="e3a5e-137">freigeben</span><span class="sxs-lookup"><span data-stu-id="e3a5e-137">share</span></span>         | <span data-ttu-id="e3a5e-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-138">[shareAction][]</span></span>   | <span data-ttu-id="e3a5e-139">Ein Element wurde freigegeben.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-139">An item was shared.</span></span>
| <span data-ttu-id="e3a5e-140">Version</span><span class="sxs-lookup"><span data-stu-id="e3a5e-140">version</span></span>       | <span data-ttu-id="e3a5e-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="e3a5e-141">[versionAction][]</span></span> | <span data-ttu-id="e3a5e-142">Ein Element wurde mit einer Versionsangabe versehen.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="e3a5e-153">Hinweise</span><span class="sxs-lookup"><span data-stu-id="e3a5e-153">Remarks</span></span>

<span data-ttu-id="e3a5e-154">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e3a5e-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
