---
title: Aktualisieren von „settingStateDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fa47448fffacf3e48e7b9f63a34cf93b4392044
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986859"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="3b088-103">Aktualisieren von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="3b088-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="3b088-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b088-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b088-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3b088-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b088-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3b088-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b088-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b088-107">Prerequisites</span></span>
<span data-ttu-id="3b088-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b088-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b088-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b088-110">Permission type</span></span>|<span data-ttu-id="3b088-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b088-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b088-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b088-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b088-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b088-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b088-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b088-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b088-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b088-115">Not supported.</span></span>|
|<span data-ttu-id="3b088-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b088-116">Application</span></span>|<span data-ttu-id="3b088-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b088-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b088-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b088-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3b088-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b088-119">Request headers</span></span>
|<span data-ttu-id="3b088-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3b088-120">Header</span></span>|<span data-ttu-id="3b088-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3b088-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b088-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b088-122">Authorization</span></span>|<span data-ttu-id="3b088-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b088-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b088-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3b088-124">Accept</span></span>|<span data-ttu-id="3b088-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b088-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b088-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b088-126">Request body</span></span>
<span data-ttu-id="3b088-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="3b088-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="3b088-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3b088-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="3b088-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b088-129">Property</span></span>|<span data-ttu-id="3b088-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3b088-130">Type</span></span>|<span data-ttu-id="3b088-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b088-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b088-132">id</span><span class="sxs-lookup"><span data-stu-id="3b088-132">id</span></span>|<span data-ttu-id="3b088-133">String</span><span class="sxs-lookup"><span data-stu-id="3b088-133">String</span></span>|<span data-ttu-id="3b088-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3b088-134">Key of the entity.</span></span>|
|<span data-ttu-id="3b088-135">settingName</span><span class="sxs-lookup"><span data-stu-id="3b088-135">settingName</span></span>|<span data-ttu-id="3b088-136">String</span><span class="sxs-lookup"><span data-stu-id="3b088-136">String</span></span>|<span data-ttu-id="3b088-137">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-137">Name of the setting</span></span>|
|<span data-ttu-id="3b088-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="3b088-138">instancePath</span></span>|<span data-ttu-id="3b088-139">String</span><span class="sxs-lookup"><span data-stu-id="3b088-139">String</span></span>|<span data-ttu-id="3b088-140">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="3b088-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="3b088-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-141">unknownDeviceCount</span></span>|<span data-ttu-id="3b088-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-142">Int32</span></span>|<span data-ttu-id="3b088-143">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="3b088-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="3b088-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-145">Int32</span></span>|<span data-ttu-id="3b088-146">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="3b088-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-147">compliantDeviceCount</span></span>|<span data-ttu-id="3b088-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-148">Int32</span></span>|<span data-ttu-id="3b088-149">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="3b088-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-150">remediatedDeviceCount</span></span>|<span data-ttu-id="3b088-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-151">Int32</span></span>|<span data-ttu-id="3b088-152">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="3b088-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3b088-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-154">Int32</span></span>|<span data-ttu-id="3b088-155">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="3b088-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-156">errorDeviceCount</span></span>|<span data-ttu-id="3b088-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-157">Int32</span></span>|<span data-ttu-id="3b088-158">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-158">Device error count for the setting</span></span>|
|<span data-ttu-id="3b088-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b088-159">conflictDeviceCount</span></span>|<span data-ttu-id="3b088-160">Int32</span><span class="sxs-lookup"><span data-stu-id="3b088-160">Int32</span></span>|<span data-ttu-id="3b088-161">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="3b088-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="3b088-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b088-162">Response</span></span>
<span data-ttu-id="3b088-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3b088-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b088-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b088-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b088-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b088-165">Request</span></span>
<span data-ttu-id="3b088-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b088-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="3b088-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b088-167">Response</span></span>
<span data-ttu-id="3b088-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b088-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




