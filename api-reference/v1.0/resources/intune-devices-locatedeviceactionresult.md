---
title: locateDeviceActionResult-Ressourcentyp
description: Gerät suchen – Aktionsergebnis
author: tfitzmac
ms.openlocfilehash: a12919e273f8e84d177ec3982756cb20363ffffe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306314"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="0fbf3-103">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0fbf3-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="0fbf3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0fbf3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fbf3-105">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="0fbf3-105">Locate device action result</span></span>

<span data-ttu-id="0fbf3-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0fbf3-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0fbf3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0fbf3-107">Properties</span></span>
|<span data-ttu-id="0fbf3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fbf3-108">Property</span></span>|<span data-ttu-id="0fbf3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0fbf3-109">Type</span></span>|<span data-ttu-id="0fbf3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fbf3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fbf3-111">actionName</span><span class="sxs-lookup"><span data-stu-id="0fbf3-111">actionName</span></span>|<span data-ttu-id="0fbf3-112">String</span><span class="sxs-lookup"><span data-stu-id="0fbf3-112">String</span></span>|<span data-ttu-id="0fbf3-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0fbf3-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0fbf3-114">actionState</span><span class="sxs-lookup"><span data-stu-id="0fbf3-114">actionState</span></span>|[<span data-ttu-id="0fbf3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0fbf3-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="0fbf3-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0fbf3-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0fbf3-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0fbf3-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0fbf3-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0fbf3-118">startDateTime</span></span>|<span data-ttu-id="0fbf3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbf3-119">DateTimeOffset</span></span>|<span data-ttu-id="0fbf3-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0fbf3-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0fbf3-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fbf3-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="0fbf3-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbf3-122">DateTimeOffset</span></span>|<span data-ttu-id="0fbf3-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0fbf3-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0fbf3-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="0fbf3-124">deviceLocation</span></span>|[<span data-ttu-id="0fbf3-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="0fbf3-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="0fbf3-126">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="0fbf3-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fbf3-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0fbf3-127">Relationships</span></span>
<span data-ttu-id="0fbf3-128">Keine</span><span class="sxs-lookup"><span data-stu-id="0fbf3-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0fbf3-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0fbf3-129">JSON Representation</span></span>
<span data-ttu-id="0fbf3-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0fbf3-130">Here is a JSON representation of the resource.</span></span>
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



