---
title: exclusionGroupAssignmentTarget-Ressourcentyp
description: Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fbfa4e6df9dae514a99fa96aace073bd702def9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254086"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="a1cfb-103">exclusionGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1cfb-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="a1cfb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a1cfb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1cfb-105">Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.</span><span class="sxs-lookup"><span data-stu-id="a1cfb-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="a1cfb-106">Erbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a1cfb-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1cfb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1cfb-107">Properties</span></span>
|<span data-ttu-id="a1cfb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1cfb-108">Property</span></span>|<span data-ttu-id="a1cfb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a1cfb-109">Type</span></span>|<span data-ttu-id="a1cfb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1cfb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1cfb-111">groupId</span><span class="sxs-lookup"><span data-stu-id="a1cfb-111">groupId</span></span>|<span data-ttu-id="a1cfb-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1cfb-112">String</span></span>|<span data-ttu-id="a1cfb-113">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="a1cfb-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="a1cfb-114">Vererbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a1cfb-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1cfb-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a1cfb-115">Relationships</span></span>
<span data-ttu-id="a1cfb-116">Keine</span><span class="sxs-lookup"><span data-stu-id="a1cfb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1cfb-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1cfb-117">JSON Representation</span></span>
<span data-ttu-id="a1cfb-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1cfb-118">Here is a JSON representation of the resource.</span></span>
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



