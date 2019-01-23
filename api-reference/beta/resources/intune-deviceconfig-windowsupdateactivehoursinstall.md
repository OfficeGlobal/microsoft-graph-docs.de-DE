---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28f40501123f465d8fcbfa05c3febb8ffab6f27a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409468"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="0f6eb-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f6eb-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="0f6eb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0f6eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f6eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f6eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f6eb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f6eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f6eb-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0f6eb-107">Not yet documented</span></span>


<span data-ttu-id="0f6eb-108">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="0f6eb-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f6eb-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f6eb-109">Properties</span></span>
|<span data-ttu-id="0f6eb-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f6eb-110">Property</span></span>|<span data-ttu-id="0f6eb-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0f6eb-111">Type</span></span>|<span data-ttu-id="0f6eb-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f6eb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f6eb-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="0f6eb-113">activeHoursStart</span></span>|<span data-ttu-id="0f6eb-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0f6eb-114">TimeOfDay</span></span>|<span data-ttu-id="0f6eb-115">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="0f6eb-115">Active Hours Start</span></span>|
|<span data-ttu-id="0f6eb-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="0f6eb-116">activeHoursEnd</span></span>|<span data-ttu-id="0f6eb-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0f6eb-117">TimeOfDay</span></span>|<span data-ttu-id="0f6eb-118">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="0f6eb-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f6eb-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f6eb-119">Relationships</span></span>
<span data-ttu-id="0f6eb-120">Keine</span><span class="sxs-lookup"><span data-stu-id="0f6eb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f6eb-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f6eb-121">JSON Representation</span></span>
<span data-ttu-id="0f6eb-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f6eb-122">Here is a JSON representation of the resource.</span></span>
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




