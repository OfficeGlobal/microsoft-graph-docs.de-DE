---
title: Ressourcentyp targetResourceGroup
description: 'Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war. Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851184"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="e270b-104">Ressourcentyp targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e270b-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="e270b-105">Gibt den Typ der Gruppe, die aufgrund der Audit-Aktivität betroffen war.</span><span class="sxs-lookup"><span data-stu-id="e270b-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="e270b-106">Enthält die Werte wie unified Gruppen im Vergleich zu Azure AD</span><span class="sxs-lookup"><span data-stu-id="e270b-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="e270b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e270b-107">Properties</span></span>
| <span data-ttu-id="e270b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e270b-108">Property</span></span>     | <span data-ttu-id="e270b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e270b-109">Type</span></span>   |<span data-ttu-id="e270b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e270b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e270b-111">groupType</span><span class="sxs-lookup"><span data-stu-id="e270b-111">groupType</span></span>|<span data-ttu-id="e270b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e270b-112">String</span></span>| <span data-ttu-id="e270b-113">Mögliche Werte sind: `unifiedGroups`, `azureAD` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e270b-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e270b-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e270b-114">JSON representation</span></span>

<span data-ttu-id="e270b-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e270b-115">Here is a JSON representation of the resource.</span></span>

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
