---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515468"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="65fb1-102">RenameAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="65fb1-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65fb1-103">Wenn die **RenameAction**-Ressource für ein [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element umbenannt hat.</span><span class="sxs-lookup"><span data-stu-id="65fb1-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="65fb1-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65fb1-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

## <a name="properties"></a><span data-ttu-id="65fb1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65fb1-105">Properties</span></span>

| <span data-ttu-id="65fb1-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="65fb1-106">Property name</span></span> | <span data-ttu-id="65fb1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="65fb1-107">Type</span></span>   | <span data-ttu-id="65fb1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65fb1-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="65fb1-109">oldName</span><span class="sxs-lookup"><span data-stu-id="65fb1-109">oldName</span></span>       | <span data-ttu-id="65fb1-110">string</span><span class="sxs-lookup"><span data-stu-id="65fb1-110">string</span></span> | <span data-ttu-id="65fb1-111">Der vorherige Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="65fb1-111">The previous name of the item.</span></span>
| <span data-ttu-id="65fb1-112">newname</span><span class="sxs-lookup"><span data-stu-id="65fb1-112">newName</span></span>       | <span data-ttu-id="65fb1-113">string</span><span class="sxs-lookup"><span data-stu-id="65fb1-113">string</span></span> | <span data-ttu-id="65fb1-114">Der neue Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="65fb1-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="65fb1-115">Hinweise</span><span class="sxs-lookup"><span data-stu-id="65fb1-115">Remarks</span></span>

<span data-ttu-id="65fb1-116">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="65fb1-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/renameaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
