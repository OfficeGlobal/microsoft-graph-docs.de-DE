---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68a276dc2a750db801b6f4ae893dbfc57ae66a97
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140306"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="d4af1-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4af1-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d4af1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4af1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4af1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d4af1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4af1-106">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="d4af1-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="d4af1-107">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d4af1-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4af1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4af1-108">Properties</span></span>
|<span data-ttu-id="d4af1-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4af1-109">Property</span></span>|<span data-ttu-id="d4af1-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d4af1-110">Type</span></span>|<span data-ttu-id="d4af1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4af1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4af1-112">groupId</span><span class="sxs-lookup"><span data-stu-id="d4af1-112">groupId</span></span>|<span data-ttu-id="d4af1-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4af1-113">String</span></span>|<span data-ttu-id="d4af1-114">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="d4af1-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4af1-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4af1-115">Relationships</span></span>
<span data-ttu-id="d4af1-116">Keine</span><span class="sxs-lookup"><span data-stu-id="d4af1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4af1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4af1-117">JSON Representation</span></span>
<span data-ttu-id="d4af1-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4af1-118">Here is a JSON representation of the resource.</span></span>
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




