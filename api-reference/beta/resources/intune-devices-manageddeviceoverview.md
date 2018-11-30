---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
ms.openlocfilehash: 11f1012329d0217499d813b94f72474da8c683a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062185"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="f3efc-103">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f3efc-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="f3efc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3efc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3efc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3efc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3efc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3efc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3efc-107">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="f3efc-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="f3efc-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="f3efc-108">Methods</span></span>
|<span data-ttu-id="f3efc-109">Methode</span><span class="sxs-lookup"><span data-stu-id="f3efc-109">Method</span></span>|<span data-ttu-id="f3efc-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f3efc-110">Return Type</span></span>|<span data-ttu-id="f3efc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3efc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3efc-112">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="f3efc-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="f3efc-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f3efc-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="f3efc-114">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3efc-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="f3efc-115">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f3efc-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="f3efc-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f3efc-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="f3efc-117">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3efc-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3efc-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f3efc-118">Properties</span></span>
|<span data-ttu-id="f3efc-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3efc-119">Property</span></span>|<span data-ttu-id="f3efc-120">Typ</span><span class="sxs-lookup"><span data-stu-id="f3efc-120">Type</span></span>|<span data-ttu-id="f3efc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3efc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3efc-122">id</span><span class="sxs-lookup"><span data-stu-id="f3efc-122">id</span></span>|<span data-ttu-id="f3efc-123">String</span><span class="sxs-lookup"><span data-stu-id="f3efc-123">String</span></span>|<span data-ttu-id="f3efc-124">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="f3efc-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f3efc-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3efc-125">enrolledDeviceCount</span></span>|<span data-ttu-id="f3efc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f3efc-126">Int32</span></span>|<span data-ttu-id="f3efc-127">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="f3efc-127">Total enrolled device count.</span></span> <span data-ttu-id="f3efc-128">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="f3efc-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f3efc-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f3efc-129">mdmEnrolledCount</span></span>|<span data-ttu-id="f3efc-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f3efc-130">Int32</span></span>|<span data-ttu-id="f3efc-131">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="f3efc-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f3efc-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3efc-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f3efc-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f3efc-133">Int32</span></span>|<span data-ttu-id="f3efc-134">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="f3efc-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f3efc-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f3efc-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f3efc-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f3efc-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f3efc-137">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="f3efc-137">Device operating system summary.</span></span>|
|<span data-ttu-id="f3efc-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f3efc-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f3efc-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f3efc-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f3efc-140">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="f3efc-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="f3efc-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f3efc-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="f3efc-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f3efc-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="f3efc-143">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="f3efc-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="f3efc-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3efc-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f3efc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3efc-145">DateTimeOffset</span></span>|<span data-ttu-id="f3efc-146">Zeitpunkt der letzten Änderungsdatum des Geräts (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="f3efc-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3efc-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f3efc-147">Relationships</span></span>
<span data-ttu-id="f3efc-148">Keine</span><span class="sxs-lookup"><span data-stu-id="f3efc-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3efc-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f3efc-149">JSON Representation</span></span>
<span data-ttu-id="f3efc-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f3efc-150">Here is a JSON representation of the resource.</span></span>
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





