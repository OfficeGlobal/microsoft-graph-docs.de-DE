---
title: locateDeviceActionResult-Ressourcentyp
description: Gerät suchen – Aktionsergebnis
author: tfitzmac
ms.openlocfilehash: 82f8b5ba1bd1f1ce1584af50a4a2b3037e588adc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345451"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="23ead-103">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23ead-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="23ead-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23ead-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23ead-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23ead-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23ead-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23ead-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23ead-107">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="23ead-107">Locate device action result</span></span>

<span data-ttu-id="23ead-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23ead-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23ead-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23ead-109">Properties</span></span>
|<span data-ttu-id="23ead-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23ead-110">Property</span></span>|<span data-ttu-id="23ead-111">Typ</span><span class="sxs-lookup"><span data-stu-id="23ead-111">Type</span></span>|<span data-ttu-id="23ead-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23ead-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ead-113">actionName</span><span class="sxs-lookup"><span data-stu-id="23ead-113">actionName</span></span>|<span data-ttu-id="23ead-114">String</span><span class="sxs-lookup"><span data-stu-id="23ead-114">String</span></span>|<span data-ttu-id="23ead-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23ead-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23ead-116">actionState</span><span class="sxs-lookup"><span data-stu-id="23ead-116">actionState</span></span>|[<span data-ttu-id="23ead-117">actionState</span><span class="sxs-lookup"><span data-stu-id="23ead-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="23ead-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="23ead-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="23ead-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="23ead-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="23ead-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="23ead-120">startDateTime</span></span>|<span data-ttu-id="23ead-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ead-121">DateTimeOffset</span></span>|<span data-ttu-id="23ead-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23ead-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23ead-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="23ead-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="23ead-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ead-124">DateTimeOffset</span></span>|<span data-ttu-id="23ead-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23ead-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23ead-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="23ead-126">deviceLocation</span></span>|[<span data-ttu-id="23ead-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="23ead-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="23ead-128">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="23ead-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="23ead-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23ead-129">Relationships</span></span>
<span data-ttu-id="23ead-130">Keine</span><span class="sxs-lookup"><span data-stu-id="23ead-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23ead-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23ead-131">JSON Representation</span></span>
<span data-ttu-id="23ead-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23ead-132">Here is a JSON representation of the resource.</span></span>
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





