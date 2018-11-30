---
title: rolePermission-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 16c78e2ee4475a717879d501aabeb5fe2ae0d481
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017619"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="33be7-103">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="33be7-103">rolePermission resource type</span></span>

> <span data-ttu-id="33be7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33be7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33be7-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="33be7-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="33be7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33be7-106">Properties</span></span>
|<span data-ttu-id="33be7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33be7-107">Property</span></span>|<span data-ttu-id="33be7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="33be7-108">Type</span></span>|<span data-ttu-id="33be7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33be7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33be7-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="33be7-110">resourceActions</span></span>|<span data-ttu-id="33be7-111">[resourceAction](../resources/intune-rbac-resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="33be7-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="33be7-112">Aktionen</span><span class="sxs-lookup"><span data-stu-id="33be7-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="33be7-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="33be7-113">Relationships</span></span>
<span data-ttu-id="33be7-114">Keine</span><span class="sxs-lookup"><span data-stu-id="33be7-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33be7-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33be7-115">JSON Representation</span></span>
<span data-ttu-id="33be7-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33be7-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



