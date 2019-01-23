---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395055"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="fc731-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fc731-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="fc731-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fc731-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc731-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc731-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc731-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc731-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc731-107">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="fc731-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="fc731-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc731-108">Properties</span></span>
|<span data-ttu-id="fc731-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc731-109">Property</span></span>|<span data-ttu-id="fc731-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fc731-110">Type</span></span>|<span data-ttu-id="fc731-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc731-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc731-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="fc731-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="fc731-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc731-113">DateTimeOffset</span></span>|<span data-ttu-id="fc731-114">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="fc731-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="fc731-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc731-115">lastCollectedDateTime</span></span>|<span data-ttu-id="fc731-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc731-116">DateTimeOffset</span></span>|<span data-ttu-id="fc731-117">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="fc731-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="fc731-118">longitude</span><span class="sxs-lookup"><span data-stu-id="fc731-118">longitude</span></span>|<span data-ttu-id="fc731-119">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-119">Double</span></span>|<span data-ttu-id="fc731-120">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="fc731-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="fc731-121">latitude</span><span class="sxs-lookup"><span data-stu-id="fc731-121">latitude</span></span>|<span data-ttu-id="fc731-122">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-122">Double</span></span>|<span data-ttu-id="fc731-123">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="fc731-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="fc731-124">altitude</span><span class="sxs-lookup"><span data-stu-id="fc731-124">altitude</span></span>|<span data-ttu-id="fc731-125">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-125">Double</span></span>|<span data-ttu-id="fc731-126">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="fc731-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="fc731-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="fc731-127">horizontalAccuracy</span></span>|<span data-ttu-id="fc731-128">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-128">Double</span></span>|<span data-ttu-id="fc731-129">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="fc731-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="fc731-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="fc731-130">verticalAccuracy</span></span>|<span data-ttu-id="fc731-131">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-131">Double</span></span>|<span data-ttu-id="fc731-132">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="fc731-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="fc731-133">heading</span><span class="sxs-lookup"><span data-stu-id="fc731-133">heading</span></span>|<span data-ttu-id="fc731-134">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-134">Double</span></span>|<span data-ttu-id="fc731-135">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="fc731-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="fc731-136">speed</span><span class="sxs-lookup"><span data-stu-id="fc731-136">speed</span></span>|<span data-ttu-id="fc731-137">Double</span><span class="sxs-lookup"><span data-stu-id="fc731-137">Double</span></span>|<span data-ttu-id="fc731-138">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="fc731-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc731-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc731-139">Relationships</span></span>
<span data-ttu-id="fc731-140">Keine</span><span class="sxs-lookup"><span data-stu-id="fc731-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc731-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc731-141">JSON Representation</span></span>
<span data-ttu-id="fc731-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc731-142">Here is a JSON representation of the resource.</span></span>
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




