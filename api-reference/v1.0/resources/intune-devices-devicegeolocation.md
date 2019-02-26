---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260214"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="45585-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="45585-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="45585-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="45585-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45585-105">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="45585-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="45585-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45585-106">Properties</span></span>
|<span data-ttu-id="45585-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45585-107">Property</span></span>|<span data-ttu-id="45585-108">Typ</span><span class="sxs-lookup"><span data-stu-id="45585-108">Type</span></span>|<span data-ttu-id="45585-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45585-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45585-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="45585-110">lastCollectedDateTime</span></span>|<span data-ttu-id="45585-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45585-111">DateTimeOffset</span></span>|<span data-ttu-id="45585-112">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="45585-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="45585-113">longitude</span><span class="sxs-lookup"><span data-stu-id="45585-113">longitude</span></span>|<span data-ttu-id="45585-114">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="45585-114">Double</span></span>|<span data-ttu-id="45585-115">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="45585-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="45585-116">latitude</span><span class="sxs-lookup"><span data-stu-id="45585-116">latitude</span></span>|<span data-ttu-id="45585-117">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="45585-117">Double</span></span>|<span data-ttu-id="45585-118">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="45585-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="45585-119">altitude</span><span class="sxs-lookup"><span data-stu-id="45585-119">altitude</span></span>|<span data-ttu-id="45585-120">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="45585-120">Double</span></span>|<span data-ttu-id="45585-121">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="45585-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="45585-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="45585-122">horizontalAccuracy</span></span>|<span data-ttu-id="45585-123">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="45585-123">Double</span></span>|<span data-ttu-id="45585-124">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="45585-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="45585-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="45585-125">verticalAccuracy</span></span>|<span data-ttu-id="45585-126">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="45585-126">Double</span></span>|<span data-ttu-id="45585-127">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="45585-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="45585-128">heading</span><span class="sxs-lookup"><span data-stu-id="45585-128">heading</span></span>|<span data-ttu-id="45585-129">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="45585-129">Double</span></span>|<span data-ttu-id="45585-130">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="45585-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="45585-131">speed</span><span class="sxs-lookup"><span data-stu-id="45585-131">speed</span></span>|<span data-ttu-id="45585-132">Double</span><span class="sxs-lookup"><span data-stu-id="45585-132">Double</span></span>|<span data-ttu-id="45585-133">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="45585-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="45585-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="45585-134">Relationships</span></span>
<span data-ttu-id="45585-135">Keine</span><span class="sxs-lookup"><span data-stu-id="45585-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45585-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45585-136">JSON Representation</span></span>
<span data-ttu-id="45585-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45585-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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



