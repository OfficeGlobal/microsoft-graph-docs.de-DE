---
title: Ressourcentyp hourlySchedule
description: Stündlich ausführen Zeitplan eines sich wiederholenden Gerät Management Skripts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf62c11da0932f5f10b6cc7a76ccecfd1e74ee92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396826"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="55716-103">Ressourcentyp hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="55716-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="55716-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="55716-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="55716-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55716-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55716-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55716-107">Stündlich ausführen Zeitplan eines sich wiederholenden Gerät Management Skripts.</span><span class="sxs-lookup"><span data-stu-id="55716-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="55716-108">Erbt vom [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="55716-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55716-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="55716-109">Properties</span></span>
|<span data-ttu-id="55716-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="55716-110">Property</span></span>|<span data-ttu-id="55716-111">Typ</span><span class="sxs-lookup"><span data-stu-id="55716-111">Type</span></span>|<span data-ttu-id="55716-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55716-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55716-113">Intervall</span><span class="sxs-lookup"><span data-stu-id="55716-113">interval</span></span>|<span data-ttu-id="55716-114">Int32</span><span class="sxs-lookup"><span data-stu-id="55716-114">Int32</span></span>|<span data-ttu-id="55716-115">Intervall in Stunden</span><span class="sxs-lookup"><span data-stu-id="55716-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="55716-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="55716-116">Relationships</span></span>
<span data-ttu-id="55716-117">Keine</span><span class="sxs-lookup"><span data-stu-id="55716-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55716-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="55716-118">JSON Representation</span></span>
<span data-ttu-id="55716-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="55716-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




