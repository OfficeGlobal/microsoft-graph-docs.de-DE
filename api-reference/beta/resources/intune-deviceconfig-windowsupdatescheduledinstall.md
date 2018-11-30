---
title: windowsUpdateScheduledInstall-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 9f39a9716efed39529c54eaddc62cde075b51954
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060206"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="91b2d-103">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91b2d-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="91b2d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91b2d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91b2d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91b2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91b2d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91b2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91b2d-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="91b2d-107">Not yet documented</span></span>

<span data-ttu-id="91b2d-108">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="91b2d-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91b2d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91b2d-109">Properties</span></span>
|<span data-ttu-id="91b2d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91b2d-110">Property</span></span>|<span data-ttu-id="91b2d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="91b2d-111">Type</span></span>|<span data-ttu-id="91b2d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91b2d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b2d-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="91b2d-113">scheduledInstallDay</span></span>|[<span data-ttu-id="91b2d-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="91b2d-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="91b2d-115">Geplante installieren Tag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="91b2d-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="91b2d-116">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="91b2d-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="91b2d-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="91b2d-117">scheduledInstallTime</span></span>|<span data-ttu-id="91b2d-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="91b2d-118">TimeOfDay</span></span>|<span data-ttu-id="91b2d-119">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="91b2d-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="91b2d-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91b2d-120">Relationships</span></span>
<span data-ttu-id="91b2d-121">Keine</span><span class="sxs-lookup"><span data-stu-id="91b2d-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91b2d-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91b2d-122">JSON Representation</span></span>
<span data-ttu-id="91b2d-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91b2d-123">Here is a JSON representation of the resource.</span></span>
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





