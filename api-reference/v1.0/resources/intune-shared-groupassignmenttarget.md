---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ac3c4519cc074c3cce423ca5d0745c8a78d865
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250173"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="52206-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="52206-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="52206-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="52206-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52206-105">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="52206-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="52206-106">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="52206-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52206-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="52206-107">Properties</span></span>
|<span data-ttu-id="52206-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52206-108">Property</span></span>|<span data-ttu-id="52206-109">Typ</span><span class="sxs-lookup"><span data-stu-id="52206-109">Type</span></span>|<span data-ttu-id="52206-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52206-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52206-111">groupId</span><span class="sxs-lookup"><span data-stu-id="52206-111">groupId</span></span>|<span data-ttu-id="52206-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52206-112">String</span></span>|<span data-ttu-id="52206-113">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="52206-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52206-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="52206-114">Relationships</span></span>
<span data-ttu-id="52206-115">Keine</span><span class="sxs-lookup"><span data-stu-id="52206-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52206-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="52206-116">JSON Representation</span></span>
<span data-ttu-id="52206-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="52206-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



