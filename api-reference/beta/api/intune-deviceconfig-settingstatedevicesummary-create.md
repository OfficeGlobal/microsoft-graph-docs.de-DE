---
title: settingStateDeviceSummary erstellen
description: Erstellen eines neuen SettingStateDeviceSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 06c9851a534f59be935791e1c1f435d2180bf9d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852108"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="9bbbe-103">settingStateDeviceSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="9bbbe-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="9bbbe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bbbe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bbbe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bbbe-107">Erstellen eines neuen [SettingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-107">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9bbbe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9bbbe-108">Prerequisites</span></span>
<span data-ttu-id="9bbbe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bbbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bbbe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bbbe-111">Permission type</span></span>|<span data-ttu-id="9bbbe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bbbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bbbe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bbbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bbbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bbbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bbbe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bbbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bbbe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bbbe-116">Not supported.</span></span>|
|<span data-ttu-id="9bbbe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-117">Application</span></span>|<span data-ttu-id="9bbbe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bbbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bbbe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9bbbe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bbbe-120">Request headers</span></span>
|<span data-ttu-id="9bbbe-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9bbbe-121">Header</span></span>|<span data-ttu-id="9bbbe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9bbbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bbbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bbbe-123">Authorization</span></span>|<span data-ttu-id="9bbbe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9bbbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bbbe-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9bbbe-125">Accept</span></span>|<span data-ttu-id="9bbbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bbbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bbbe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bbbe-127">Request body</span></span>
<span data-ttu-id="9bbbe-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs settingStateDeviceSummary an.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-128">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="9bbbe-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs settingStateDeviceSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-129">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="9bbbe-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9bbbe-130">Property</span></span>|<span data-ttu-id="9bbbe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9bbbe-131">Type</span></span>|<span data-ttu-id="9bbbe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bbbe-133">id</span><span class="sxs-lookup"><span data-stu-id="9bbbe-133">id</span></span>|<span data-ttu-id="9bbbe-134">String</span><span class="sxs-lookup"><span data-stu-id="9bbbe-134">String</span></span>|<span data-ttu-id="9bbbe-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9bbbe-135">Key of the entity.</span></span>|
|<span data-ttu-id="9bbbe-136">settingName</span><span class="sxs-lookup"><span data-stu-id="9bbbe-136">settingName</span></span>|<span data-ttu-id="9bbbe-137">String</span><span class="sxs-lookup"><span data-stu-id="9bbbe-137">String</span></span>|<span data-ttu-id="9bbbe-138">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-138">Name of the setting</span></span>|
|<span data-ttu-id="9bbbe-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="9bbbe-139">instancePath</span></span>|<span data-ttu-id="9bbbe-140">String</span><span class="sxs-lookup"><span data-stu-id="9bbbe-140">String</span></span>|<span data-ttu-id="9bbbe-141">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="9bbbe-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="9bbbe-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-142">unknownDeviceCount</span></span>|<span data-ttu-id="9bbbe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-143">Int32</span></span>|<span data-ttu-id="9bbbe-144">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="9bbbe-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="9bbbe-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-146">Int32</span></span>|<span data-ttu-id="9bbbe-147">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="9bbbe-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-148">compliantDeviceCount</span></span>|<span data-ttu-id="9bbbe-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-149">Int32</span></span>|<span data-ttu-id="9bbbe-150">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="9bbbe-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-151">remediatedDeviceCount</span></span>|<span data-ttu-id="9bbbe-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-152">Int32</span></span>|<span data-ttu-id="9bbbe-153">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="9bbbe-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9bbbe-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-155">Int32</span></span>|<span data-ttu-id="9bbbe-156">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="9bbbe-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-157">errorDeviceCount</span></span>|<span data-ttu-id="9bbbe-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-158">Int32</span></span>|<span data-ttu-id="9bbbe-159">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-159">Device error count for the setting</span></span>|
|<span data-ttu-id="9bbbe-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bbbe-160">conflictDeviceCount</span></span>|<span data-ttu-id="9bbbe-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9bbbe-161">Int32</span></span>|<span data-ttu-id="9bbbe-162">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="9bbbe-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bbbe-163">Response</span></span>
<span data-ttu-id="9bbbe-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-164">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bbbe-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bbbe-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bbbe-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bbbe-166">Request</span></span>
<span data-ttu-id="9bbbe-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9bbbe-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bbbe-168">Response</span></span>
<span data-ttu-id="9bbbe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bbbe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





