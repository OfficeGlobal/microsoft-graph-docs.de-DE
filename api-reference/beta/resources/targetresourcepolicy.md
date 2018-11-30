---
title: Ressourcentyp targetResourcePolicy
description: 'Gibt die Richtlinie, die von der Aktivität Audit betroffen war. Die Ressource TargetResource abgeleitet.   '
ms.openlocfilehash: 20486c535d0df4b3745f5cfc3414b320a9374075
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063422"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="727a3-104">Ressourcentyp targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="727a3-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="727a3-105">Gibt die Richtlinie, die von der Aktivität Audit betroffen war.</span><span class="sxs-lookup"><span data-stu-id="727a3-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="727a3-106">Die Ressource [TargetResource](targetresource.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="727a3-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="727a3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="727a3-107">Properties</span></span>
| <span data-ttu-id="727a3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="727a3-108">Property</span></span>     | <span data-ttu-id="727a3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="727a3-109">Type</span></span>   |<span data-ttu-id="727a3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="727a3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="727a3-111">policyType</span><span class="sxs-lookup"><span data-stu-id="727a3-111">policyType</span></span>|<span data-ttu-id="727a3-112">String</span><span class="sxs-lookup"><span data-stu-id="727a3-112">String</span></span>|<span data-ttu-id="727a3-113">Gibt den Namen der Richtlinie, die geändert oder wurde gezielt für Änderung</span><span class="sxs-lookup"><span data-stu-id="727a3-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="727a3-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="727a3-114">JSON representation</span></span>

<span data-ttu-id="727a3-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="727a3-115">Here is a JSON representation of the resource.</span></span>

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