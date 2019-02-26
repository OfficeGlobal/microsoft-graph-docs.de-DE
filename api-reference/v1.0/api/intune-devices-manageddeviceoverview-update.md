---
title: Aktualisieren von „managedDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e4b7acf2b03ee37bf9171bfe83164c25e993f5f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260578"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="4f499-103">Aktualisieren von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="4f499-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="4f499-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4f499-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f499-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="4f499-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f499-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4f499-106">Prerequisites</span></span>
<span data-ttu-id="4f499-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4f499-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f499-109">Permission type</span></span>|<span data-ttu-id="4f499-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f499-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f499-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f499-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f499-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f499-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4f499-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f499-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f499-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f499-114">Not supported.</span></span>|
|<span data-ttu-id="4f499-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f499-115">Application</span></span>|<span data-ttu-id="4f499-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f499-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f499-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f499-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="4f499-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f499-118">Request headers</span></span>
|<span data-ttu-id="4f499-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4f499-119">Header</span></span>|<span data-ttu-id="4f499-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4f499-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f499-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f499-121">Authorization</span></span>|<span data-ttu-id="4f499-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f499-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f499-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4f499-123">Accept</span></span>|<span data-ttu-id="4f499-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f499-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f499-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f499-125">Request body</span></span>
<span data-ttu-id="4f499-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="4f499-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="4f499-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4f499-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="4f499-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f499-128">Property</span></span>|<span data-ttu-id="4f499-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4f499-129">Type</span></span>|<span data-ttu-id="4f499-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f499-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f499-131">id</span><span class="sxs-lookup"><span data-stu-id="4f499-131">id</span></span>|<span data-ttu-id="4f499-132">String</span><span class="sxs-lookup"><span data-stu-id="4f499-132">String</span></span>|<span data-ttu-id="4f499-133">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="4f499-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="4f499-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4f499-134">enrolledDeviceCount</span></span>|<span data-ttu-id="4f499-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4f499-135">Int32</span></span>|<span data-ttu-id="4f499-136">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="4f499-136">Total enrolled device count.</span></span> <span data-ttu-id="4f499-137">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="4f499-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="4f499-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="4f499-138">mdmEnrolledCount</span></span>|<span data-ttu-id="4f499-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4f499-139">Int32</span></span>|<span data-ttu-id="4f499-140">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="4f499-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="4f499-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4f499-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="4f499-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4f499-142">Int32</span></span>|<span data-ttu-id="4f499-143">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="4f499-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="4f499-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="4f499-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="4f499-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="4f499-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="4f499-146">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="4f499-146">Device operating system summary.</span></span>|
|<span data-ttu-id="4f499-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="4f499-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="4f499-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="4f499-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="4f499-149">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="4f499-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="4f499-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f499-150">Response</span></span>
<span data-ttu-id="4f499-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4f499-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f499-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f499-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f499-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f499-153">Request</span></span>
<span data-ttu-id="4f499-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f499-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 685

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
  }
}
```

### <a name="response"></a><span data-ttu-id="4f499-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f499-155">Response</span></span>
<span data-ttu-id="4f499-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f499-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

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
  }
}
```



