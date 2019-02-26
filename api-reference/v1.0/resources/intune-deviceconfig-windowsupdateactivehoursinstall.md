---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264057"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="46304-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46304-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="46304-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="46304-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46304-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="46304-105">Not yet documented</span></span>


<span data-ttu-id="46304-106">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="46304-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46304-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46304-107">Properties</span></span>
|<span data-ttu-id="46304-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46304-108">Property</span></span>|<span data-ttu-id="46304-109">Typ</span><span class="sxs-lookup"><span data-stu-id="46304-109">Type</span></span>|<span data-ttu-id="46304-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46304-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46304-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="46304-111">activeHoursStart</span></span>|<span data-ttu-id="46304-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="46304-112">TimeOfDay</span></span>|<span data-ttu-id="46304-113">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="46304-113">Active Hours Start</span></span>|
|<span data-ttu-id="46304-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="46304-114">activeHoursEnd</span></span>|<span data-ttu-id="46304-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="46304-115">TimeOfDay</span></span>|<span data-ttu-id="46304-116">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="46304-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="46304-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46304-117">Relationships</span></span>
<span data-ttu-id="46304-118">Keine</span><span class="sxs-lookup"><span data-stu-id="46304-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46304-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46304-119">JSON Representation</span></span>
<span data-ttu-id="46304-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46304-120">Here is a JSON representation of the resource.</span></span>
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



