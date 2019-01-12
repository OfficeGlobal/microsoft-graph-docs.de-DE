---
title: windowsUpdateScheduledInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae4cb747cb4648cd9f4cc9550933688d180dd38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952041"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="8512c-103">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8512c-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="8512c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8512c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8512c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8512c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8512c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8512c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8512c-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8512c-107">Not yet documented</span></span>

<span data-ttu-id="8512c-108">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8512c-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8512c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8512c-109">Properties</span></span>
|<span data-ttu-id="8512c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8512c-110">Property</span></span>|<span data-ttu-id="8512c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8512c-111">Type</span></span>|<span data-ttu-id="8512c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8512c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8512c-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="8512c-113">scheduledInstallDay</span></span>|[<span data-ttu-id="8512c-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="8512c-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="8512c-115">Geplante installieren Tag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="8512c-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="8512c-116">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="8512c-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8512c-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="8512c-117">scheduledInstallTime</span></span>|<span data-ttu-id="8512c-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8512c-118">TimeOfDay</span></span>|<span data-ttu-id="8512c-119">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="8512c-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="8512c-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8512c-120">Relationships</span></span>
<span data-ttu-id="8512c-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8512c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8512c-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8512c-122">JSON Representation</span></span>
<span data-ttu-id="8512c-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8512c-123">Here is a JSON representation of the resource.</span></span>
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





