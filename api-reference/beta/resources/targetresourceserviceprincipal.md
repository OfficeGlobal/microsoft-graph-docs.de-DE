---
title: Ressourcentyp targetResourceServicePrincipal
description: Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen. Die Ressource TargetResource abgeleitet.
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064064"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="182b1-104">Ressourcentyp targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="182b1-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="182b1-105">Gibt die ServicePrincipalId für die Ressource, die die Audit-Aktivität betroffen.</span><span class="sxs-lookup"><span data-stu-id="182b1-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="182b1-106">Die Ressource [TargetResource](targetresource.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="182b1-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="182b1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="182b1-107">Properties</span></span>
| <span data-ttu-id="182b1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="182b1-108">Property</span></span>     | <span data-ttu-id="182b1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="182b1-109">Type</span></span>   |<span data-ttu-id="182b1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="182b1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="182b1-111">appId</span><span class="sxs-lookup"><span data-stu-id="182b1-111">appId</span></span>|<span data-ttu-id="182b1-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="182b1-112">String</span></span>|<span data-ttu-id="182b1-113">Gibt die eindeutige Id der Anwendung an.</span><span class="sxs-lookup"><span data-stu-id="182b1-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="182b1-114">Verweist auf die App-Id für eine angegebene app.</span><span class="sxs-lookup"><span data-stu-id="182b1-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="182b1-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="182b1-115">JSON representation</span></span>

<span data-ttu-id="182b1-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="182b1-116">Here is a JSON representation of the resource.</span></span>

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