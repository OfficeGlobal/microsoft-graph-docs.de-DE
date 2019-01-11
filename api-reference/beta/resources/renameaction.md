---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: 88fa2738c014f028ebd2cc6e37f83151c7fc984a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835707"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="c2259-102">RenameAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c2259-102">RenameAction resource type</span></span>

> <span data-ttu-id="c2259-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c2259-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2259-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2259-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2259-105">Wenn die **RenameAction**-Ressource für ein [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element umbenannt hat.</span><span class="sxs-lookup"><span data-stu-id="c2259-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c2259-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c2259-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2259-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c2259-107">Properties</span></span>

| <span data-ttu-id="c2259-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="c2259-108">Property name</span></span> | <span data-ttu-id="c2259-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c2259-109">Type</span></span>   | <span data-ttu-id="c2259-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2259-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c2259-111">oldName</span><span class="sxs-lookup"><span data-stu-id="c2259-111">oldName</span></span>       | <span data-ttu-id="c2259-112">string</span><span class="sxs-lookup"><span data-stu-id="c2259-112">string</span></span> | <span data-ttu-id="c2259-113">Der vorherige Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="c2259-113">The previous name of the item.</span></span>
| <span data-ttu-id="c2259-114">newName</span><span class="sxs-lookup"><span data-stu-id="c2259-114">newName</span></span>       | <span data-ttu-id="c2259-115">string</span><span class="sxs-lookup"><span data-stu-id="c2259-115">string</span></span> | <span data-ttu-id="c2259-116">Der neue Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="c2259-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="c2259-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="c2259-117">Remarks</span></span>

<span data-ttu-id="c2259-118">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c2259-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
