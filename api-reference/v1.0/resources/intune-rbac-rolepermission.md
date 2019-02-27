---
title: rolePermission-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90de4e78bbc831ebb9eb7bf5ee65c26434fc06
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257785"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="faeab-103">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="faeab-103">rolePermission resource type</span></span>

> <span data-ttu-id="faeab-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="faeab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faeab-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="faeab-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="faeab-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="faeab-106">Properties</span></span>
|<span data-ttu-id="faeab-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="faeab-107">Property</span></span>|<span data-ttu-id="faeab-108">Typ</span><span class="sxs-lookup"><span data-stu-id="faeab-108">Type</span></span>|<span data-ttu-id="faeab-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="faeab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faeab-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="faeab-110">resourceActions</span></span>|<span data-ttu-id="faeab-111">[resourceAction](../resources/intune-rbac-resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="faeab-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="faeab-112">Aktionen</span><span class="sxs-lookup"><span data-stu-id="faeab-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="faeab-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="faeab-113">Relationships</span></span>
<span data-ttu-id="faeab-114">Keine</span><span class="sxs-lookup"><span data-stu-id="faeab-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faeab-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="faeab-115">JSON Representation</span></span>
<span data-ttu-id="faeab-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="faeab-116">Here is a JSON representation of the resource.</span></span>
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



