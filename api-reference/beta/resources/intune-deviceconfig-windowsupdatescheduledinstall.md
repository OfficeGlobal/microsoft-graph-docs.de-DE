---
title: windowsUpdateScheduledInstall-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee91ed2541c02adbb7a130f0a9de869d86044632
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395629"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="153fa-103">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="153fa-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="153fa-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="153fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="153fa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="153fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="153fa-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="153fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="153fa-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="153fa-107">Not yet documented</span></span>


<span data-ttu-id="153fa-108">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="153fa-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="153fa-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="153fa-109">Properties</span></span>
|<span data-ttu-id="153fa-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="153fa-110">Property</span></span>|<span data-ttu-id="153fa-111">Typ</span><span class="sxs-lookup"><span data-stu-id="153fa-111">Type</span></span>|<span data-ttu-id="153fa-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="153fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="153fa-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="153fa-113">scheduledInstallDay</span></span>|[<span data-ttu-id="153fa-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="153fa-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="153fa-115">Geplante installieren Tag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="153fa-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="153fa-116">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="153fa-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="153fa-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="153fa-117">scheduledInstallTime</span></span>|<span data-ttu-id="153fa-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="153fa-118">TimeOfDay</span></span>|<span data-ttu-id="153fa-119">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="153fa-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="153fa-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="153fa-120">Relationships</span></span>
<span data-ttu-id="153fa-121">Keine</span><span class="sxs-lookup"><span data-stu-id="153fa-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="153fa-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="153fa-122">JSON Representation</span></span>
<span data-ttu-id="153fa-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="153fa-123">Here is a JSON representation of the resource.</span></span>
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




