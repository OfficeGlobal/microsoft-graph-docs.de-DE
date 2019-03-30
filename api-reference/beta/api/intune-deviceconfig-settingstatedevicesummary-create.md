---
title: settingStateDeviceSummary erstellen
description: Erstellen eines neuen SettingStateDeviceSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d77324ee3d1e13d51cc196d90015ee09e5760c1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986775"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="4b006-103">settingStateDeviceSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="4b006-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="4b006-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b006-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b006-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4b006-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b006-106">Erstellen eines neuen [SettingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b006-106">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b006-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b006-107">Prerequisites</span></span>
<span data-ttu-id="4b006-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b006-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b006-110">Permission type</span></span>|<span data-ttu-id="4b006-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b006-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b006-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b006-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b006-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b006-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b006-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b006-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b006-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b006-115">Not supported.</span></span>|
|<span data-ttu-id="4b006-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b006-116">Application</span></span>|<span data-ttu-id="4b006-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b006-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b006-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b006-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4b006-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b006-119">Request headers</span></span>
|<span data-ttu-id="4b006-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4b006-120">Header</span></span>|<span data-ttu-id="4b006-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4b006-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b006-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b006-122">Authorization</span></span>|<span data-ttu-id="4b006-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b006-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b006-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b006-124">Accept</span></span>|<span data-ttu-id="4b006-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b006-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b006-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b006-126">Request body</span></span>
<span data-ttu-id="4b006-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs settingStateDeviceSummary an.</span><span class="sxs-lookup"><span data-stu-id="4b006-127">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="4b006-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs settingStateDeviceSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b006-128">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="4b006-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b006-129">Property</span></span>|<span data-ttu-id="4b006-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4b006-130">Type</span></span>|<span data-ttu-id="4b006-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b006-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b006-132">id</span><span class="sxs-lookup"><span data-stu-id="4b006-132">id</span></span>|<span data-ttu-id="4b006-133">String</span><span class="sxs-lookup"><span data-stu-id="4b006-133">String</span></span>|<span data-ttu-id="4b006-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4b006-134">Key of the entity.</span></span>|
|<span data-ttu-id="4b006-135">settingName</span><span class="sxs-lookup"><span data-stu-id="4b006-135">settingName</span></span>|<span data-ttu-id="4b006-136">String</span><span class="sxs-lookup"><span data-stu-id="4b006-136">String</span></span>|<span data-ttu-id="4b006-137">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-137">Name of the setting</span></span>|
|<span data-ttu-id="4b006-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="4b006-138">instancePath</span></span>|<span data-ttu-id="4b006-139">String</span><span class="sxs-lookup"><span data-stu-id="4b006-139">String</span></span>|<span data-ttu-id="4b006-140">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="4b006-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="4b006-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-141">unknownDeviceCount</span></span>|<span data-ttu-id="4b006-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-142">Int32</span></span>|<span data-ttu-id="4b006-143">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="4b006-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="4b006-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-145">Int32</span></span>|<span data-ttu-id="4b006-146">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="4b006-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-147">compliantDeviceCount</span></span>|<span data-ttu-id="4b006-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-148">Int32</span></span>|<span data-ttu-id="4b006-149">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="4b006-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-150">remediatedDeviceCount</span></span>|<span data-ttu-id="4b006-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-151">Int32</span></span>|<span data-ttu-id="4b006-152">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="4b006-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4b006-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-154">Int32</span></span>|<span data-ttu-id="4b006-155">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="4b006-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-156">errorDeviceCount</span></span>|<span data-ttu-id="4b006-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-157">Int32</span></span>|<span data-ttu-id="4b006-158">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-158">Device error count for the setting</span></span>|
|<span data-ttu-id="4b006-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4b006-159">conflictDeviceCount</span></span>|<span data-ttu-id="4b006-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4b006-160">Int32</span></span>|<span data-ttu-id="4b006-161">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="4b006-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="4b006-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b006-162">Response</span></span>
<span data-ttu-id="4b006-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4b006-163">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b006-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b006-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b006-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b006-165">Request</span></span>
<span data-ttu-id="4b006-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b006-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="4b006-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b006-167">Response</span></span>
<span data-ttu-id="4b006-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b006-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




