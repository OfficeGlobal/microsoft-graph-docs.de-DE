---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68e89b2e63b99324332874a3ad6a2f2e3c335832
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816128"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="d90bb-103">deviceGeoLocation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d90bb-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="d90bb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d90bb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d90bb-105">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="d90bb-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="d90bb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d90bb-106">Properties</span></span>
|<span data-ttu-id="d90bb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d90bb-107">Property</span></span>|<span data-ttu-id="d90bb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d90bb-108">Type</span></span>|<span data-ttu-id="d90bb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d90bb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90bb-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="d90bb-110">lastCollectedDateTime</span></span>|<span data-ttu-id="d90bb-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d90bb-111">DateTimeOffset</span></span>|<span data-ttu-id="d90bb-112">Zeit der Aufzeichnung des Standorts, relativ zu UTC</span><span class="sxs-lookup"><span data-stu-id="d90bb-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="d90bb-113">longitude</span><span class="sxs-lookup"><span data-stu-id="d90bb-113">longitude</span></span>|<span data-ttu-id="d90bb-114">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-114">Double</span></span>|<span data-ttu-id="d90bb-115">Längengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="d90bb-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="d90bb-116">latitude</span><span class="sxs-lookup"><span data-stu-id="d90bb-116">latitude</span></span>|<span data-ttu-id="d90bb-117">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-117">Double</span></span>|<span data-ttu-id="d90bb-118">Breitengrad-Koordinate des Gerätestandorts</span><span class="sxs-lookup"><span data-stu-id="d90bb-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="d90bb-119">altitude</span><span class="sxs-lookup"><span data-stu-id="d90bb-119">altitude</span></span>|<span data-ttu-id="d90bb-120">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-120">Double</span></span>|<span data-ttu-id="d90bb-121">Höhe in Metern über dem Meeresspiegel</span><span class="sxs-lookup"><span data-stu-id="d90bb-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="d90bb-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="d90bb-122">horizontalAccuracy</span></span>|<span data-ttu-id="d90bb-123">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-123">Double</span></span>|<span data-ttu-id="d90bb-124">Genauigkeit von Länge und Breite in Metern</span><span class="sxs-lookup"><span data-stu-id="d90bb-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="d90bb-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="d90bb-125">verticalAccuracy</span></span>|<span data-ttu-id="d90bb-126">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-126">Double</span></span>|<span data-ttu-id="d90bb-127">Genauigkeit der Höhe in Metern</span><span class="sxs-lookup"><span data-stu-id="d90bb-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="d90bb-128">heading</span><span class="sxs-lookup"><span data-stu-id="d90bb-128">heading</span></span>|<span data-ttu-id="d90bb-129">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-129">Double</span></span>|<span data-ttu-id="d90bb-130">Kurs in Grad vom geografischen Norden</span><span class="sxs-lookup"><span data-stu-id="d90bb-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="d90bb-131">speed</span><span class="sxs-lookup"><span data-stu-id="d90bb-131">speed</span></span>|<span data-ttu-id="d90bb-132">Double</span><span class="sxs-lookup"><span data-stu-id="d90bb-132">Double</span></span>|<span data-ttu-id="d90bb-133">Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde</span><span class="sxs-lookup"><span data-stu-id="d90bb-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="d90bb-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d90bb-134">Relationships</span></span>
<span data-ttu-id="d90bb-135">Keine</span><span class="sxs-lookup"><span data-stu-id="d90bb-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d90bb-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d90bb-136">JSON Representation</span></span>
<span data-ttu-id="d90bb-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d90bb-137">Here is a JSON representation of the resource.</span></span>
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



