---
title: Ressourcentyp dailySchedule
description: Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d0f4f258afe1de65bd8fecf32d9df387716a2c6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987713"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="c4c13-103">Ressourcentyp dailySchedule</span><span class="sxs-lookup"><span data-stu-id="c4c13-103">dailySchedule resource type</span></span>

> <span data-ttu-id="c4c13-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c4c13-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4c13-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4c13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4c13-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c4c13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4c13-107">Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.</span><span class="sxs-lookup"><span data-stu-id="c4c13-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="c4c13-108">Erbt vom [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c4c13-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4c13-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c4c13-109">Properties</span></span>
|<span data-ttu-id="c4c13-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4c13-110">Property</span></span>|<span data-ttu-id="c4c13-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c4c13-111">Type</span></span>|<span data-ttu-id="c4c13-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4c13-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4c13-113">Intervall</span><span class="sxs-lookup"><span data-stu-id="c4c13-113">interval</span></span>|<span data-ttu-id="c4c13-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c4c13-114">Int32</span></span>|<span data-ttu-id="c4c13-115">Intervall in Tagen</span><span class="sxs-lookup"><span data-stu-id="c4c13-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4c13-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c4c13-116">Relationships</span></span>
<span data-ttu-id="c4c13-117">Keine</span><span class="sxs-lookup"><span data-stu-id="c4c13-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4c13-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c4c13-118">JSON Representation</span></span>
<span data-ttu-id="c4c13-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c4c13-119">Here is a JSON representation of the resource.</span></span>
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





