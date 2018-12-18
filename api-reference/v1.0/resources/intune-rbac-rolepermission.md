---
title: rolePermission-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 0433c3f3a0ab3ef63fcd2a44776c083ddb5b91a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325676"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="5aa8f-103">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5aa8f-103">rolePermission resource type</span></span>

> <span data-ttu-id="5aa8f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5aa8f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5aa8f-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5aa8f-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="5aa8f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5aa8f-106">Properties</span></span>
|<span data-ttu-id="5aa8f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5aa8f-107">Property</span></span>|<span data-ttu-id="5aa8f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5aa8f-108">Type</span></span>|<span data-ttu-id="5aa8f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5aa8f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aa8f-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="5aa8f-110">resourceActions</span></span>|<span data-ttu-id="5aa8f-111">[resourceAction](../resources/intune-rbac-resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="5aa8f-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="5aa8f-112">Aktionen</span><span class="sxs-lookup"><span data-stu-id="5aa8f-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aa8f-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5aa8f-113">Relationships</span></span>
<span data-ttu-id="5aa8f-114">Keine</span><span class="sxs-lookup"><span data-stu-id="5aa8f-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5aa8f-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5aa8f-115">JSON Representation</span></span>
<span data-ttu-id="5aa8f-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5aa8f-116">Here is a JSON representation of the resource.</span></span>
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



