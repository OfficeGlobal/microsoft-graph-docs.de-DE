---
title: Aktualisieren von „managedDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: be6b7260b6613ef4396e84670b0c83869804b43c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824934"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="6bf02-103">Aktualisieren von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="6bf02-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="6bf02-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6bf02-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf02-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="6bf02-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bf02-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6bf02-106">Prerequisites</span></span>
<span data-ttu-id="6bf02-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bf02-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6bf02-109">Permission type</span></span>|<span data-ttu-id="6bf02-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6bf02-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bf02-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6bf02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bf02-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf02-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6bf02-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6bf02-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bf02-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bf02-114">Not supported.</span></span>|
|<span data-ttu-id="6bf02-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6bf02-115">Application</span></span>|<span data-ttu-id="6bf02-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bf02-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bf02-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bf02-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="6bf02-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6bf02-118">Request headers</span></span>
|<span data-ttu-id="6bf02-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6bf02-119">Header</span></span>|<span data-ttu-id="6bf02-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6bf02-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bf02-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bf02-121">Authorization</span></span>|<span data-ttu-id="6bf02-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6bf02-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bf02-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6bf02-123">Accept</span></span>|<span data-ttu-id="6bf02-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6bf02-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bf02-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6bf02-125">Request body</span></span>
<span data-ttu-id="6bf02-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="6bf02-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="6bf02-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="6bf02-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="6bf02-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6bf02-128">Property</span></span>|<span data-ttu-id="6bf02-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6bf02-129">Type</span></span>|<span data-ttu-id="6bf02-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bf02-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf02-131">id</span><span class="sxs-lookup"><span data-stu-id="6bf02-131">id</span></span>|<span data-ttu-id="6bf02-132">String</span><span class="sxs-lookup"><span data-stu-id="6bf02-132">String</span></span>|<span data-ttu-id="6bf02-133">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="6bf02-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="6bf02-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6bf02-134">enrolledDeviceCount</span></span>|<span data-ttu-id="6bf02-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6bf02-135">Int32</span></span>|<span data-ttu-id="6bf02-136">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="6bf02-136">Total enrolled device count.</span></span> <span data-ttu-id="6bf02-137">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="6bf02-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="6bf02-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="6bf02-138">mdmEnrolledCount</span></span>|<span data-ttu-id="6bf02-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6bf02-139">Int32</span></span>|<span data-ttu-id="6bf02-140">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="6bf02-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="6bf02-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6bf02-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="6bf02-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6bf02-142">Int32</span></span>|<span data-ttu-id="6bf02-143">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="6bf02-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="6bf02-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6bf02-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="6bf02-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6bf02-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="6bf02-146">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="6bf02-146">Device operating system summary.</span></span>|
|<span data-ttu-id="6bf02-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6bf02-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="6bf02-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6bf02-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="6bf02-149">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="6bf02-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="6bf02-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bf02-150">Response</span></span>
<span data-ttu-id="6bf02-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6bf02-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bf02-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6bf02-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bf02-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bf02-153">Request</span></span>
<span data-ttu-id="6bf02-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6bf02-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6bf02-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bf02-155">Response</span></span>
<span data-ttu-id="6bf02-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6bf02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



