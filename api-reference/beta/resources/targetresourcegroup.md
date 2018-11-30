---
title: Ressourcentyp targetResourceGroup
description: 'Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war. Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061422"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="7bc96-104">Ressourcentyp targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="7bc96-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="7bc96-105">Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war.</span><span class="sxs-lookup"><span data-stu-id="7bc96-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="7bc96-106">Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD</span><span class="sxs-lookup"><span data-stu-id="7bc96-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="7bc96-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7bc96-107">Properties</span></span>
| <span data-ttu-id="7bc96-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bc96-108">Property</span></span>     | <span data-ttu-id="7bc96-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7bc96-109">Type</span></span>   |<span data-ttu-id="7bc96-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bc96-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bc96-111">groupType</span><span class="sxs-lookup"><span data-stu-id="7bc96-111">groupType</span></span>|<span data-ttu-id="7bc96-112">String</span><span class="sxs-lookup"><span data-stu-id="7bc96-112">String</span></span>| <span data-ttu-id="7bc96-113">Mögliche Werte sind: `unifiedGroups`, `azureAD` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7bc96-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bc96-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7bc96-114">JSON representation</span></span>

<span data-ttu-id="7bc96-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7bc96-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->