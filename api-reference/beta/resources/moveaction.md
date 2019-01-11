---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 40049b506c72af5aacddf461b22e1ddd280d7ad4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852899"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="81527-102">MoveAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81527-102">MoveAction resource type</span></span>

> <span data-ttu-id="81527-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81527-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81527-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81527-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81527-105">Wenn eine **MoveAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element verschoben hat.</span><span class="sxs-lookup"><span data-stu-id="81527-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="81527-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81527-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

## <a name="properties"></a><span data-ttu-id="81527-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81527-107">Properties</span></span>

| <span data-ttu-id="81527-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="81527-108">Property name</span></span> | <span data-ttu-id="81527-109">Typ</span><span class="sxs-lookup"><span data-stu-id="81527-109">Type</span></span>   | <span data-ttu-id="81527-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81527-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="81527-111">from</span><span class="sxs-lookup"><span data-stu-id="81527-111">from</span></span>          | <span data-ttu-id="81527-112">string</span><span class="sxs-lookup"><span data-stu-id="81527-112">string</span></span> | <span data-ttu-id="81527-113">Der Name des Speicherorts aus dem das Element verschoben wurde.</span><span class="sxs-lookup"><span data-stu-id="81527-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="81527-114">to</span><span class="sxs-lookup"><span data-stu-id="81527-114">to</span></span>            | <span data-ttu-id="81527-115">string</span><span class="sxs-lookup"><span data-stu-id="81527-115">string</span></span> | <span data-ttu-id="81527-116">Der Name des Speicherorts in den das Element verschoben wurde.</span><span class="sxs-lookup"><span data-stu-id="81527-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="81527-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="81527-117">Remarks</span></span>

<span data-ttu-id="81527-118">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="81527-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
