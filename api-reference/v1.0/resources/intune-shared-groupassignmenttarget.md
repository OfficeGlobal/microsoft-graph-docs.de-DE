---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
ms.openlocfilehash: 0ebb41b1f737a20a37d322bac7ab5ae6ab2a248f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018270"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="282e9-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="282e9-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="282e9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="282e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="282e9-105">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="282e9-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="282e9-106">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="282e9-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="282e9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="282e9-107">Properties</span></span>
|<span data-ttu-id="282e9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="282e9-108">Property</span></span>|<span data-ttu-id="282e9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="282e9-109">Type</span></span>|<span data-ttu-id="282e9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="282e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="282e9-111">groupId</span><span class="sxs-lookup"><span data-stu-id="282e9-111">groupId</span></span>|<span data-ttu-id="282e9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="282e9-112">String</span></span>|<span data-ttu-id="282e9-113">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="282e9-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="282e9-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="282e9-114">Relationships</span></span>
<span data-ttu-id="282e9-115">Keine</span><span class="sxs-lookup"><span data-stu-id="282e9-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="282e9-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="282e9-116">JSON Representation</span></span>
<span data-ttu-id="282e9-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="282e9-117">Here is a JSON representation of the resource.</span></span>
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



