---
title: Aktualisieren von „deviceConfigurationDeviceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5fa3cbdcc5d359625285048a2e1c66bbecb2cc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417105"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="80c04-103">Aktualisieren von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="80c04-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="80c04-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="80c04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80c04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80c04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80c04-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80c04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80c04-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="80c04-107">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80c04-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80c04-108">Prerequisites</span></span>
<span data-ttu-id="80c04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="80c04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="80c04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80c04-111">Permission type</span></span>|<span data-ttu-id="80c04-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80c04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80c04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80c04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80c04-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c04-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80c04-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80c04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80c04-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80c04-116">Not supported.</span></span>|
|<span data-ttu-id="80c04-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80c04-117">Application</span></span>|<span data-ttu-id="80c04-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80c04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80c04-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80c04-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="80c04-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80c04-120">Request headers</span></span>
|<span data-ttu-id="80c04-121">Header</span><span class="sxs-lookup"><span data-stu-id="80c04-121">Header</span></span>|<span data-ttu-id="80c04-122">Wert</span><span class="sxs-lookup"><span data-stu-id="80c04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80c04-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="80c04-123">Authorization</span></span>|<span data-ttu-id="80c04-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80c04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80c04-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80c04-125">Accept</span></span>|<span data-ttu-id="80c04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80c04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80c04-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80c04-127">Request body</span></span>
<span data-ttu-id="80c04-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="80c04-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="80c04-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="80c04-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="80c04-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80c04-130">Property</span></span>|<span data-ttu-id="80c04-131">Typ</span><span class="sxs-lookup"><span data-stu-id="80c04-131">Type</span></span>|<span data-ttu-id="80c04-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80c04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c04-133">id</span><span class="sxs-lookup"><span data-stu-id="80c04-133">id</span></span>|<span data-ttu-id="80c04-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80c04-134">String</span></span>|<span data-ttu-id="80c04-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="80c04-135">Key of the entity.</span></span>|
|<span data-ttu-id="80c04-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="80c04-136">deviceDisplayName</span></span>|<span data-ttu-id="80c04-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80c04-137">String</span></span>|<span data-ttu-id="80c04-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="80c04-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="80c04-139">userName</span><span class="sxs-lookup"><span data-stu-id="80c04-139">userName</span></span>|<span data-ttu-id="80c04-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80c04-140">String</span></span>|<span data-ttu-id="80c04-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="80c04-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="80c04-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="80c04-142">deviceModel</span></span>|<span data-ttu-id="80c04-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80c04-143">String</span></span>|<span data-ttu-id="80c04-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="80c04-144">The device model that is being reported</span></span>|
|<span data-ttu-id="80c04-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="80c04-145">platform</span></span>|<span data-ttu-id="80c04-146">Int32</span><span class="sxs-lookup"><span data-stu-id="80c04-146">Int32</span></span>|<span data-ttu-id="80c04-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="80c04-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="80c04-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="80c04-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="80c04-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c04-149">DateTimeOffset</span></span>|<span data-ttu-id="80c04-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="80c04-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="80c04-151">status</span><span class="sxs-lookup"><span data-stu-id="80c04-151">status</span></span>|[<span data-ttu-id="80c04-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="80c04-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="80c04-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="80c04-153">Compliance status of the policy report.</span></span> <span data-ttu-id="80c04-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="80c04-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="80c04-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="80c04-155">lastReportedDateTime</span></span>|<span data-ttu-id="80c04-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c04-156">DateTimeOffset</span></span>|<span data-ttu-id="80c04-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="80c04-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="80c04-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80c04-158">userPrincipalName</span></span>|<span data-ttu-id="80c04-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80c04-159">String</span></span>|<span data-ttu-id="80c04-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="80c04-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="80c04-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="80c04-161">Response</span></span>
<span data-ttu-id="80c04-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="80c04-162">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80c04-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80c04-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="80c04-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80c04-164">Request</span></span>
<span data-ttu-id="80c04-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80c04-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80c04-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="80c04-166">Response</span></span>
<span data-ttu-id="80c04-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80c04-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




