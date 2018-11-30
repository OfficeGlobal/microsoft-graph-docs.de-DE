---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
ms.openlocfilehash: 1bc72e4fb2d01c55d5d16ff2a45a020c5eaf99e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018983"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="8ef29-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8ef29-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="8ef29-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8ef29-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ef29-105">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="8ef29-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="8ef29-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ef29-106">Properties</span></span>
|<span data-ttu-id="8ef29-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ef29-107">Property</span></span>|<span data-ttu-id="8ef29-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8ef29-108">Type</span></span>|<span data-ttu-id="8ef29-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ef29-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ef29-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef29-110">lastCollectedDateTime</span></span>|<span data-ttu-id="8ef29-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef29-111">DateTimeOffset</span></span>|<span data-ttu-id="8ef29-112">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="8ef29-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="8ef29-113">longitude</span><span class="sxs-lookup"><span data-stu-id="8ef29-113">longitude</span></span>|<span data-ttu-id="8ef29-114">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-114">Double</span></span>|<span data-ttu-id="8ef29-115">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="8ef29-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="8ef29-116">latitude</span><span class="sxs-lookup"><span data-stu-id="8ef29-116">latitude</span></span>|<span data-ttu-id="8ef29-117">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-117">Double</span></span>|<span data-ttu-id="8ef29-118">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="8ef29-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="8ef29-119">altitude</span><span class="sxs-lookup"><span data-stu-id="8ef29-119">altitude</span></span>|<span data-ttu-id="8ef29-120">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-120">Double</span></span>|<span data-ttu-id="8ef29-121">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="8ef29-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="8ef29-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="8ef29-122">horizontalAccuracy</span></span>|<span data-ttu-id="8ef29-123">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-123">Double</span></span>|<span data-ttu-id="8ef29-124">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="8ef29-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="8ef29-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="8ef29-125">verticalAccuracy</span></span>|<span data-ttu-id="8ef29-126">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-126">Double</span></span>|<span data-ttu-id="8ef29-127">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="8ef29-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="8ef29-128">heading</span><span class="sxs-lookup"><span data-stu-id="8ef29-128">heading</span></span>|<span data-ttu-id="8ef29-129">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-129">Double</span></span>|<span data-ttu-id="8ef29-130">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="8ef29-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="8ef29-131">speed</span><span class="sxs-lookup"><span data-stu-id="8ef29-131">speed</span></span>|<span data-ttu-id="8ef29-132">Double</span><span class="sxs-lookup"><span data-stu-id="8ef29-132">Double</span></span>|<span data-ttu-id="8ef29-133">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="8ef29-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ef29-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8ef29-134">Relationships</span></span>
<span data-ttu-id="8ef29-135">Keine</span><span class="sxs-lookup"><span data-stu-id="8ef29-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ef29-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ef29-136">JSON Representation</span></span>
<span data-ttu-id="8ef29-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ef29-137">Here is a JSON representation of the resource.</span></span>
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



