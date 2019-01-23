---
title: exclusionGroupAssignmentTarget-Ressourcentyp
description: Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a42cab192a9cd643c6c11de596ca0790fa8b4a5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421886"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="e6301-103">exclusionGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e6301-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="e6301-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e6301-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6301-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6301-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6301-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6301-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6301-107">Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.</span><span class="sxs-lookup"><span data-stu-id="e6301-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="e6301-108">Erbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e6301-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6301-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6301-109">Properties</span></span>
|<span data-ttu-id="e6301-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6301-110">Property</span></span>|<span data-ttu-id="e6301-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e6301-111">Type</span></span>|<span data-ttu-id="e6301-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6301-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6301-113">groupId</span><span class="sxs-lookup"><span data-stu-id="e6301-113">groupId</span></span>|<span data-ttu-id="e6301-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6301-114">String</span></span>|<span data-ttu-id="e6301-115">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="e6301-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="e6301-116">Vererbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e6301-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6301-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e6301-117">Relationships</span></span>
<span data-ttu-id="e6301-118">Keine</span><span class="sxs-lookup"><span data-stu-id="e6301-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6301-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6301-119">JSON Representation</span></span>
<span data-ttu-id="e6301-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6301-120">Here is a JSON representation of the resource.</span></span>
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




