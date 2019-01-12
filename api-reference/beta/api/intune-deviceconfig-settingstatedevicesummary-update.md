---
title: Aktualisieren von „settingStateDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ab0a3ec4609ce3f5015d9bb1ae6f1b815f5d6b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920597"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="26cdd-103">Aktualisieren von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="26cdd-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="26cdd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="26cdd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26cdd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26cdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26cdd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="26cdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26cdd-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="26cdd-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26cdd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="26cdd-108">Prerequisites</span></span>
<span data-ttu-id="26cdd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26cdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26cdd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26cdd-111">Permission type</span></span>|<span data-ttu-id="26cdd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26cdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26cdd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26cdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26cdd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26cdd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26cdd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26cdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26cdd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26cdd-116">Not supported.</span></span>|
|<span data-ttu-id="26cdd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26cdd-117">Application</span></span>|<span data-ttu-id="26cdd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26cdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26cdd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26cdd-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="26cdd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26cdd-120">Request headers</span></span>
|<span data-ttu-id="26cdd-121">Header</span><span class="sxs-lookup"><span data-stu-id="26cdd-121">Header</span></span>|<span data-ttu-id="26cdd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="26cdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26cdd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26cdd-123">Authorization</span></span>|<span data-ttu-id="26cdd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="26cdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26cdd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="26cdd-125">Accept</span></span>|<span data-ttu-id="26cdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26cdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26cdd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26cdd-127">Request body</span></span>
<span data-ttu-id="26cdd-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="26cdd-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="26cdd-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="26cdd-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="26cdd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26cdd-130">Property</span></span>|<span data-ttu-id="26cdd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="26cdd-131">Type</span></span>|<span data-ttu-id="26cdd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26cdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26cdd-133">id</span><span class="sxs-lookup"><span data-stu-id="26cdd-133">id</span></span>|<span data-ttu-id="26cdd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26cdd-134">String</span></span>|<span data-ttu-id="26cdd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="26cdd-135">Key of the entity.</span></span>|
|<span data-ttu-id="26cdd-136">settingName</span><span class="sxs-lookup"><span data-stu-id="26cdd-136">settingName</span></span>|<span data-ttu-id="26cdd-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26cdd-137">String</span></span>|<span data-ttu-id="26cdd-138">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-138">Name of the setting</span></span>|
|<span data-ttu-id="26cdd-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="26cdd-139">instancePath</span></span>|<span data-ttu-id="26cdd-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26cdd-140">String</span></span>|<span data-ttu-id="26cdd-141">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="26cdd-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="26cdd-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-142">unknownDeviceCount</span></span>|<span data-ttu-id="26cdd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-143">Int32</span></span>|<span data-ttu-id="26cdd-144">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="26cdd-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="26cdd-146">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-146">Int32</span></span>|<span data-ttu-id="26cdd-147">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="26cdd-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-148">compliantDeviceCount</span></span>|<span data-ttu-id="26cdd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-149">Int32</span></span>|<span data-ttu-id="26cdd-150">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="26cdd-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-151">remediatedDeviceCount</span></span>|<span data-ttu-id="26cdd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-152">Int32</span></span>|<span data-ttu-id="26cdd-153">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="26cdd-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="26cdd-155">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-155">Int32</span></span>|<span data-ttu-id="26cdd-156">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="26cdd-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-157">errorDeviceCount</span></span>|<span data-ttu-id="26cdd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-158">Int32</span></span>|<span data-ttu-id="26cdd-159">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-159">Device error count for the setting</span></span>|
|<span data-ttu-id="26cdd-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26cdd-160">conflictDeviceCount</span></span>|<span data-ttu-id="26cdd-161">Int32</span><span class="sxs-lookup"><span data-stu-id="26cdd-161">Int32</span></span>|<span data-ttu-id="26cdd-162">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="26cdd-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="26cdd-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="26cdd-163">Response</span></span>
<span data-ttu-id="26cdd-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="26cdd-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26cdd-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26cdd-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="26cdd-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26cdd-166">Request</span></span>
<span data-ttu-id="26cdd-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26cdd-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 296

{
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

### <a name="response"></a><span data-ttu-id="26cdd-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="26cdd-168">Response</span></span>
<span data-ttu-id="26cdd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26cdd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





