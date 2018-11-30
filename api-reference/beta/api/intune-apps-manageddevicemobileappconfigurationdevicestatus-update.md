---
title: ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ManagedDeviceMobileAppConfigurationDeviceStatus-Objekts.
ms.openlocfilehash: 92f3b2e4b119f1da552d276f4c59b8bdac2e55e3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062352"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="f23c8-103">ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f23c8-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="f23c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f23c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f23c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f23c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f23c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f23c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f23c8-107">Aktualisieren Sie die Eigenschaften eines [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f23c8-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f23c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f23c8-108">Prerequisites</span></span>
<span data-ttu-id="f23c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f23c8-111">Permission type</span></span>|<span data-ttu-id="f23c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f23c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f23c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f23c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f23c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23c8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f23c8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f23c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f23c8-116">Not supported.</span></span>|
|<span data-ttu-id="f23c8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f23c8-117">Application</span></span>|<span data-ttu-id="f23c8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f23c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23c8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f23c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f23c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f23c8-120">Request headers</span></span>
|<span data-ttu-id="f23c8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f23c8-121">Header</span></span>|<span data-ttu-id="f23c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f23c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f23c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23c8-123">Authorization</span></span>|<span data-ttu-id="f23c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f23c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f23c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f23c8-125">Accept</span></span>|<span data-ttu-id="f23c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f23c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f23c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f23c8-127">Request body</span></span>
<span data-ttu-id="f23c8-128">Geben Sie im Textkörper Anforderung für das Objekt [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f23c8-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="f23c8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f23c8-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="f23c8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f23c8-130">Property</span></span>|<span data-ttu-id="f23c8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f23c8-131">Type</span></span>|<span data-ttu-id="f23c8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f23c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23c8-133">id</span><span class="sxs-lookup"><span data-stu-id="f23c8-133">id</span></span>|<span data-ttu-id="f23c8-134">String</span><span class="sxs-lookup"><span data-stu-id="f23c8-134">String</span></span>|<span data-ttu-id="f23c8-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f23c8-135">Key of the entity.</span></span>|
|<span data-ttu-id="f23c8-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f23c8-136">deviceDisplayName</span></span>|<span data-ttu-id="f23c8-137">String</span><span class="sxs-lookup"><span data-stu-id="f23c8-137">String</span></span>|<span data-ttu-id="f23c8-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="f23c8-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f23c8-139">userName</span><span class="sxs-lookup"><span data-stu-id="f23c8-139">userName</span></span>|<span data-ttu-id="f23c8-140">String</span><span class="sxs-lookup"><span data-stu-id="f23c8-140">String</span></span>|<span data-ttu-id="f23c8-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="f23c8-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="f23c8-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f23c8-142">deviceModel</span></span>|<span data-ttu-id="f23c8-143">String</span><span class="sxs-lookup"><span data-stu-id="f23c8-143">String</span></span>|<span data-ttu-id="f23c8-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="f23c8-144">The device model that is being reported</span></span>|
|<span data-ttu-id="f23c8-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="f23c8-145">platform</span></span>|<span data-ttu-id="f23c8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f23c8-146">Int32</span></span>|<span data-ttu-id="f23c8-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="f23c8-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="f23c8-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f23c8-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f23c8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23c8-149">DateTimeOffset</span></span>|<span data-ttu-id="f23c8-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="f23c8-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f23c8-151">status</span><span class="sxs-lookup"><span data-stu-id="f23c8-151">status</span></span>|[<span data-ttu-id="f23c8-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f23c8-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f23c8-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="f23c8-153">Compliance status of the policy report.</span></span> <span data-ttu-id="f23c8-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f23c8-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f23c8-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f23c8-155">lastReportedDateTime</span></span>|<span data-ttu-id="f23c8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23c8-156">DateTimeOffset</span></span>|<span data-ttu-id="f23c8-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="f23c8-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f23c8-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f23c8-158">userPrincipalName</span></span>|<span data-ttu-id="f23c8-159">String</span><span class="sxs-lookup"><span data-stu-id="f23c8-159">String</span></span>|<span data-ttu-id="f23c8-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="f23c8-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f23c8-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="f23c8-161">Response</span></span>
<span data-ttu-id="f23c8-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f23c8-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23c8-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f23c8-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="f23c8-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f23c8-164">Request</span></span>
<span data-ttu-id="f23c8-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f23c8-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 377

{
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

### <a name="response"></a><span data-ttu-id="f23c8-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="f23c8-166">Response</span></span>
<span data-ttu-id="f23c8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f23c8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
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





