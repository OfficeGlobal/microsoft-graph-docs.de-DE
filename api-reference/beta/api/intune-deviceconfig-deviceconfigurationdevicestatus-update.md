---
title: Aktualisieren von „deviceConfigurationDeviceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6baab31d895e8710d981c571e3bc4d7d8408d853
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981692"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="89644-103">Aktualisieren von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="89644-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="89644-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89644-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89644-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="89644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89644-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="89644-106">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89644-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="89644-107">Prerequisites</span></span>
<span data-ttu-id="89644-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89644-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89644-110">Permission type</span></span>|<span data-ttu-id="89644-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89644-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89644-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89644-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89644-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89644-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89644-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89644-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89644-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89644-115">Not supported.</span></span>|
|<span data-ttu-id="89644-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89644-116">Application</span></span>|<span data-ttu-id="89644-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89644-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89644-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89644-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="89644-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89644-119">Request headers</span></span>
|<span data-ttu-id="89644-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="89644-120">Header</span></span>|<span data-ttu-id="89644-121">Wert</span><span class="sxs-lookup"><span data-stu-id="89644-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89644-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89644-122">Authorization</span></span>|<span data-ttu-id="89644-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="89644-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89644-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="89644-124">Accept</span></span>|<span data-ttu-id="89644-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89644-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89644-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89644-126">Request body</span></span>
<span data-ttu-id="89644-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="89644-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="89644-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="89644-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="89644-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89644-129">Property</span></span>|<span data-ttu-id="89644-130">Typ</span><span class="sxs-lookup"><span data-stu-id="89644-130">Type</span></span>|<span data-ttu-id="89644-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89644-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89644-132">id</span><span class="sxs-lookup"><span data-stu-id="89644-132">id</span></span>|<span data-ttu-id="89644-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89644-133">String</span></span>|<span data-ttu-id="89644-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="89644-134">Key of the entity.</span></span>|
|<span data-ttu-id="89644-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="89644-135">deviceDisplayName</span></span>|<span data-ttu-id="89644-136">String</span><span class="sxs-lookup"><span data-stu-id="89644-136">String</span></span>|<span data-ttu-id="89644-137">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="89644-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="89644-138">userName</span><span class="sxs-lookup"><span data-stu-id="89644-138">userName</span></span>|<span data-ttu-id="89644-139">String</span><span class="sxs-lookup"><span data-stu-id="89644-139">String</span></span>|<span data-ttu-id="89644-140">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="89644-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="89644-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="89644-141">deviceModel</span></span>|<span data-ttu-id="89644-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89644-142">String</span></span>|<span data-ttu-id="89644-143">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="89644-143">The device model that is being reported</span></span>|
|<span data-ttu-id="89644-144">Plattform</span><span class="sxs-lookup"><span data-stu-id="89644-144">platform</span></span>|<span data-ttu-id="89644-145">Int32</span><span class="sxs-lookup"><span data-stu-id="89644-145">Int32</span></span>|<span data-ttu-id="89644-146">Plattform des gemeldeten Geräts</span><span class="sxs-lookup"><span data-stu-id="89644-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="89644-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="89644-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="89644-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89644-148">DateTimeOffset</span></span>|<span data-ttu-id="89644-149">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="89644-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="89644-150">status</span><span class="sxs-lookup"><span data-stu-id="89644-150">status</span></span>|[<span data-ttu-id="89644-151">Wurde</span><span class="sxs-lookup"><span data-stu-id="89644-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="89644-152">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="89644-152">Compliance status of the policy report.</span></span> <span data-ttu-id="89644-153">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="89644-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="89644-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="89644-154">lastReportedDateTime</span></span>|<span data-ttu-id="89644-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89644-155">DateTimeOffset</span></span>|<span data-ttu-id="89644-156">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="89644-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="89644-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89644-157">userPrincipalName</span></span>|<span data-ttu-id="89644-158">String</span><span class="sxs-lookup"><span data-stu-id="89644-158">String</span></span>|<span data-ttu-id="89644-159">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="89644-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="89644-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="89644-160">Response</span></span>
<span data-ttu-id="89644-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="89644-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89644-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89644-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="89644-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89644-163">Request</span></span>
<span data-ttu-id="89644-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89644-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="89644-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="89644-165">Response</span></span>
<span data-ttu-id="89644-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89644-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




