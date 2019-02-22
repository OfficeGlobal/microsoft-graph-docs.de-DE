---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9deab255749e70cfd165f28c27c09182b298e00a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144093"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b542b-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b542b-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="b542b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b542b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b542b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b542b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b542b-106">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b542b-106">Not yet documented</span></span>


<span data-ttu-id="b542b-107">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b542b-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b542b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b542b-108">Properties</span></span>
|<span data-ttu-id="b542b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b542b-109">Property</span></span>|<span data-ttu-id="b542b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b542b-110">Type</span></span>|<span data-ttu-id="b542b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b542b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b542b-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b542b-112">activeHoursStart</span></span>|<span data-ttu-id="b542b-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b542b-113">TimeOfDay</span></span>|<span data-ttu-id="b542b-114">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="b542b-114">Active Hours Start</span></span>|
|<span data-ttu-id="b542b-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b542b-115">activeHoursEnd</span></span>|<span data-ttu-id="b542b-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b542b-116">TimeOfDay</span></span>|<span data-ttu-id="b542b-117">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="b542b-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b542b-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b542b-118">Relationships</span></span>
<span data-ttu-id="b542b-119">Keine</span><span class="sxs-lookup"><span data-stu-id="b542b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b542b-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b542b-120">JSON Representation</span></span>
<span data-ttu-id="b542b-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b542b-121">Here is a JSON representation of the resource.</span></span>
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




