---
title: Ressourcentyp targetResourcePolicy
description: 'Gibt die Richtlinie, die von der Aktivität Audit betroffen war. Die Ressource TargetResource abgeleitet.   '
localization_priority: Normal
ms.openlocfilehash: 355e6ac11741a2aa7aeb780bdac4b7be373092af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813139"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="e18ec-104">Ressourcentyp targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="e18ec-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="e18ec-105">Gibt die Richtlinie, die von der Aktivität Audit betroffen war.</span><span class="sxs-lookup"><span data-stu-id="e18ec-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="e18ec-106">Die Ressource [TargetResource](targetresource.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="e18ec-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="e18ec-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e18ec-107">Properties</span></span>
| <span data-ttu-id="e18ec-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e18ec-108">Property</span></span>     | <span data-ttu-id="e18ec-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e18ec-109">Type</span></span>   |<span data-ttu-id="e18ec-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e18ec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e18ec-111">policyType</span><span class="sxs-lookup"><span data-stu-id="e18ec-111">policyType</span></span>|<span data-ttu-id="e18ec-112">String</span><span class="sxs-lookup"><span data-stu-id="e18ec-112">String</span></span>|<span data-ttu-id="e18ec-113">Gibt den Namen der Richtlinie, die geändert oder wurde gezielt für Änderung</span><span class="sxs-lookup"><span data-stu-id="e18ec-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e18ec-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e18ec-114">JSON representation</span></span>

<span data-ttu-id="e18ec-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e18ec-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
