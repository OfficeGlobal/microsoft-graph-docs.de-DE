---
title: dailySchedule-Ressourcentyp
description: Täglicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 310d9a4dbd995dfc162591547a40ace8c596f54b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152661"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="c97ee-103">dailySchedule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c97ee-103">dailySchedule resource type</span></span>

> <span data-ttu-id="c97ee-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c97ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c97ee-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c97ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c97ee-106">Täglicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.</span><span class="sxs-lookup"><span data-stu-id="c97ee-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="c97ee-107">Erbt von [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c97ee-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c97ee-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c97ee-108">Properties</span></span>
|<span data-ttu-id="c97ee-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c97ee-109">Property</span></span>|<span data-ttu-id="c97ee-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c97ee-110">Type</span></span>|<span data-ttu-id="c97ee-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c97ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97ee-112">Intervall</span><span class="sxs-lookup"><span data-stu-id="c97ee-112">interval</span></span>|<span data-ttu-id="c97ee-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c97ee-113">Int32</span></span>|<span data-ttu-id="c97ee-114">Intervall in Tagen</span><span class="sxs-lookup"><span data-stu-id="c97ee-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="c97ee-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c97ee-115">Relationships</span></span>
<span data-ttu-id="c97ee-116">Keine</span><span class="sxs-lookup"><span data-stu-id="c97ee-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c97ee-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c97ee-117">JSON Representation</span></span>
<span data-ttu-id="c97ee-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c97ee-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```




