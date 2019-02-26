---
title: hourlySchedule-Ressourcentyp
description: Stündlicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb3eacf4e17ed1137ce78d21112c394a45423c6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173416"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="84e8c-103">hourlySchedule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="84e8c-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="84e8c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84e8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84e8c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="84e8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e8c-106">Stündlicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.</span><span class="sxs-lookup"><span data-stu-id="84e8c-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="84e8c-107">Erbt von [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="84e8c-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84e8c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="84e8c-108">Properties</span></span>
|<span data-ttu-id="84e8c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84e8c-109">Property</span></span>|<span data-ttu-id="84e8c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="84e8c-110">Type</span></span>|<span data-ttu-id="84e8c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84e8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e8c-112">Intervall</span><span class="sxs-lookup"><span data-stu-id="84e8c-112">interval</span></span>|<span data-ttu-id="84e8c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="84e8c-113">Int32</span></span>|<span data-ttu-id="84e8c-114">Intervall in Stunden</span><span class="sxs-lookup"><span data-stu-id="84e8c-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e8c-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="84e8c-115">Relationships</span></span>
<span data-ttu-id="84e8c-116">Keine</span><span class="sxs-lookup"><span data-stu-id="84e8c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84e8c-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="84e8c-117">JSON Representation</span></span>
<span data-ttu-id="84e8c-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="84e8c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




