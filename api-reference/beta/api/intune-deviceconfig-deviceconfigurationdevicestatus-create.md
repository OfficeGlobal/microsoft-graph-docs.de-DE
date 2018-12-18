---
title: Erstellen von „deviceConfigurationDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: a43af27a299d131947a1c9d95e6b01e68270f491
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310472"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="776f4-103">Erstellen von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="776f4-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="776f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="776f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="776f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="776f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="776f4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="776f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="776f4-107">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="776f4-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="776f4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="776f4-108">Prerequisites</span></span>
<span data-ttu-id="776f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="776f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="776f4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="776f4-111">Permission type</span></span>|<span data-ttu-id="776f4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="776f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="776f4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="776f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="776f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="776f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="776f4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="776f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="776f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="776f4-116">Not supported.</span></span>|
|<span data-ttu-id="776f4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="776f4-117">Application</span></span>|<span data-ttu-id="776f4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="776f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="776f4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="776f4-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="776f4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="776f4-120">Request headers</span></span>
|<span data-ttu-id="776f4-121">Header</span><span class="sxs-lookup"><span data-stu-id="776f4-121">Header</span></span>|<span data-ttu-id="776f4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="776f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="776f4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="776f4-123">Authorization</span></span>|<span data-ttu-id="776f4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="776f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="776f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="776f4-125">Accept</span></span>|<span data-ttu-id="776f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="776f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="776f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="776f4-127">Request body</span></span>
<span data-ttu-id="776f4-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="776f4-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="776f4-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="776f4-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="776f4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="776f4-130">Property</span></span>|<span data-ttu-id="776f4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="776f4-131">Type</span></span>|<span data-ttu-id="776f4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="776f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="776f4-133">id</span><span class="sxs-lookup"><span data-stu-id="776f4-133">id</span></span>|<span data-ttu-id="776f4-134">String</span><span class="sxs-lookup"><span data-stu-id="776f4-134">String</span></span>|<span data-ttu-id="776f4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="776f4-135">Key of the entity.</span></span>|
|<span data-ttu-id="776f4-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="776f4-136">deviceDisplayName</span></span>|<span data-ttu-id="776f4-137">String</span><span class="sxs-lookup"><span data-stu-id="776f4-137">String</span></span>|<span data-ttu-id="776f4-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="776f4-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="776f4-139">userName</span><span class="sxs-lookup"><span data-stu-id="776f4-139">userName</span></span>|<span data-ttu-id="776f4-140">String</span><span class="sxs-lookup"><span data-stu-id="776f4-140">String</span></span>|<span data-ttu-id="776f4-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="776f4-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="776f4-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="776f4-142">deviceModel</span></span>|<span data-ttu-id="776f4-143">String</span><span class="sxs-lookup"><span data-stu-id="776f4-143">String</span></span>|<span data-ttu-id="776f4-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="776f4-144">The device model that is being reported</span></span>|
|<span data-ttu-id="776f4-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="776f4-145">platform</span></span>|<span data-ttu-id="776f4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="776f4-146">Int32</span></span>|<span data-ttu-id="776f4-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="776f4-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="776f4-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="776f4-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="776f4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="776f4-149">DateTimeOffset</span></span>|<span data-ttu-id="776f4-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="776f4-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="776f4-151">status</span><span class="sxs-lookup"><span data-stu-id="776f4-151">status</span></span>|[<span data-ttu-id="776f4-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="776f4-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="776f4-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="776f4-153">Compliance status of the policy report.</span></span> <span data-ttu-id="776f4-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="776f4-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="776f4-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="776f4-155">lastReportedDateTime</span></span>|<span data-ttu-id="776f4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="776f4-156">DateTimeOffset</span></span>|<span data-ttu-id="776f4-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="776f4-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="776f4-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="776f4-158">userPrincipalName</span></span>|<span data-ttu-id="776f4-159">String</span><span class="sxs-lookup"><span data-stu-id="776f4-159">String</span></span>|<span data-ttu-id="776f4-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="776f4-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="776f4-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="776f4-161">Response</span></span>
<span data-ttu-id="776f4-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="776f4-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="776f4-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="776f4-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="776f4-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="776f4-164">Request</span></span>
<span data-ttu-id="776f4-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="776f4-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="776f4-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="776f4-166">Response</span></span>
<span data-ttu-id="776f4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="776f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





