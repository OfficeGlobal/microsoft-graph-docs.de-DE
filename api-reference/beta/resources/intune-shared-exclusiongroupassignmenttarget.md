---
title: exclusionGroupAssignmentTarget-Ressourcentyp
description: Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0397a3f3def5be86b10f17e50617d488bf6a1512
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175395"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="7cdc7-103">exclusionGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7cdc7-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="7cdc7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7cdc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cdc7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7cdc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cdc7-106">Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.</span><span class="sxs-lookup"><span data-stu-id="7cdc7-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="7cdc7-107">Erbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7cdc7-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7cdc7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7cdc7-108">Properties</span></span>
|<span data-ttu-id="7cdc7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7cdc7-109">Property</span></span>|<span data-ttu-id="7cdc7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7cdc7-110">Type</span></span>|<span data-ttu-id="7cdc7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cdc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cdc7-112">groupId</span><span class="sxs-lookup"><span data-stu-id="7cdc7-112">groupId</span></span>|<span data-ttu-id="7cdc7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cdc7-113">String</span></span>|<span data-ttu-id="7cdc7-114">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="7cdc7-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="7cdc7-115">Vererbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7cdc7-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cdc7-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7cdc7-116">Relationships</span></span>
<span data-ttu-id="7cdc7-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7cdc7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cdc7-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7cdc7-118">JSON Representation</span></span>
<span data-ttu-id="7cdc7-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7cdc7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```




