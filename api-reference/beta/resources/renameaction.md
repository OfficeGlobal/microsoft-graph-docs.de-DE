---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
ms.openlocfilehash: 12956ab51923f6d9f175b25203bf2921a64a8a6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061477"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="a4466-102">RenameAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a4466-102">RenameAction resource type</span></span>

> <span data-ttu-id="a4466-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a4466-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4466-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4466-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4466-105">Wenn die **RenameAction**-Ressource für ein [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element umbenannt hat.</span><span class="sxs-lookup"><span data-stu-id="a4466-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a4466-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a4466-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a4466-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a4466-107">Properties</span></span>

| <span data-ttu-id="a4466-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="a4466-108">Property name</span></span> | <span data-ttu-id="a4466-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a4466-109">Type</span></span>   | <span data-ttu-id="a4466-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4466-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a4466-111">oldName</span><span class="sxs-lookup"><span data-stu-id="a4466-111">oldName</span></span>       | <span data-ttu-id="a4466-112">string</span><span class="sxs-lookup"><span data-stu-id="a4466-112">string</span></span> | <span data-ttu-id="a4466-113">Der vorherige Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="a4466-113">The previous name of the item.</span></span>
| <span data-ttu-id="a4466-114">newName</span><span class="sxs-lookup"><span data-stu-id="a4466-114">newName</span></span>       | <span data-ttu-id="a4466-115">string</span><span class="sxs-lookup"><span data-stu-id="a4466-115">string</span></span> | <span data-ttu-id="a4466-116">Der neue Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="a4466-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="a4466-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="a4466-117">Remarks</span></span>

<span data-ttu-id="a4466-118">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a4466-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
