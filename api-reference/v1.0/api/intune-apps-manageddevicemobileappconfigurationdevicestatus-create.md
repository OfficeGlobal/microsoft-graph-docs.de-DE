---
title: Erstellen von managedDeviceMobileAppConfigurationDeviceStatus
description: Erstellen eines neuen ManagedDeviceMobileAppConfigurationDeviceStatus-Objekts.
author: tfitzmac
ms.openlocfilehash: 8a9b709104119622b2555c2a05548789de134363
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318036"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="86c3e-103">Erstellen von managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="86c3e-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="86c3e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="86c3e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86c3e-105">Erstellen eines neuen [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="86c3e-105">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86c3e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86c3e-106">Prerequisites</span></span>
<span data-ttu-id="86c3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c3e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86c3e-109">Permission type</span></span>|<span data-ttu-id="86c3e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86c3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86c3e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86c3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86c3e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c3e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86c3e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86c3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86c3e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86c3e-114">Not supported.</span></span>|
|<span data-ttu-id="86c3e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86c3e-115">Application</span></span>|<span data-ttu-id="86c3e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86c3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86c3e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86c3e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="86c3e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86c3e-118">Request headers</span></span>
|<span data-ttu-id="86c3e-119">Header</span><span class="sxs-lookup"><span data-stu-id="86c3e-119">Header</span></span>|<span data-ttu-id="86c3e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="86c3e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86c3e-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="86c3e-121">Authorization</span></span>|<span data-ttu-id="86c3e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86c3e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86c3e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="86c3e-123">Accept</span></span>|<span data-ttu-id="86c3e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86c3e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c3e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86c3e-125">Request body</span></span>
<span data-ttu-id="86c3e-126">Geben Sie im Textkörper Anforderung für das Objekt ManagedDeviceMobileAppConfigurationDeviceStatus eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="86c3e-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="86c3e-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ManagedDeviceMobileAppConfigurationDeviceStatus erstellen.</span><span class="sxs-lookup"><span data-stu-id="86c3e-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="86c3e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86c3e-128">Property</span></span>|<span data-ttu-id="86c3e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="86c3e-129">Type</span></span>|<span data-ttu-id="86c3e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86c3e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c3e-131">id</span><span class="sxs-lookup"><span data-stu-id="86c3e-131">id</span></span>|<span data-ttu-id="86c3e-132">String</span><span class="sxs-lookup"><span data-stu-id="86c3e-132">String</span></span>|<span data-ttu-id="86c3e-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="86c3e-133">Key of the entity.</span></span>|
|<span data-ttu-id="86c3e-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="86c3e-134">deviceDisplayName</span></span>|<span data-ttu-id="86c3e-135">String</span><span class="sxs-lookup"><span data-stu-id="86c3e-135">String</span></span>|<span data-ttu-id="86c3e-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="86c3e-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="86c3e-137">userName</span><span class="sxs-lookup"><span data-stu-id="86c3e-137">userName</span></span>|<span data-ttu-id="86c3e-138">String</span><span class="sxs-lookup"><span data-stu-id="86c3e-138">String</span></span>|<span data-ttu-id="86c3e-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="86c3e-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="86c3e-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="86c3e-140">deviceModel</span></span>|<span data-ttu-id="86c3e-141">String</span><span class="sxs-lookup"><span data-stu-id="86c3e-141">String</span></span>|<span data-ttu-id="86c3e-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="86c3e-142">The device model that is being reported</span></span>|
|<span data-ttu-id="86c3e-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="86c3e-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="86c3e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86c3e-144">DateTimeOffset</span></span>|<span data-ttu-id="86c3e-145">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="86c3e-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="86c3e-146">status</span><span class="sxs-lookup"><span data-stu-id="86c3e-146">status</span></span>|[<span data-ttu-id="86c3e-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="86c3e-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="86c3e-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="86c3e-148">Compliance status of the policy report.</span></span> <span data-ttu-id="86c3e-149">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="86c3e-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="86c3e-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="86c3e-150">lastReportedDateTime</span></span>|<span data-ttu-id="86c3e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86c3e-151">DateTimeOffset</span></span>|<span data-ttu-id="86c3e-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="86c3e-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="86c3e-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86c3e-153">userPrincipalName</span></span>|<span data-ttu-id="86c3e-154">String</span><span class="sxs-lookup"><span data-stu-id="86c3e-154">String</span></span>|<span data-ttu-id="86c3e-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="86c3e-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="86c3e-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="86c3e-156">Response</span></span>
<span data-ttu-id="86c3e-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="86c3e-157">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c3e-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86c3e-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="86c3e-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86c3e-159">Request</span></span>
<span data-ttu-id="86c3e-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86c3e-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="86c3e-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="86c3e-161">Response</span></span>
<span data-ttu-id="86c3e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86c3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



