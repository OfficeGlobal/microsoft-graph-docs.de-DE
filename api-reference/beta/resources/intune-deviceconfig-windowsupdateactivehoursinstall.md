---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 7a40a791a9a00d7cfd60287bade1759592e1bcf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064684"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="10874-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="10874-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="10874-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="10874-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10874-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10874-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10874-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10874-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10874-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="10874-107">Not yet documented</span></span>

<span data-ttu-id="10874-108">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="10874-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="10874-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10874-109">Properties</span></span>
|<span data-ttu-id="10874-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10874-110">Property</span></span>|<span data-ttu-id="10874-111">Typ</span><span class="sxs-lookup"><span data-stu-id="10874-111">Type</span></span>|<span data-ttu-id="10874-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10874-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10874-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="10874-113">activeHoursStart</span></span>|<span data-ttu-id="10874-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="10874-114">TimeOfDay</span></span>|<span data-ttu-id="10874-115">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="10874-115">Active Hours Start</span></span>|
|<span data-ttu-id="10874-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="10874-116">activeHoursEnd</span></span>|<span data-ttu-id="10874-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="10874-117">TimeOfDay</span></span>|<span data-ttu-id="10874-118">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="10874-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="10874-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10874-119">Relationships</span></span>
<span data-ttu-id="10874-120">Keine</span><span class="sxs-lookup"><span data-stu-id="10874-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10874-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10874-121">JSON Representation</span></span>
<span data-ttu-id="10874-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10874-122">Here is a JSON representation of the resource.</span></span>
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





