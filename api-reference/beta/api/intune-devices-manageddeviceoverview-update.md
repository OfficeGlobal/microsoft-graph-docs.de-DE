---
title: Aktualisieren von „managedDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 642d565a7555446da1728c0a697598de4d5459cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147845"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="24d36-103">Aktualisieren von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="24d36-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="24d36-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24d36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24d36-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="24d36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24d36-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="24d36-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24d36-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24d36-107">Prerequisites</span></span>
<span data-ttu-id="24d36-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="24d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="24d36-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24d36-110">Permission type</span></span>|<span data-ttu-id="24d36-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24d36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24d36-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24d36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24d36-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24d36-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24d36-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24d36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24d36-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24d36-115">Not supported.</span></span>|
|<span data-ttu-id="24d36-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24d36-116">Application</span></span>|<span data-ttu-id="24d36-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24d36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24d36-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24d36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="24d36-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24d36-119">Request headers</span></span>
|<span data-ttu-id="24d36-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="24d36-120">Header</span></span>|<span data-ttu-id="24d36-121">Wert</span><span class="sxs-lookup"><span data-stu-id="24d36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24d36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d36-122">Authorization</span></span>|<span data-ttu-id="24d36-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="24d36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24d36-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="24d36-124">Accept</span></span>|<span data-ttu-id="24d36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24d36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d36-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24d36-126">Request body</span></span>
<span data-ttu-id="24d36-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="24d36-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="24d36-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="24d36-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="24d36-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24d36-129">Property</span></span>|<span data-ttu-id="24d36-130">Typ</span><span class="sxs-lookup"><span data-stu-id="24d36-130">Type</span></span>|<span data-ttu-id="24d36-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24d36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24d36-132">id</span><span class="sxs-lookup"><span data-stu-id="24d36-132">id</span></span>|<span data-ttu-id="24d36-133">String</span><span class="sxs-lookup"><span data-stu-id="24d36-133">String</span></span>|<span data-ttu-id="24d36-134">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="24d36-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="24d36-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24d36-135">enrolledDeviceCount</span></span>|<span data-ttu-id="24d36-136">Int32</span><span class="sxs-lookup"><span data-stu-id="24d36-136">Int32</span></span>|<span data-ttu-id="24d36-137">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="24d36-137">Total enrolled device count.</span></span> <span data-ttu-id="24d36-138">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="24d36-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="24d36-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="24d36-139">mdmEnrolledCount</span></span>|<span data-ttu-id="24d36-140">Int32</span><span class="sxs-lookup"><span data-stu-id="24d36-140">Int32</span></span>|<span data-ttu-id="24d36-141">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="24d36-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="24d36-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24d36-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="24d36-143">Int32</span><span class="sxs-lookup"><span data-stu-id="24d36-143">Int32</span></span>|<span data-ttu-id="24d36-144">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="24d36-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="24d36-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="24d36-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="24d36-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="24d36-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="24d36-147">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="24d36-147">Device operating system summary.</span></span>|
|<span data-ttu-id="24d36-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="24d36-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="24d36-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="24d36-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="24d36-150">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="24d36-150">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="24d36-151">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="24d36-151">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="24d36-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="24d36-152">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="24d36-153">Modelliert und fertigt meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="24d36-153">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="24d36-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24d36-154">lastModifiedDateTime</span></span>|<span data-ttu-id="24d36-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24d36-155">DateTimeOffset</span></span>|<span data-ttu-id="24d36-156">Datum der letzten Änderung der Geräteübersicht</span><span class="sxs-lookup"><span data-stu-id="24d36-156">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="24d36-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="24d36-157">Response</span></span>
<span data-ttu-id="24d36-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="24d36-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24d36-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24d36-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="24d36-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24d36-160">Request</span></span>
<span data-ttu-id="24d36-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24d36-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 943

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="24d36-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="24d36-162">Response</span></span>
<span data-ttu-id="24d36-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24d36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1056

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




