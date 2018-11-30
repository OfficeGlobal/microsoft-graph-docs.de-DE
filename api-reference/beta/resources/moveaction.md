---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
ms.openlocfilehash: d31cfc9a45b83f74058073ca18ca2df15a9914ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058921"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="8ec4d-102">MoveAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8ec4d-102">MoveAction resource type</span></span>

> <span data-ttu-id="8ec4d-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ec4d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ec4d-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ec4d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ec4d-105">Wenn eine **MoveAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element verschoben hat.</span><span class="sxs-lookup"><span data-stu-id="8ec4d-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8ec4d-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ec4d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8ec4d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ec4d-107">Properties</span></span>

| <span data-ttu-id="8ec4d-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8ec4d-108">Property name</span></span> | <span data-ttu-id="8ec4d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8ec4d-109">Type</span></span>   | <span data-ttu-id="8ec4d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ec4d-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8ec4d-111">from</span><span class="sxs-lookup"><span data-stu-id="8ec4d-111">from</span></span>          | <span data-ttu-id="8ec4d-112">string</span><span class="sxs-lookup"><span data-stu-id="8ec4d-112">string</span></span> | <span data-ttu-id="8ec4d-113">Der Name des Speicherorts aus dem das Element verschoben wurde.</span><span class="sxs-lookup"><span data-stu-id="8ec4d-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="8ec4d-114">to</span><span class="sxs-lookup"><span data-stu-id="8ec4d-114">to</span></span>            | <span data-ttu-id="8ec4d-115">string</span><span class="sxs-lookup"><span data-stu-id="8ec4d-115">string</span></span> | <span data-ttu-id="8ec4d-116">Der Name des Speicherorts in den das Element verschoben wurde.</span><span class="sxs-lookup"><span data-stu-id="8ec4d-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="8ec4d-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="8ec4d-117">Remarks</span></span>

<span data-ttu-id="8ec4d-118">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8ec4d-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
