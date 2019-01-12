---
title: rolePermission-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8b9ba237052fef2b4caa8123d147ea1782fa9b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932805"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="dece9-103">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dece9-103">rolePermission resource type</span></span>

> <span data-ttu-id="dece9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dece9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dece9-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="dece9-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="dece9-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dece9-106">Properties</span></span>
|<span data-ttu-id="dece9-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dece9-107">Property</span></span>|<span data-ttu-id="dece9-108">Typ</span><span class="sxs-lookup"><span data-stu-id="dece9-108">Type</span></span>|<span data-ttu-id="dece9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dece9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dece9-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="dece9-110">resourceActions</span></span>|<span data-ttu-id="dece9-111">[resourceAction](../resources/intune-rbac-resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="dece9-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="dece9-112">Aktionen</span><span class="sxs-lookup"><span data-stu-id="dece9-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="dece9-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dece9-113">Relationships</span></span>
<span data-ttu-id="dece9-114">Keine</span><span class="sxs-lookup"><span data-stu-id="dece9-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dece9-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dece9-115">JSON Representation</span></span>
<span data-ttu-id="dece9-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dece9-116">Here is a JSON representation of the resource.</span></span>
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



