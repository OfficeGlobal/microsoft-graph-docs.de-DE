---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd81a0665d3d85a10488f78245449d265c85a8cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845262"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="1c347-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1c347-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="1c347-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c347-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c347-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c347-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c347-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c347-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c347-107">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="1c347-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="1c347-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1c347-108">Properties</span></span>
|<span data-ttu-id="1c347-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c347-109">Property</span></span>|<span data-ttu-id="1c347-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1c347-110">Type</span></span>|<span data-ttu-id="1c347-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c347-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c347-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="1c347-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="1c347-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c347-113">DateTimeOffset</span></span>|<span data-ttu-id="1c347-114">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="1c347-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="1c347-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c347-115">lastCollectedDateTime</span></span>|<span data-ttu-id="1c347-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c347-116">DateTimeOffset</span></span>|<span data-ttu-id="1c347-117">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="1c347-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="1c347-118">longitude</span><span class="sxs-lookup"><span data-stu-id="1c347-118">longitude</span></span>|<span data-ttu-id="1c347-119">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-119">Double</span></span>|<span data-ttu-id="1c347-120">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="1c347-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="1c347-121">latitude</span><span class="sxs-lookup"><span data-stu-id="1c347-121">latitude</span></span>|<span data-ttu-id="1c347-122">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-122">Double</span></span>|<span data-ttu-id="1c347-123">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="1c347-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="1c347-124">altitude</span><span class="sxs-lookup"><span data-stu-id="1c347-124">altitude</span></span>|<span data-ttu-id="1c347-125">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-125">Double</span></span>|<span data-ttu-id="1c347-126">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="1c347-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="1c347-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="1c347-127">horizontalAccuracy</span></span>|<span data-ttu-id="1c347-128">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-128">Double</span></span>|<span data-ttu-id="1c347-129">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="1c347-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="1c347-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="1c347-130">verticalAccuracy</span></span>|<span data-ttu-id="1c347-131">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-131">Double</span></span>|<span data-ttu-id="1c347-132">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="1c347-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="1c347-133">heading</span><span class="sxs-lookup"><span data-stu-id="1c347-133">heading</span></span>|<span data-ttu-id="1c347-134">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-134">Double</span></span>|<span data-ttu-id="1c347-135">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="1c347-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="1c347-136">speed</span><span class="sxs-lookup"><span data-stu-id="1c347-136">speed</span></span>|<span data-ttu-id="1c347-137">Double</span><span class="sxs-lookup"><span data-stu-id="1c347-137">Double</span></span>|<span data-ttu-id="1c347-138">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="1c347-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c347-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1c347-139">Relationships</span></span>
<span data-ttu-id="1c347-140">Keine</span><span class="sxs-lookup"><span data-stu-id="1c347-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c347-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1c347-141">JSON Representation</span></span>
<span data-ttu-id="1c347-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c347-142">Here is a JSON representation of the resource.</span></span>
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





