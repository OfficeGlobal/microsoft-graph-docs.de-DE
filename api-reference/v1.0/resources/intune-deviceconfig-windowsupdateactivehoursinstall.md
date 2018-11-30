---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: c9647cda65d680629fda57e3dfdcbffb3d5d8625
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016141"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="8add5-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8add5-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="8add5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8add5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8add5-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8add5-105">Not yet documented</span></span>

<span data-ttu-id="8add5-106">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8add5-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8add5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8add5-107">Properties</span></span>
|<span data-ttu-id="8add5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8add5-108">Property</span></span>|<span data-ttu-id="8add5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8add5-109">Type</span></span>|<span data-ttu-id="8add5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8add5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8add5-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8add5-111">activeHoursStart</span></span>|<span data-ttu-id="8add5-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8add5-112">TimeOfDay</span></span>|<span data-ttu-id="8add5-113">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="8add5-113">Active Hours Start</span></span>|
|<span data-ttu-id="8add5-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8add5-114">activeHoursEnd</span></span>|<span data-ttu-id="8add5-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8add5-115">TimeOfDay</span></span>|<span data-ttu-id="8add5-116">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="8add5-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="8add5-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8add5-117">Relationships</span></span>
<span data-ttu-id="8add5-118">Keine</span><span class="sxs-lookup"><span data-stu-id="8add5-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8add5-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8add5-119">JSON Representation</span></span>
<span data-ttu-id="8add5-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8add5-120">Here is a JSON representation of the resource.</span></span>
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



