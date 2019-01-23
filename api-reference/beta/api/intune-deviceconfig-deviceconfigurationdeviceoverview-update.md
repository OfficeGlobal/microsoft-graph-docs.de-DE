---
title: Aktualisieren von „deviceConfigurationDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 180778580f7737141efa935a2dfe87b412b677e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423377"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="55cd7-103">Aktualisieren von „deviceConfigurationDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="55cd7-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="55cd7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="55cd7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="55cd7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55cd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55cd7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55cd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55cd7-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="55cd7-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55cd7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="55cd7-108">Prerequisites</span></span>
<span data-ttu-id="55cd7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="55cd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="55cd7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55cd7-111">Permission type</span></span>|<span data-ttu-id="55cd7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55cd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55cd7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55cd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55cd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55cd7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55cd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55cd7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55cd7-116">Not supported.</span></span>|
|<span data-ttu-id="55cd7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55cd7-117">Application</span></span>|<span data-ttu-id="55cd7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55cd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55cd7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55cd7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="55cd7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55cd7-120">Request headers</span></span>
|<span data-ttu-id="55cd7-121">Header</span><span class="sxs-lookup"><span data-stu-id="55cd7-121">Header</span></span>|<span data-ttu-id="55cd7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="55cd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55cd7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="55cd7-123">Authorization</span></span>|<span data-ttu-id="55cd7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="55cd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55cd7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="55cd7-125">Accept</span></span>|<span data-ttu-id="55cd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55cd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55cd7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55cd7-127">Request body</span></span>
<span data-ttu-id="55cd7-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="55cd7-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="55cd7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="55cd7-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="55cd7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="55cd7-130">Property</span></span>|<span data-ttu-id="55cd7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="55cd7-131">Type</span></span>|<span data-ttu-id="55cd7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55cd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55cd7-133">id</span><span class="sxs-lookup"><span data-stu-id="55cd7-133">id</span></span>|<span data-ttu-id="55cd7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55cd7-134">String</span></span>|<span data-ttu-id="55cd7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="55cd7-135">Key of the entity.</span></span>|
|<span data-ttu-id="55cd7-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-136">pendingCount</span></span>|<span data-ttu-id="55cd7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-137">Int32</span></span>|<span data-ttu-id="55cd7-138">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="55cd7-138">Number of pending devices</span></span>|
|<span data-ttu-id="55cd7-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-139">notApplicableCount</span></span>|<span data-ttu-id="55cd7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-140">Int32</span></span>|<span data-ttu-id="55cd7-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="55cd7-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="55cd7-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="55cd7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-143">Int32</span></span>|<span data-ttu-id="55cd7-144">Anzahl der Geräte, die aufgrund von Konflikt Plattform und Richtlinie nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="55cd7-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="55cd7-145">successCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-145">successCount</span></span>|<span data-ttu-id="55cd7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-146">Int32</span></span>|<span data-ttu-id="55cd7-147">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="55cd7-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="55cd7-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-148">errorCount</span></span>|<span data-ttu-id="55cd7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-149">Int32</span></span>|<span data-ttu-id="55cd7-150">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="55cd7-150">Number of error devices</span></span>|
|<span data-ttu-id="55cd7-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-151">failedCount</span></span>|<span data-ttu-id="55cd7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-152">Int32</span></span>|<span data-ttu-id="55cd7-153">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="55cd7-153">Number of failed devices</span></span>|
|<span data-ttu-id="55cd7-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="55cd7-154">conflictCount</span></span>|<span data-ttu-id="55cd7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-155">Int32</span></span>|<span data-ttu-id="55cd7-156">Anzahl der Geräte in Konflikt</span><span class="sxs-lookup"><span data-stu-id="55cd7-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="55cd7-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="55cd7-157">lastUpdateDateTime</span></span>|<span data-ttu-id="55cd7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55cd7-158">DateTimeOffset</span></span>|<span data-ttu-id="55cd7-159">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="55cd7-159">Last update time</span></span>|
|<span data-ttu-id="55cd7-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="55cd7-160">configurationVersion</span></span>|<span data-ttu-id="55cd7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="55cd7-161">Int32</span></span>|<span data-ttu-id="55cd7-162">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="55cd7-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="55cd7-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="55cd7-163">Response</span></span>
<span data-ttu-id="55cd7-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="55cd7-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55cd7-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55cd7-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="55cd7-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55cd7-166">Request</span></span>
<span data-ttu-id="55cd7-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55cd7-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
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

### <a name="response"></a><span data-ttu-id="55cd7-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="55cd7-168">Response</span></span>
<span data-ttu-id="55cd7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55cd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




