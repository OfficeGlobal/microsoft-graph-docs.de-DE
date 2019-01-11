---
title: Aktualisieren von „managedDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5116d2d1bdd3b1b71252db528e9d0f476a219d42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822526"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="f33da-103">Aktualisieren von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="f33da-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="f33da-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f33da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f33da-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f33da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f33da-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f33da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f33da-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f33da-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f33da-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f33da-108">Prerequisites</span></span>
<span data-ttu-id="f33da-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f33da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f33da-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f33da-111">Permission type</span></span>|<span data-ttu-id="f33da-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f33da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f33da-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f33da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f33da-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f33da-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f33da-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f33da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f33da-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f33da-116">Not supported.</span></span>|
|<span data-ttu-id="f33da-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f33da-117">Application</span></span>|<span data-ttu-id="f33da-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f33da-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f33da-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f33da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="f33da-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f33da-120">Request headers</span></span>
|<span data-ttu-id="f33da-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f33da-121">Header</span></span>|<span data-ttu-id="f33da-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f33da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f33da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f33da-123">Authorization</span></span>|<span data-ttu-id="f33da-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f33da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f33da-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f33da-125">Accept</span></span>|<span data-ttu-id="f33da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f33da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f33da-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f33da-127">Request body</span></span>
<span data-ttu-id="f33da-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="f33da-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="f33da-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f33da-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="f33da-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f33da-130">Property</span></span>|<span data-ttu-id="f33da-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f33da-131">Type</span></span>|<span data-ttu-id="f33da-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f33da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f33da-133">id</span><span class="sxs-lookup"><span data-stu-id="f33da-133">id</span></span>|<span data-ttu-id="f33da-134">String</span><span class="sxs-lookup"><span data-stu-id="f33da-134">String</span></span>|<span data-ttu-id="f33da-135">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="f33da-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f33da-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f33da-136">enrolledDeviceCount</span></span>|<span data-ttu-id="f33da-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f33da-137">Int32</span></span>|<span data-ttu-id="f33da-138">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="f33da-138">Total enrolled device count.</span></span> <span data-ttu-id="f33da-139">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="f33da-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f33da-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f33da-140">mdmEnrolledCount</span></span>|<span data-ttu-id="f33da-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f33da-141">Int32</span></span>|<span data-ttu-id="f33da-142">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="f33da-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f33da-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f33da-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f33da-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f33da-144">Int32</span></span>|<span data-ttu-id="f33da-145">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="f33da-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f33da-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f33da-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f33da-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f33da-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f33da-148">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="f33da-148">Device operating system summary.</span></span>|
|<span data-ttu-id="f33da-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f33da-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f33da-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f33da-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f33da-151">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="f33da-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="f33da-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f33da-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="f33da-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f33da-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="f33da-154">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="f33da-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="f33da-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f33da-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f33da-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f33da-156">DateTimeOffset</span></span>|<span data-ttu-id="f33da-157">Zeitpunkt der letzten Änderungsdatum des Geräts (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="f33da-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="f33da-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="f33da-158">Response</span></span>
<span data-ttu-id="f33da-159">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f33da-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f33da-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f33da-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="f33da-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f33da-161">Request</span></span>
<span data-ttu-id="f33da-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f33da-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 947

{
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

### <a name="response"></a><span data-ttu-id="f33da-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="f33da-163">Response</span></span>
<span data-ttu-id="f33da-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f33da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





