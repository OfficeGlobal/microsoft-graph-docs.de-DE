---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1eaa46929ae627dbf6cdee8d300b7910b4817ffc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149602"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="93bab-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93bab-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="93bab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93bab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93bab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="93bab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93bab-106">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="93bab-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="93bab-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93bab-107">Properties</span></span>
|<span data-ttu-id="93bab-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93bab-108">Property</span></span>|<span data-ttu-id="93bab-109">Typ</span><span class="sxs-lookup"><span data-stu-id="93bab-109">Type</span></span>|<span data-ttu-id="93bab-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93bab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93bab-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="93bab-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="93bab-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93bab-112">DateTimeOffset</span></span>|<span data-ttu-id="93bab-113">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="93bab-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="93bab-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="93bab-114">lastCollectedDateTime</span></span>|<span data-ttu-id="93bab-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93bab-115">DateTimeOffset</span></span>|<span data-ttu-id="93bab-116">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="93bab-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="93bab-117">longitude</span><span class="sxs-lookup"><span data-stu-id="93bab-117">longitude</span></span>|<span data-ttu-id="93bab-118">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="93bab-118">Double</span></span>|<span data-ttu-id="93bab-119">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="93bab-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="93bab-120">latitude</span><span class="sxs-lookup"><span data-stu-id="93bab-120">latitude</span></span>|<span data-ttu-id="93bab-121">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="93bab-121">Double</span></span>|<span data-ttu-id="93bab-122">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="93bab-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="93bab-123">altitude</span><span class="sxs-lookup"><span data-stu-id="93bab-123">altitude</span></span>|<span data-ttu-id="93bab-124">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="93bab-124">Double</span></span>|<span data-ttu-id="93bab-125">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="93bab-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="93bab-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="93bab-126">horizontalAccuracy</span></span>|<span data-ttu-id="93bab-127">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="93bab-127">Double</span></span>|<span data-ttu-id="93bab-128">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="93bab-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="93bab-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="93bab-129">verticalAccuracy</span></span>|<span data-ttu-id="93bab-130">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="93bab-130">Double</span></span>|<span data-ttu-id="93bab-131">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="93bab-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="93bab-132">heading</span><span class="sxs-lookup"><span data-stu-id="93bab-132">heading</span></span>|<span data-ttu-id="93bab-133">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="93bab-133">Double</span></span>|<span data-ttu-id="93bab-134">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="93bab-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="93bab-135">speed</span><span class="sxs-lookup"><span data-stu-id="93bab-135">speed</span></span>|<span data-ttu-id="93bab-136">Double</span><span class="sxs-lookup"><span data-stu-id="93bab-136">Double</span></span>|<span data-ttu-id="93bab-137">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="93bab-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="93bab-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="93bab-138">Relationships</span></span>
<span data-ttu-id="93bab-139">Keine</span><span class="sxs-lookup"><span data-stu-id="93bab-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93bab-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93bab-140">JSON Representation</span></span>
<span data-ttu-id="93bab-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93bab-141">Here is a JSON representation of the resource.</span></span>
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




