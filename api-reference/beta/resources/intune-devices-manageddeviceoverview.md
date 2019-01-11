---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1eeb349e8ec77adce3d69df9d61f43e43fb3b770
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872548"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="9b904-103">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9b904-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="9b904-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b904-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b904-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b904-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b904-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b904-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b904-107">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="9b904-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="9b904-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="9b904-108">Methods</span></span>
|<span data-ttu-id="9b904-109">Methode</span><span class="sxs-lookup"><span data-stu-id="9b904-109">Method</span></span>|<span data-ttu-id="9b904-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9b904-110">Return Type</span></span>|<span data-ttu-id="9b904-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b904-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b904-112">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="9b904-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="9b904-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9b904-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="9b904-114">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b904-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="9b904-115">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9b904-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="9b904-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9b904-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="9b904-117">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b904-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b904-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9b904-118">Properties</span></span>
|<span data-ttu-id="9b904-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9b904-119">Property</span></span>|<span data-ttu-id="9b904-120">Typ</span><span class="sxs-lookup"><span data-stu-id="9b904-120">Type</span></span>|<span data-ttu-id="9b904-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b904-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b904-122">id</span><span class="sxs-lookup"><span data-stu-id="9b904-122">id</span></span>|<span data-ttu-id="9b904-123">String</span><span class="sxs-lookup"><span data-stu-id="9b904-123">String</span></span>|<span data-ttu-id="9b904-124">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="9b904-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="9b904-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b904-125">enrolledDeviceCount</span></span>|<span data-ttu-id="9b904-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9b904-126">Int32</span></span>|<span data-ttu-id="9b904-127">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="9b904-127">Total enrolled device count.</span></span> <span data-ttu-id="9b904-128">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="9b904-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="9b904-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="9b904-129">mdmEnrolledCount</span></span>|<span data-ttu-id="9b904-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9b904-130">Int32</span></span>|<span data-ttu-id="9b904-131">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="9b904-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="9b904-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b904-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="9b904-133">Int32</span><span class="sxs-lookup"><span data-stu-id="9b904-133">Int32</span></span>|<span data-ttu-id="9b904-134">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="9b904-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="9b904-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9b904-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="9b904-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9b904-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="9b904-137">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="9b904-137">Device operating system summary.</span></span>|
|<span data-ttu-id="9b904-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b904-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="9b904-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b904-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="9b904-140">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="9b904-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="9b904-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="9b904-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="9b904-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="9b904-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="9b904-143">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="9b904-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="9b904-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b904-144">lastModifiedDateTime</span></span>|<span data-ttu-id="9b904-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b904-145">DateTimeOffset</span></span>|<span data-ttu-id="9b904-146">Zeitpunkt der letzten Änderungsdatum des Geräts (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="9b904-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b904-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9b904-147">Relationships</span></span>
<span data-ttu-id="9b904-148">Keine</span><span class="sxs-lookup"><span data-stu-id="9b904-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b904-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9b904-149">JSON Representation</span></span>
<span data-ttu-id="9b904-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9b904-150">Here is a JSON representation of the resource.</span></span>
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```





