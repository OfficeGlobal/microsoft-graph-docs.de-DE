---
title: locateDeviceActionResult-Ressourcentyp
description: Gerät suchen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 246fcae2a9a51822f97d7f193ff6056bee55db26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923495"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="d2d90-103">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2d90-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="d2d90-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2d90-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2d90-105">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="d2d90-105">Locate device action result</span></span>

<span data-ttu-id="d2d90-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d2d90-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2d90-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2d90-107">Properties</span></span>
|<span data-ttu-id="d2d90-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2d90-108">Property</span></span>|<span data-ttu-id="d2d90-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d2d90-109">Type</span></span>|<span data-ttu-id="d2d90-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2d90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d90-111">actionName</span><span class="sxs-lookup"><span data-stu-id="d2d90-111">actionName</span></span>|<span data-ttu-id="d2d90-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d2d90-112">String</span></span>|<span data-ttu-id="d2d90-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d2d90-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d2d90-114">actionState</span><span class="sxs-lookup"><span data-stu-id="d2d90-114">actionState</span></span>|[<span data-ttu-id="d2d90-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d2d90-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="d2d90-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d2d90-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d2d90-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d2d90-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d2d90-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d90-118">startDateTime</span></span>|<span data-ttu-id="d2d90-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d90-119">DateTimeOffset</span></span>|<span data-ttu-id="d2d90-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d2d90-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d2d90-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d90-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="d2d90-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d90-122">DateTimeOffset</span></span>|<span data-ttu-id="d2d90-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d2d90-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d2d90-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="d2d90-124">deviceLocation</span></span>|[<span data-ttu-id="d2d90-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="d2d90-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="d2d90-126">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="d2d90-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2d90-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d2d90-127">Relationships</span></span>
<span data-ttu-id="d2d90-128">Keine</span><span class="sxs-lookup"><span data-stu-id="d2d90-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2d90-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2d90-129">JSON Representation</span></span>
<span data-ttu-id="d2d90-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d2d90-130">Here is a JSON representation of the resource.</span></span>
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



