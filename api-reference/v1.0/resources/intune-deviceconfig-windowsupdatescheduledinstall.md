---
title: windowsUpdateScheduledInstall-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 06e26bfb43691c8774e166a65b36d6ab872d44e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017498"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="1e982-103">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1e982-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="1e982-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1e982-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e982-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1e982-105">Not yet documented</span></span>

<span data-ttu-id="1e982-106">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="1e982-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e982-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1e982-107">Properties</span></span>
|<span data-ttu-id="1e982-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e982-108">Property</span></span>|<span data-ttu-id="1e982-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1e982-109">Type</span></span>|<span data-ttu-id="1e982-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e982-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e982-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="1e982-111">scheduledInstallDay</span></span>|[<span data-ttu-id="1e982-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="1e982-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="1e982-113">Geplante installieren Tag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="1e982-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="1e982-114">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="1e982-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1e982-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="1e982-115">scheduledInstallTime</span></span>|<span data-ttu-id="1e982-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1e982-116">TimeOfDay</span></span>|<span data-ttu-id="1e982-117">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="1e982-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e982-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1e982-118">Relationships</span></span>
<span data-ttu-id="1e982-119">Keine</span><span class="sxs-lookup"><span data-stu-id="1e982-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e982-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1e982-120">JSON Representation</span></span>
<span data-ttu-id="1e982-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e982-121">Here is a JSON representation of the resource.</span></span>
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



