---
title: Erstellen von „deviceConfigurationDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec890b9e1d876f7bdc23a2952e5a7163deadfc45
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171260"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="70f9c-103">Erstellen von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="70f9c-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="70f9c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70f9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70f9c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70f9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70f9c-106">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="70f9c-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70f9c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70f9c-107">Prerequisites</span></span>
<span data-ttu-id="70f9c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="70f9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="70f9c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70f9c-110">Permission type</span></span>|<span data-ttu-id="70f9c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70f9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70f9c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70f9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70f9c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f9c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70f9c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70f9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70f9c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70f9c-115">Not supported.</span></span>|
|<span data-ttu-id="70f9c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70f9c-116">Application</span></span>|<span data-ttu-id="70f9c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70f9c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70f9c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70f9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="70f9c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70f9c-119">Request headers</span></span>
|<span data-ttu-id="70f9c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70f9c-120">Header</span></span>|<span data-ttu-id="70f9c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="70f9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70f9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70f9c-122">Authorization</span></span>|<span data-ttu-id="70f9c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70f9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70f9c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70f9c-124">Accept</span></span>|<span data-ttu-id="70f9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70f9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70f9c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70f9c-126">Request body</span></span>
<span data-ttu-id="70f9c-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="70f9c-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="70f9c-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="70f9c-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="70f9c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70f9c-129">Property</span></span>|<span data-ttu-id="70f9c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="70f9c-130">Type</span></span>|<span data-ttu-id="70f9c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70f9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70f9c-132">id</span><span class="sxs-lookup"><span data-stu-id="70f9c-132">id</span></span>|<span data-ttu-id="70f9c-133">String</span><span class="sxs-lookup"><span data-stu-id="70f9c-133">String</span></span>|<span data-ttu-id="70f9c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="70f9c-134">Key of the entity.</span></span>|
|<span data-ttu-id="70f9c-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="70f9c-135">deviceDisplayName</span></span>|<span data-ttu-id="70f9c-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70f9c-136">String</span></span>|<span data-ttu-id="70f9c-137">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="70f9c-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="70f9c-138">userName</span><span class="sxs-lookup"><span data-stu-id="70f9c-138">userName</span></span>|<span data-ttu-id="70f9c-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70f9c-139">String</span></span>|<span data-ttu-id="70f9c-140">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="70f9c-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="70f9c-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="70f9c-141">deviceModel</span></span>|<span data-ttu-id="70f9c-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70f9c-142">String</span></span>|<span data-ttu-id="70f9c-143">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="70f9c-143">The device model that is being reported</span></span>|
|<span data-ttu-id="70f9c-144">Plattform</span><span class="sxs-lookup"><span data-stu-id="70f9c-144">platform</span></span>|<span data-ttu-id="70f9c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="70f9c-145">Int32</span></span>|<span data-ttu-id="70f9c-146">Plattform des gemeldeten Geräts</span><span class="sxs-lookup"><span data-stu-id="70f9c-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="70f9c-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="70f9c-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="70f9c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70f9c-148">DateTimeOffset</span></span>|<span data-ttu-id="70f9c-149">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="70f9c-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="70f9c-150">status</span><span class="sxs-lookup"><span data-stu-id="70f9c-150">status</span></span>|[<span data-ttu-id="70f9c-151">Wurde</span><span class="sxs-lookup"><span data-stu-id="70f9c-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="70f9c-152">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="70f9c-152">Compliance status of the policy report.</span></span> <span data-ttu-id="70f9c-153">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="70f9c-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="70f9c-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="70f9c-154">lastReportedDateTime</span></span>|<span data-ttu-id="70f9c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70f9c-155">DateTimeOffset</span></span>|<span data-ttu-id="70f9c-156">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="70f9c-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="70f9c-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70f9c-157">userPrincipalName</span></span>|<span data-ttu-id="70f9c-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70f9c-158">String</span></span>|<span data-ttu-id="70f9c-159">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="70f9c-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="70f9c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="70f9c-160">Response</span></span>
<span data-ttu-id="70f9c-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="70f9c-161">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70f9c-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70f9c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="70f9c-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70f9c-163">Request</span></span>
<span data-ttu-id="70f9c-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70f9c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="70f9c-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="70f9c-165">Response</span></span>
<span data-ttu-id="70f9c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70f9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




