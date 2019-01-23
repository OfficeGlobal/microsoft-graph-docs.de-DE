---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2039f5917aa5d69b74ccb6c1732496dc567ab673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399423"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="d0058-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0058-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d0058-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d0058-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0058-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0058-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0058-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0058-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0058-107">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="d0058-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="d0058-108">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d0058-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0058-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0058-109">Properties</span></span>
|<span data-ttu-id="d0058-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0058-110">Property</span></span>|<span data-ttu-id="d0058-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d0058-111">Type</span></span>|<span data-ttu-id="d0058-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0058-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0058-113">groupId</span><span class="sxs-lookup"><span data-stu-id="d0058-113">groupId</span></span>|<span data-ttu-id="d0058-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0058-114">String</span></span>|<span data-ttu-id="d0058-115">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="d0058-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0058-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0058-116">Relationships</span></span>
<span data-ttu-id="d0058-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d0058-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0058-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0058-118">JSON Representation</span></span>
<span data-ttu-id="d0058-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0058-119">Here is a JSON representation of the resource.</span></span>
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




