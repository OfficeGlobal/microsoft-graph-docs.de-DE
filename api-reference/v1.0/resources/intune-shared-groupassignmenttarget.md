---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7218fc69564ea08a7302cfb0af7856360cd9a330
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809044"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="71acb-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71acb-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="71acb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71acb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71acb-105">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="71acb-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="71acb-106">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="71acb-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71acb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71acb-107">Properties</span></span>
|<span data-ttu-id="71acb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71acb-108">Property</span></span>|<span data-ttu-id="71acb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="71acb-109">Type</span></span>|<span data-ttu-id="71acb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71acb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71acb-111">groupId</span><span class="sxs-lookup"><span data-stu-id="71acb-111">groupId</span></span>|<span data-ttu-id="71acb-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71acb-112">String</span></span>|<span data-ttu-id="71acb-113">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="71acb-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71acb-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71acb-114">Relationships</span></span>
<span data-ttu-id="71acb-115">Keine</span><span class="sxs-lookup"><span data-stu-id="71acb-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71acb-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71acb-116">JSON Representation</span></span>
<span data-ttu-id="71acb-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71acb-117">Here is a JSON representation of the resource.</span></span>
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



