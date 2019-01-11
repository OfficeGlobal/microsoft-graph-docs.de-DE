---
title: exclusionGroupAssignmentTarget-Ressourcentyp
description: Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad844205e0cb5f5b4d0b86d71212e2d9c2ca223e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826453"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="97550-103">exclusionGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="97550-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="97550-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97550-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97550-105">Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.</span><span class="sxs-lookup"><span data-stu-id="97550-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="97550-106">Erbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="97550-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97550-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97550-107">Properties</span></span>
|<span data-ttu-id="97550-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97550-108">Property</span></span>|<span data-ttu-id="97550-109">Typ</span><span class="sxs-lookup"><span data-stu-id="97550-109">Type</span></span>|<span data-ttu-id="97550-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97550-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97550-111">groupId</span><span class="sxs-lookup"><span data-stu-id="97550-111">groupId</span></span>|<span data-ttu-id="97550-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97550-112">String</span></span>|<span data-ttu-id="97550-113">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="97550-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="97550-114">Vererbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="97550-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="97550-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="97550-115">Relationships</span></span>
<span data-ttu-id="97550-116">Keine</span><span class="sxs-lookup"><span data-stu-id="97550-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97550-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97550-117">JSON Representation</span></span>
<span data-ttu-id="97550-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="97550-118">Here is a JSON representation of the resource.</span></span>
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



