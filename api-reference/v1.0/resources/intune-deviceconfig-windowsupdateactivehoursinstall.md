---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed4f909db5dd31195ace7d98151b226b03849c81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967182"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="46305-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46305-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="46305-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46305-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46305-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="46305-105">Not yet documented</span></span>

<span data-ttu-id="46305-106">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="46305-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46305-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46305-107">Properties</span></span>
|<span data-ttu-id="46305-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46305-108">Property</span></span>|<span data-ttu-id="46305-109">Typ</span><span class="sxs-lookup"><span data-stu-id="46305-109">Type</span></span>|<span data-ttu-id="46305-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46305-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46305-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="46305-111">activeHoursStart</span></span>|<span data-ttu-id="46305-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="46305-112">TimeOfDay</span></span>|<span data-ttu-id="46305-113">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="46305-113">Active Hours Start</span></span>|
|<span data-ttu-id="46305-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="46305-114">activeHoursEnd</span></span>|<span data-ttu-id="46305-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="46305-115">TimeOfDay</span></span>|<span data-ttu-id="46305-116">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="46305-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="46305-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46305-117">Relationships</span></span>
<span data-ttu-id="46305-118">Keine</span><span class="sxs-lookup"><span data-stu-id="46305-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46305-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46305-119">JSON Representation</span></span>
<span data-ttu-id="46305-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46305-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



