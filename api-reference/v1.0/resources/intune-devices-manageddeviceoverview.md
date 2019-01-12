---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7a5abdd3b5455272de7d1cf73044a1356d728dd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981196"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="83787-103">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="83787-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="83787-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83787-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83787-105">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="83787-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="83787-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="83787-106">Methods</span></span>
|<span data-ttu-id="83787-107">Methode</span><span class="sxs-lookup"><span data-stu-id="83787-107">Method</span></span>|<span data-ttu-id="83787-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="83787-108">Return Type</span></span>|<span data-ttu-id="83787-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83787-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83787-110">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="83787-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="83787-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83787-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="83787-112">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="83787-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="83787-113">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="83787-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="83787-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83787-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="83787-115">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="83787-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83787-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83787-116">Properties</span></span>
|<span data-ttu-id="83787-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83787-117">Property</span></span>|<span data-ttu-id="83787-118">Typ</span><span class="sxs-lookup"><span data-stu-id="83787-118">Type</span></span>|<span data-ttu-id="83787-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83787-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83787-120">id</span><span class="sxs-lookup"><span data-stu-id="83787-120">id</span></span>|<span data-ttu-id="83787-121">String</span><span class="sxs-lookup"><span data-stu-id="83787-121">String</span></span>|<span data-ttu-id="83787-122">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="83787-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="83787-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83787-123">enrolledDeviceCount</span></span>|<span data-ttu-id="83787-124">Int32</span><span class="sxs-lookup"><span data-stu-id="83787-124">Int32</span></span>|<span data-ttu-id="83787-125">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="83787-125">Total enrolled device count.</span></span> <span data-ttu-id="83787-126">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="83787-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="83787-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="83787-127">mdmEnrolledCount</span></span>|<span data-ttu-id="83787-128">Int32</span><span class="sxs-lookup"><span data-stu-id="83787-128">Int32</span></span>|<span data-ttu-id="83787-129">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="83787-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="83787-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83787-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="83787-131">Int32</span><span class="sxs-lookup"><span data-stu-id="83787-131">Int32</span></span>|<span data-ttu-id="83787-132">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="83787-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="83787-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="83787-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="83787-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="83787-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="83787-135">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="83787-135">Device operating system summary.</span></span>|
|<span data-ttu-id="83787-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="83787-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="83787-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="83787-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="83787-138">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="83787-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="83787-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83787-139">Relationships</span></span>
<span data-ttu-id="83787-140">Keine</span><span class="sxs-lookup"><span data-stu-id="83787-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83787-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83787-141">JSON Representation</span></span>
<span data-ttu-id="83787-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83787-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



