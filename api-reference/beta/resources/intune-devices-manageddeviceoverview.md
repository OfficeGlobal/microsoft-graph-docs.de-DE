---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6c7187bc5cb984e4ca7e607068e6010f747f868
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175003"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="17447-103">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="17447-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="17447-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17447-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17447-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="17447-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17447-106">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="17447-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="17447-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="17447-107">Methods</span></span>
|<span data-ttu-id="17447-108">Methode</span><span class="sxs-lookup"><span data-stu-id="17447-108">Method</span></span>|<span data-ttu-id="17447-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="17447-109">Return Type</span></span>|<span data-ttu-id="17447-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17447-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17447-111">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="17447-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="17447-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17447-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="17447-113">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="17447-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="17447-114">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="17447-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="17447-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17447-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="17447-116">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="17447-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17447-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17447-117">Properties</span></span>
|<span data-ttu-id="17447-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17447-118">Property</span></span>|<span data-ttu-id="17447-119">Typ</span><span class="sxs-lookup"><span data-stu-id="17447-119">Type</span></span>|<span data-ttu-id="17447-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17447-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17447-121">id</span><span class="sxs-lookup"><span data-stu-id="17447-121">id</span></span>|<span data-ttu-id="17447-122">String</span><span class="sxs-lookup"><span data-stu-id="17447-122">String</span></span>|<span data-ttu-id="17447-123">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="17447-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="17447-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17447-124">enrolledDeviceCount</span></span>|<span data-ttu-id="17447-125">Int32</span><span class="sxs-lookup"><span data-stu-id="17447-125">Int32</span></span>|<span data-ttu-id="17447-126">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="17447-126">Total enrolled device count.</span></span> <span data-ttu-id="17447-127">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="17447-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="17447-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="17447-128">mdmEnrolledCount</span></span>|<span data-ttu-id="17447-129">Int32</span><span class="sxs-lookup"><span data-stu-id="17447-129">Int32</span></span>|<span data-ttu-id="17447-130">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="17447-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="17447-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17447-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="17447-132">Int32</span><span class="sxs-lookup"><span data-stu-id="17447-132">Int32</span></span>|<span data-ttu-id="17447-133">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="17447-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="17447-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="17447-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="17447-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="17447-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="17447-136">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="17447-136">Device operating system summary.</span></span>|
|<span data-ttu-id="17447-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="17447-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="17447-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="17447-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="17447-139">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="17447-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="17447-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="17447-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="17447-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="17447-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="17447-142">Modelliert und fertigt meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="17447-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="17447-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17447-143">lastModifiedDateTime</span></span>|<span data-ttu-id="17447-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17447-144">DateTimeOffset</span></span>|<span data-ttu-id="17447-145">Datum der letzten Änderung der Geräteübersicht</span><span class="sxs-lookup"><span data-stu-id="17447-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="17447-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="17447-146">Relationships</span></span>
<span data-ttu-id="17447-147">Keine</span><span class="sxs-lookup"><span data-stu-id="17447-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17447-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17447-148">JSON Representation</span></span>
<span data-ttu-id="17447-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="17447-149">Here is a JSON representation of the resource.</span></span>
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




