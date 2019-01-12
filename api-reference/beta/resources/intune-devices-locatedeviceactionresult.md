---
title: locateDeviceActionResult-Ressourcentyp
description: Gerät suchen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f342f26916b1144a317d02871364e25da2d8c4d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912456"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="b0770-103">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b0770-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="b0770-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b0770-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0770-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0770-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0770-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b0770-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0770-107">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="b0770-107">Locate device action result</span></span>

<span data-ttu-id="b0770-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0770-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0770-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b0770-109">Properties</span></span>
|<span data-ttu-id="b0770-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0770-110">Property</span></span>|<span data-ttu-id="b0770-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b0770-111">Type</span></span>|<span data-ttu-id="b0770-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0770-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0770-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b0770-113">actionName</span></span>|<span data-ttu-id="b0770-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0770-114">String</span></span>|<span data-ttu-id="b0770-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0770-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0770-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b0770-116">actionState</span></span>|[<span data-ttu-id="b0770-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b0770-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b0770-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0770-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b0770-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b0770-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b0770-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0770-120">startDateTime</span></span>|<span data-ttu-id="b0770-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0770-121">DateTimeOffset</span></span>|<span data-ttu-id="b0770-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0770-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0770-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0770-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b0770-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0770-124">DateTimeOffset</span></span>|<span data-ttu-id="b0770-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0770-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0770-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="b0770-126">deviceLocation</span></span>|[<span data-ttu-id="b0770-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="b0770-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="b0770-128">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="b0770-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0770-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b0770-129">Relationships</span></span>
<span data-ttu-id="b0770-130">Keine</span><span class="sxs-lookup"><span data-stu-id="b0770-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0770-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b0770-131">JSON Representation</span></span>
<span data-ttu-id="b0770-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b0770-132">Here is a JSON representation of the resource.</span></span>
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





