---
title: locateDeviceActionResult-Ressourcentyp
description: Gerät suchen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f4c9e1dc914c8648df2924308942bd5f83204aa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154117"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="d9d4a-103">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d9d4a-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="d9d4a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9d4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9d4a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d9d4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9d4a-106">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="d9d4a-106">Locate device action result</span></span>


<span data-ttu-id="d9d4a-107">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9d4a-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9d4a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d9d4a-108">Properties</span></span>
|<span data-ttu-id="d9d4a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9d4a-109">Property</span></span>|<span data-ttu-id="d9d4a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d9d4a-110">Type</span></span>|<span data-ttu-id="d9d4a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9d4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9d4a-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d9d4a-112">actionName</span></span>|<span data-ttu-id="d9d4a-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d9d4a-113">String</span></span>|<span data-ttu-id="d9d4a-114">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9d4a-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d9d4a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d9d4a-115">actionState</span></span>|[<span data-ttu-id="d9d4a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d9d4a-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d9d4a-117">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="d9d4a-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d9d4a-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d9d4a-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d9d4a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d9d4a-119">startDateTime</span></span>|<span data-ttu-id="d9d4a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9d4a-120">DateTimeOffset</span></span>|<span data-ttu-id="d9d4a-121">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9d4a-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d9d4a-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9d4a-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d9d4a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9d4a-123">DateTimeOffset</span></span>|<span data-ttu-id="d9d4a-124">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9d4a-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d9d4a-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="d9d4a-125">deviceLocation</span></span>|[<span data-ttu-id="d9d4a-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="d9d4a-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="d9d4a-127">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="d9d4a-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9d4a-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d9d4a-128">Relationships</span></span>
<span data-ttu-id="d9d4a-129">Keine</span><span class="sxs-lookup"><span data-stu-id="d9d4a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9d4a-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d9d4a-130">JSON Representation</span></span>
<span data-ttu-id="d9d4a-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d9d4a-131">Here is a JSON representation of the resource.</span></span>
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
}
```




