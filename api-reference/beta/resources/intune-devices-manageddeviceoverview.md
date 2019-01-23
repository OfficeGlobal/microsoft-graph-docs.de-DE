---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db5cebe36850971c871f673d07f18b8d5121cb1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422236"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="1a18a-103">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1a18a-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="1a18a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1a18a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a18a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a18a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a18a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a18a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a18a-107">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="1a18a-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="1a18a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="1a18a-108">Methods</span></span>
|<span data-ttu-id="1a18a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="1a18a-109">Method</span></span>|<span data-ttu-id="1a18a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1a18a-110">Return Type</span></span>|<span data-ttu-id="1a18a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a18a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a18a-112">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="1a18a-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="1a18a-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a18a-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="1a18a-114">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a18a-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="1a18a-115">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1a18a-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="1a18a-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a18a-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="1a18a-117">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a18a-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a18a-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1a18a-118">Properties</span></span>
|<span data-ttu-id="1a18a-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a18a-119">Property</span></span>|<span data-ttu-id="1a18a-120">Typ</span><span class="sxs-lookup"><span data-stu-id="1a18a-120">Type</span></span>|<span data-ttu-id="1a18a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a18a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a18a-122">id</span><span class="sxs-lookup"><span data-stu-id="1a18a-122">id</span></span>|<span data-ttu-id="1a18a-123">String</span><span class="sxs-lookup"><span data-stu-id="1a18a-123">String</span></span>|<span data-ttu-id="1a18a-124">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="1a18a-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="1a18a-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1a18a-125">enrolledDeviceCount</span></span>|<span data-ttu-id="1a18a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="1a18a-126">Int32</span></span>|<span data-ttu-id="1a18a-127">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="1a18a-127">Total enrolled device count.</span></span> <span data-ttu-id="1a18a-128">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="1a18a-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="1a18a-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="1a18a-129">mdmEnrolledCount</span></span>|<span data-ttu-id="1a18a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1a18a-130">Int32</span></span>|<span data-ttu-id="1a18a-131">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="1a18a-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="1a18a-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1a18a-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="1a18a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1a18a-133">Int32</span></span>|<span data-ttu-id="1a18a-134">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="1a18a-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="1a18a-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="1a18a-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="1a18a-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="1a18a-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="1a18a-137">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="1a18a-137">Device operating system summary.</span></span>|
|<span data-ttu-id="1a18a-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="1a18a-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="1a18a-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="1a18a-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="1a18a-140">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="1a18a-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="1a18a-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="1a18a-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="1a18a-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="1a18a-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="1a18a-143">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="1a18a-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="1a18a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a18a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="1a18a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a18a-145">DateTimeOffset</span></span>|<span data-ttu-id="1a18a-146">Zeitpunkt der letzten Änderungsdatum des Geräts (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="1a18a-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a18a-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1a18a-147">Relationships</span></span>
<span data-ttu-id="1a18a-148">Keine</span><span class="sxs-lookup"><span data-stu-id="1a18a-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a18a-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1a18a-149">JSON Representation</span></span>
<span data-ttu-id="1a18a-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1a18a-150">Here is a JSON representation of the resource.</span></span>
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




