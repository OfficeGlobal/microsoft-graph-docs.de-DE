---
title: Ressourcentyp dailySchedule
description: Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.
ms.openlocfilehash: 5d517b0bcd15f041b934a0ca936075bc6d3d3741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063811"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="76692-103">Ressourcentyp dailySchedule</span><span class="sxs-lookup"><span data-stu-id="76692-103">dailySchedule resource type</span></span>

> <span data-ttu-id="76692-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="76692-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76692-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76692-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76692-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="76692-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76692-107">Ausführen Tagesplans eines sich wiederholenden Gerät Management Skripts.</span><span class="sxs-lookup"><span data-stu-id="76692-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="76692-108">Erbt vom [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="76692-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76692-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="76692-109">Properties</span></span>
|<span data-ttu-id="76692-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76692-110">Property</span></span>|<span data-ttu-id="76692-111">Typ</span><span class="sxs-lookup"><span data-stu-id="76692-111">Type</span></span>|<span data-ttu-id="76692-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76692-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76692-113">Intervall</span><span class="sxs-lookup"><span data-stu-id="76692-113">interval</span></span>|<span data-ttu-id="76692-114">Int32</span><span class="sxs-lookup"><span data-stu-id="76692-114">Int32</span></span>|<span data-ttu-id="76692-115">Intervall in Tagen</span><span class="sxs-lookup"><span data-stu-id="76692-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="76692-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="76692-116">Relationships</span></span>
<span data-ttu-id="76692-117">Keine</span><span class="sxs-lookup"><span data-stu-id="76692-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76692-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="76692-118">JSON Representation</span></span>
<span data-ttu-id="76692-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="76692-119">Here is a JSON representation of the resource.</span></span>
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





