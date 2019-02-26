---
title: locateDeviceActionResult-Ressourcentyp
description: Gerät suchen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c335ac49bcf053e58381f7c1111caf5ae70cb0fd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255353"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="3d0b2-103">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3d0b2-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="3d0b2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3d0b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d0b2-105">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="3d0b2-105">Locate device action result</span></span>


<span data-ttu-id="3d0b2-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3d0b2-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d0b2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d0b2-107">Properties</span></span>
|<span data-ttu-id="3d0b2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d0b2-108">Property</span></span>|<span data-ttu-id="3d0b2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3d0b2-109">Type</span></span>|<span data-ttu-id="3d0b2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d0b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d0b2-111">actionName</span><span class="sxs-lookup"><span data-stu-id="3d0b2-111">actionName</span></span>|<span data-ttu-id="3d0b2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d0b2-112">String</span></span>|<span data-ttu-id="3d0b2-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3d0b2-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3d0b2-114">actionState</span><span class="sxs-lookup"><span data-stu-id="3d0b2-114">actionState</span></span>|[<span data-ttu-id="3d0b2-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3d0b2-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3d0b2-116">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="3d0b2-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3d0b2-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3d0b2-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3d0b2-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3d0b2-118">startDateTime</span></span>|<span data-ttu-id="3d0b2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d0b2-119">DateTimeOffset</span></span>|<span data-ttu-id="3d0b2-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3d0b2-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3d0b2-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d0b2-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="3d0b2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d0b2-122">DateTimeOffset</span></span>|<span data-ttu-id="3d0b2-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3d0b2-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3d0b2-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="3d0b2-124">deviceLocation</span></span>|[<span data-ttu-id="3d0b2-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="3d0b2-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="3d0b2-126">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="3d0b2-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d0b2-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3d0b2-127">Relationships</span></span>
<span data-ttu-id="3d0b2-128">Keine</span><span class="sxs-lookup"><span data-stu-id="3d0b2-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d0b2-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d0b2-129">JSON Representation</span></span>
<span data-ttu-id="3d0b2-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d0b2-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```



