---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f344c0ed718f32352901af63da32c11ca02e2db6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849812"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="4d9d4-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4d9d4-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="4d9d4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d9d4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d9d4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d9d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d9d4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d9d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d9d4-107">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="4d9d4-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="4d9d4-108">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4d9d4-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d9d4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d9d4-109">Properties</span></span>
|<span data-ttu-id="4d9d4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d9d4-110">Property</span></span>|<span data-ttu-id="4d9d4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4d9d4-111">Type</span></span>|<span data-ttu-id="4d9d4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d9d4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d9d4-113">groupId</span><span class="sxs-lookup"><span data-stu-id="4d9d4-113">groupId</span></span>|<span data-ttu-id="4d9d4-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d9d4-114">String</span></span>|<span data-ttu-id="4d9d4-115">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="4d9d4-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d9d4-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4d9d4-116">Relationships</span></span>
<span data-ttu-id="4d9d4-117">Keine</span><span class="sxs-lookup"><span data-stu-id="4d9d4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d9d4-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d9d4-118">JSON Representation</span></span>
<span data-ttu-id="4d9d4-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d9d4-119">Here is a JSON representation of the resource.</span></span>
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





