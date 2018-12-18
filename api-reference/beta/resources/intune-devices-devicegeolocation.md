---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
ms.openlocfilehash: b3e790809f79d8d943cc12cc0e5065972c9864ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328630"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="3b9f8-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3b9f8-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="3b9f8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b9f8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b9f8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b9f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b9f8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b9f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b9f8-107">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="3b9f8-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="3b9f8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b9f8-108">Properties</span></span>
|<span data-ttu-id="3b9f8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b9f8-109">Property</span></span>|<span data-ttu-id="3b9f8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3b9f8-110">Type</span></span>|<span data-ttu-id="3b9f8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b9f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b9f8-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="3b9f8-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="3b9f8-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b9f8-113">DateTimeOffset</span></span>|<span data-ttu-id="3b9f8-114">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="3b9f8-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3b9f8-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b9f8-115">lastCollectedDateTime</span></span>|<span data-ttu-id="3b9f8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b9f8-116">DateTimeOffset</span></span>|<span data-ttu-id="3b9f8-117">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="3b9f8-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3b9f8-118">longitude</span><span class="sxs-lookup"><span data-stu-id="3b9f8-118">longitude</span></span>|<span data-ttu-id="3b9f8-119">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-119">Double</span></span>|<span data-ttu-id="3b9f8-120">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="3b9f8-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3b9f8-121">latitude</span><span class="sxs-lookup"><span data-stu-id="3b9f8-121">latitude</span></span>|<span data-ttu-id="3b9f8-122">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-122">Double</span></span>|<span data-ttu-id="3b9f8-123">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="3b9f8-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3b9f8-124">altitude</span><span class="sxs-lookup"><span data-stu-id="3b9f8-124">altitude</span></span>|<span data-ttu-id="3b9f8-125">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-125">Double</span></span>|<span data-ttu-id="3b9f8-126">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="3b9f8-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="3b9f8-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3b9f8-127">horizontalAccuracy</span></span>|<span data-ttu-id="3b9f8-128">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-128">Double</span></span>|<span data-ttu-id="3b9f8-129">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="3b9f8-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="3b9f8-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3b9f8-130">verticalAccuracy</span></span>|<span data-ttu-id="3b9f8-131">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-131">Double</span></span>|<span data-ttu-id="3b9f8-132">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="3b9f8-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="3b9f8-133">heading</span><span class="sxs-lookup"><span data-stu-id="3b9f8-133">heading</span></span>|<span data-ttu-id="3b9f8-134">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-134">Double</span></span>|<span data-ttu-id="3b9f8-135">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="3b9f8-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="3b9f8-136">speed</span><span class="sxs-lookup"><span data-stu-id="3b9f8-136">speed</span></span>|<span data-ttu-id="3b9f8-137">Double</span><span class="sxs-lookup"><span data-stu-id="3b9f8-137">Double</span></span>|<span data-ttu-id="3b9f8-138">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="3b9f8-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b9f8-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3b9f8-139">Relationships</span></span>
<span data-ttu-id="3b9f8-140">Keine</span><span class="sxs-lookup"><span data-stu-id="3b9f8-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b9f8-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b9f8-141">JSON Representation</span></span>
<span data-ttu-id="3b9f8-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b9f8-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```





