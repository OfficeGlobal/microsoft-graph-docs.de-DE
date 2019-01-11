---
title: Ressourcentyp targetResourceServicePrincipal
description: Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen. Die Ressource TargetResource abgeleitet.
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839599"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="eba4e-104">Ressourcentyp targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="eba4e-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="eba4e-105">Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen.</span><span class="sxs-lookup"><span data-stu-id="eba4e-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="eba4e-106">Die Ressource [TargetResource](targetresource.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="eba4e-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="eba4e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eba4e-107">Properties</span></span>
| <span data-ttu-id="eba4e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eba4e-108">Property</span></span>     | <span data-ttu-id="eba4e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="eba4e-109">Type</span></span>   |<span data-ttu-id="eba4e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eba4e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eba4e-111">appId</span><span class="sxs-lookup"><span data-stu-id="eba4e-111">appId</span></span>|<span data-ttu-id="eba4e-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eba4e-112">String</span></span>|<span data-ttu-id="eba4e-113">Gibt die eindeutige Id der Anwendung an.</span><span class="sxs-lookup"><span data-stu-id="eba4e-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="eba4e-114">Verweist auf die App-Id für eine angegebene app.</span><span class="sxs-lookup"><span data-stu-id="eba4e-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eba4e-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eba4e-115">JSON representation</span></span>

<span data-ttu-id="eba4e-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eba4e-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
