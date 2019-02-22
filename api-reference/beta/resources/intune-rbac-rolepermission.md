---
title: rolePermission-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b56df927cda3cbf98e7d736311aba2db5e53906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145381"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="65f62-103">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="65f62-103">rolePermission resource type</span></span>

> <span data-ttu-id="65f62-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65f62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f62-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="65f62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f62-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="65f62-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="65f62-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65f62-107">Properties</span></span>
|<span data-ttu-id="65f62-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65f62-108">Property</span></span>|<span data-ttu-id="65f62-109">Typ</span><span class="sxs-lookup"><span data-stu-id="65f62-109">Type</span></span>|<span data-ttu-id="65f62-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65f62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f62-111">Aktionen</span><span class="sxs-lookup"><span data-stu-id="65f62-111">actions</span></span>|<span data-ttu-id="65f62-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="65f62-112">String collection</span></span>|<span data-ttu-id="65f62-113">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="65f62-113">Allowed Actions</span></span>|
|<span data-ttu-id="65f62-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="65f62-114">resourceActions</span></span>|<span data-ttu-id="65f62-115">[resourceAction](../resources/intune-rbac-resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="65f62-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="65f62-116">Aktionen</span><span class="sxs-lookup"><span data-stu-id="65f62-116">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="65f62-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="65f62-117">Relationships</span></span>
<span data-ttu-id="65f62-118">Keine</span><span class="sxs-lookup"><span data-stu-id="65f62-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65f62-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65f62-119">JSON Representation</span></span>
<span data-ttu-id="65f62-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65f62-120">Here is a JSON representation of the resource.</span></span>
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




