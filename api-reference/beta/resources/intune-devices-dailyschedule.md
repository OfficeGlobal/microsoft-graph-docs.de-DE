---
title: Ressourcentyp dailySchedule
description: Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5321bce51f0f682591c6b27a0acec4ed95d0e2e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840558"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="7e75c-103">Ressourcentyp dailySchedule</span><span class="sxs-lookup"><span data-stu-id="7e75c-103">dailySchedule resource type</span></span>

> <span data-ttu-id="7e75c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e75c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e75c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e75c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e75c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e75c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e75c-107">Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.</span><span class="sxs-lookup"><span data-stu-id="7e75c-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="7e75c-108">Erbt vom [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="7e75c-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e75c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e75c-109">Properties</span></span>
|<span data-ttu-id="7e75c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e75c-110">Property</span></span>|<span data-ttu-id="7e75c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7e75c-111">Type</span></span>|<span data-ttu-id="7e75c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e75c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e75c-113">Intervall</span><span class="sxs-lookup"><span data-stu-id="7e75c-113">interval</span></span>|<span data-ttu-id="7e75c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7e75c-114">Int32</span></span>|<span data-ttu-id="7e75c-115">Intervall in Tagen</span><span class="sxs-lookup"><span data-stu-id="7e75c-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e75c-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e75c-116">Relationships</span></span>
<span data-ttu-id="7e75c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7e75c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e75c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e75c-118">JSON Representation</span></span>
<span data-ttu-id="7e75c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e75c-119">Here is a JSON representation of the resource.</span></span>
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





