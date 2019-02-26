---
title: windowsUpdateScheduledInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264316"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="fd707-103">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd707-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="fd707-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fd707-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd707-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="fd707-105">Not yet documented</span></span>


<span data-ttu-id="fd707-106">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="fd707-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd707-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd707-107">Properties</span></span>
|<span data-ttu-id="fd707-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd707-108">Property</span></span>|<span data-ttu-id="fd707-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fd707-109">Type</span></span>|<span data-ttu-id="fd707-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd707-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd707-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="fd707-111">scheduledInstallDay</span></span>|[<span data-ttu-id="fd707-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="fd707-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="fd707-113">Geplanter Installationstag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="fd707-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="fd707-114">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="fd707-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="fd707-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="fd707-115">scheduledInstallTime</span></span>|<span data-ttu-id="fd707-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fd707-116">TimeOfDay</span></span>|<span data-ttu-id="fd707-117">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="fd707-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd707-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd707-118">Relationships</span></span>
<span data-ttu-id="fd707-119">Keine</span><span class="sxs-lookup"><span data-stu-id="fd707-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd707-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd707-120">JSON Representation</span></span>
<span data-ttu-id="fd707-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd707-121">Here is a JSON representation of the resource.</span></span>
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



