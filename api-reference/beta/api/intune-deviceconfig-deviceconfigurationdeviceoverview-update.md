---
title: Aktualisieren von „deviceConfigurationDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 79ff57c147a165f1670be733b7d14113ee7de382
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939392"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="83901-103">Aktualisieren von „deviceConfigurationDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="83901-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="83901-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83901-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83901-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83901-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83901-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83901-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83901-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="83901-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83901-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83901-108">Prerequisites</span></span>
<span data-ttu-id="83901-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83901-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83901-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83901-111">Permission type</span></span>|<span data-ttu-id="83901-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83901-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83901-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83901-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83901-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83901-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83901-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83901-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83901-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83901-116">Not supported.</span></span>|
|<span data-ttu-id="83901-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83901-117">Application</span></span>|<span data-ttu-id="83901-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83901-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83901-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83901-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="83901-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83901-120">Request headers</span></span>
|<span data-ttu-id="83901-121">Header</span><span class="sxs-lookup"><span data-stu-id="83901-121">Header</span></span>|<span data-ttu-id="83901-122">Wert</span><span class="sxs-lookup"><span data-stu-id="83901-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83901-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83901-123">Authorization</span></span>|<span data-ttu-id="83901-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83901-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83901-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="83901-125">Accept</span></span>|<span data-ttu-id="83901-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83901-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83901-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83901-127">Request body</span></span>
<span data-ttu-id="83901-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="83901-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="83901-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="83901-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="83901-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83901-130">Property</span></span>|<span data-ttu-id="83901-131">Typ</span><span class="sxs-lookup"><span data-stu-id="83901-131">Type</span></span>|<span data-ttu-id="83901-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83901-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83901-133">id</span><span class="sxs-lookup"><span data-stu-id="83901-133">id</span></span>|<span data-ttu-id="83901-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83901-134">String</span></span>|<span data-ttu-id="83901-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="83901-135">Key of the entity.</span></span>|
|<span data-ttu-id="83901-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="83901-136">pendingCount</span></span>|<span data-ttu-id="83901-137">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-137">Int32</span></span>|<span data-ttu-id="83901-138">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="83901-138">Number of pending devices</span></span>|
|<span data-ttu-id="83901-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="83901-139">notApplicableCount</span></span>|<span data-ttu-id="83901-140">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-140">Int32</span></span>|<span data-ttu-id="83901-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="83901-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="83901-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="83901-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="83901-143">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-143">Int32</span></span>|<span data-ttu-id="83901-144">Anzahl der Geräte, die aufgrund von Konflikt Plattform und Richtlinie nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="83901-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="83901-145">successCount</span><span class="sxs-lookup"><span data-stu-id="83901-145">successCount</span></span>|<span data-ttu-id="83901-146">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-146">Int32</span></span>|<span data-ttu-id="83901-147">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="83901-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="83901-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="83901-148">errorCount</span></span>|<span data-ttu-id="83901-149">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-149">Int32</span></span>|<span data-ttu-id="83901-150">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="83901-150">Number of error devices</span></span>|
|<span data-ttu-id="83901-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="83901-151">failedCount</span></span>|<span data-ttu-id="83901-152">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-152">Int32</span></span>|<span data-ttu-id="83901-153">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="83901-153">Number of failed devices</span></span>|
|<span data-ttu-id="83901-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="83901-154">conflictCount</span></span>|<span data-ttu-id="83901-155">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-155">Int32</span></span>|<span data-ttu-id="83901-156">Anzahl der Geräte in Konflikt</span><span class="sxs-lookup"><span data-stu-id="83901-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="83901-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="83901-157">lastUpdateDateTime</span></span>|<span data-ttu-id="83901-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83901-158">DateTimeOffset</span></span>|<span data-ttu-id="83901-159">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="83901-159">Last update time</span></span>|
|<span data-ttu-id="83901-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="83901-160">configurationVersion</span></span>|<span data-ttu-id="83901-161">Int32</span><span class="sxs-lookup"><span data-stu-id="83901-161">Int32</span></span>|<span data-ttu-id="83901-162">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="83901-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="83901-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="83901-163">Response</span></span>
<span data-ttu-id="83901-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83901-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83901-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83901-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="83901-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83901-166">Request</span></span>
<span data-ttu-id="83901-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83901-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 273

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="83901-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="83901-168">Response</span></span>
<span data-ttu-id="83901-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83901-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





