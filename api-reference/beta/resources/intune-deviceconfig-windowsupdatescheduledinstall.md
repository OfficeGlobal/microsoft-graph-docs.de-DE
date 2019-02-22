---
title: windowsUpdateScheduledInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de36e3777518cf7c79a7590c19147d014e2aee7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172506"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4f0b5-103">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4f0b5-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="4f0b5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f0b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f0b5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4f0b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f0b5-106">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4f0b5-106">Not yet documented</span></span>


<span data-ttu-id="4f0b5-107">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4f0b5-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f0b5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4f0b5-108">Properties</span></span>
|<span data-ttu-id="4f0b5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f0b5-109">Property</span></span>|<span data-ttu-id="4f0b5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4f0b5-110">Type</span></span>|<span data-ttu-id="4f0b5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f0b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f0b5-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4f0b5-112">scheduledInstallDay</span></span>|[<span data-ttu-id="4f0b5-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4f0b5-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4f0b5-114">Geplanter Installationstag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="4f0b5-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="4f0b5-115">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="4f0b5-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4f0b5-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4f0b5-116">scheduledInstallTime</span></span>|<span data-ttu-id="4f0b5-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4f0b5-117">TimeOfDay</span></span>|<span data-ttu-id="4f0b5-118">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="4f0b5-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f0b5-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4f0b5-119">Relationships</span></span>
<span data-ttu-id="4f0b5-120">Keine</span><span class="sxs-lookup"><span data-stu-id="4f0b5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f0b5-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4f0b5-121">JSON Representation</span></span>
<span data-ttu-id="4f0b5-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4f0b5-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```




