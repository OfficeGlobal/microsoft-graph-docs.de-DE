---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
ms.openlocfilehash: f7e9351bc4a394005cffc712aa444c999a51b363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064934"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="1d811-102">Ressourcentyp itemActionStat</span><span class="sxs-lookup"><span data-stu-id="1d811-102">itemActionStat resource type</span></span>

> <span data-ttu-id="1d811-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d811-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d811-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d811-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d811-105">Die **ItemActionStat** Ressource enthält aggregierte Details über eine Aktion über einen Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="1d811-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d811-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d811-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a><span data-ttu-id="1d811-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d811-107">Properties</span></span>

| <span data-ttu-id="1d811-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d811-108">Property</span></span>    | <span data-ttu-id="1d811-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1d811-109">Type</span></span>  | <span data-ttu-id="1d811-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d811-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="1d811-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="1d811-111">actionCount</span></span> | <span data-ttu-id="1d811-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1d811-112">Int32</span></span> | <span data-ttu-id="1d811-113">Die Anzahl der Häufigkeit, mit die Aktion stattfand.</span><span class="sxs-lookup"><span data-stu-id="1d811-113">The number of times the action took place.</span></span> <span data-ttu-id="1d811-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1d811-114">Read-only.</span></span>
| <span data-ttu-id="1d811-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="1d811-115">actorCount</span></span>  | <span data-ttu-id="1d811-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1d811-116">Int32</span></span> | <span data-ttu-id="1d811-117">Die Anzahl der unterschiedlichen Akteure, die die Aktion ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1d811-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="1d811-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1d811-118">Read-only.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
