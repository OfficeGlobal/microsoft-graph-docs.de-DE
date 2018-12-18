---
title: rolePermission-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: c33af6af3bc06a53bd24ddf97576551a5eea6e9c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349105"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="a03c3-103">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a03c3-103">rolePermission resource type</span></span>

> <span data-ttu-id="a03c3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a03c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a03c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a03c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a03c3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a03c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a03c3-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a03c3-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a03c3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a03c3-108">Properties</span></span>
|<span data-ttu-id="a03c3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a03c3-109">Property</span></span>|<span data-ttu-id="a03c3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a03c3-110">Type</span></span>|<span data-ttu-id="a03c3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a03c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a03c3-112">Aktionen</span><span class="sxs-lookup"><span data-stu-id="a03c3-112">actions</span></span>|<span data-ttu-id="a03c3-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a03c3-113">String collection</span></span>|<span data-ttu-id="a03c3-114">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="a03c3-114">Allowed Actions</span></span>|
|<span data-ttu-id="a03c3-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="a03c3-115">resourceActions</span></span>|<span data-ttu-id="a03c3-116">[resourceAction](../resources/intune-rbac-resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="a03c3-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="a03c3-117">Aktionen</span><span class="sxs-lookup"><span data-stu-id="a03c3-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="a03c3-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a03c3-118">Relationships</span></span>
<span data-ttu-id="a03c3-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a03c3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a03c3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a03c3-120">JSON Representation</span></span>
<span data-ttu-id="a03c3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a03c3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
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





