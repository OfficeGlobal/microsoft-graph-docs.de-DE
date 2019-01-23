---
title: Ressourcentyp dailySchedule
description: Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4cbe48aecf3fe561becad4734f7de0b5f68ffa0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415250"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="12973-103">Ressourcentyp dailySchedule</span><span class="sxs-lookup"><span data-stu-id="12973-103">dailySchedule resource type</span></span>

> <span data-ttu-id="12973-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="12973-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12973-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12973-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12973-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12973-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12973-107">Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.</span><span class="sxs-lookup"><span data-stu-id="12973-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="12973-108">Erbt vom [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="12973-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="12973-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12973-109">Properties</span></span>
|<span data-ttu-id="12973-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12973-110">Property</span></span>|<span data-ttu-id="12973-111">Typ</span><span class="sxs-lookup"><span data-stu-id="12973-111">Type</span></span>|<span data-ttu-id="12973-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12973-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12973-113">Intervall</span><span class="sxs-lookup"><span data-stu-id="12973-113">interval</span></span>|<span data-ttu-id="12973-114">Int32</span><span class="sxs-lookup"><span data-stu-id="12973-114">Int32</span></span>|<span data-ttu-id="12973-115">Intervall in Tagen</span><span class="sxs-lookup"><span data-stu-id="12973-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="12973-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="12973-116">Relationships</span></span>
<span data-ttu-id="12973-117">Keine</span><span class="sxs-lookup"><span data-stu-id="12973-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12973-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12973-118">JSON Representation</span></span>
<span data-ttu-id="12973-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12973-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```




