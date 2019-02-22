---
title: windowsKioskLocalGroup-Ressourcentyp
description: Die Klasse, die zum Identifizieren einer lokalen Gruppe für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3479226d770c7030fefed1a7f2f65a02808479d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169524"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="7fe02-103">windowsKioskLocalGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7fe02-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="7fe02-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7fe02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fe02-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7fe02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fe02-106">Die Klasse, die zum Identifizieren einer lokalen Gruppe für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="7fe02-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="7fe02-107">Erbt von [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="7fe02-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7fe02-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7fe02-108">Properties</span></span>
|<span data-ttu-id="7fe02-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7fe02-109">Property</span></span>|<span data-ttu-id="7fe02-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7fe02-110">Type</span></span>|<span data-ttu-id="7fe02-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7fe02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fe02-112">groupName</span><span class="sxs-lookup"><span data-stu-id="7fe02-112">groupName</span></span>|<span data-ttu-id="7fe02-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fe02-113">String</span></span>|<span data-ttu-id="7fe02-114">Der Name der lokalen Gruppe, die für diese Kiosk Konfiguration gesperrt wird.</span><span class="sxs-lookup"><span data-stu-id="7fe02-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fe02-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7fe02-115">Relationships</span></span>
<span data-ttu-id="7fe02-116">Keine</span><span class="sxs-lookup"><span data-stu-id="7fe02-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fe02-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7fe02-117">JSON Representation</span></span>
<span data-ttu-id="7fe02-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7fe02-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```




