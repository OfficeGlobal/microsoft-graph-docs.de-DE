---
title: Erstellen von „iosUpdateDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs iosUpdateDeviceStatus.
ms.openlocfilehash: 205bc02b37f3ba846e2fc7df0685d50fbd9e5279
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063021"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="77f7e-103">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="77f7e-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="77f7e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77f7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77f7e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77f7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77f7e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="77f7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77f7e-107">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="77f7e-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77f7e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77f7e-108">Prerequisites</span></span>
<span data-ttu-id="77f7e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f7e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77f7e-111">Permission type</span></span>|<span data-ttu-id="77f7e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77f7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77f7e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77f7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77f7e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f7e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77f7e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77f7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77f7e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77f7e-116">Not supported.</span></span>|
|<span data-ttu-id="77f7e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77f7e-117">Application</span></span>|<span data-ttu-id="77f7e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77f7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77f7e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77f7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="77f7e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77f7e-120">Request headers</span></span>
|<span data-ttu-id="77f7e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77f7e-121">Header</span></span>|<span data-ttu-id="77f7e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="77f7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77f7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77f7e-123">Authorization</span></span>|<span data-ttu-id="77f7e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77f7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77f7e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77f7e-125">Accept</span></span>|<span data-ttu-id="77f7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77f7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f7e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77f7e-127">Request body</span></span>
<span data-ttu-id="77f7e-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="77f7e-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="77f7e-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="77f7e-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="77f7e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77f7e-130">Property</span></span>|<span data-ttu-id="77f7e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="77f7e-131">Type</span></span>|<span data-ttu-id="77f7e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77f7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f7e-133">id</span><span class="sxs-lookup"><span data-stu-id="77f7e-133">id</span></span>|<span data-ttu-id="77f7e-134">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-134">String</span></span>|<span data-ttu-id="77f7e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="77f7e-135">Key of the entity.</span></span>|
|<span data-ttu-id="77f7e-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="77f7e-136">installStatus</span></span>|[<span data-ttu-id="77f7e-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="77f7e-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="77f7e-138">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="77f7e-138">The installation status of the policy report.</span></span> <span data-ttu-id="77f7e-139">Mögliche Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="77f7e-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="77f7e-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="77f7e-140">osVersion</span></span>|<span data-ttu-id="77f7e-141">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-141">String</span></span>|<span data-ttu-id="77f7e-142">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="77f7e-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="77f7e-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="77f7e-143">deviceId</span></span>|<span data-ttu-id="77f7e-144">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-144">String</span></span>|<span data-ttu-id="77f7e-145">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="77f7e-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="77f7e-146">userId</span><span class="sxs-lookup"><span data-stu-id="77f7e-146">userId</span></span>|<span data-ttu-id="77f7e-147">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-147">String</span></span>|<span data-ttu-id="77f7e-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="77f7e-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="77f7e-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="77f7e-149">deviceDisplayName</span></span>|<span data-ttu-id="77f7e-150">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-150">String</span></span>|<span data-ttu-id="77f7e-151">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="77f7e-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="77f7e-152">userName</span><span class="sxs-lookup"><span data-stu-id="77f7e-152">userName</span></span>|<span data-ttu-id="77f7e-153">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-153">String</span></span>|<span data-ttu-id="77f7e-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="77f7e-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="77f7e-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="77f7e-155">deviceModel</span></span>|<span data-ttu-id="77f7e-156">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-156">String</span></span>|<span data-ttu-id="77f7e-157">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="77f7e-157">The device model that is being reported</span></span>|
|<span data-ttu-id="77f7e-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="77f7e-158">platform</span></span>|<span data-ttu-id="77f7e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="77f7e-159">Int32</span></span>|<span data-ttu-id="77f7e-160">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="77f7e-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="77f7e-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="77f7e-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="77f7e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f7e-162">DateTimeOffset</span></span>|<span data-ttu-id="77f7e-163">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="77f7e-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="77f7e-164">status</span><span class="sxs-lookup"><span data-stu-id="77f7e-164">status</span></span>|[<span data-ttu-id="77f7e-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="77f7e-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="77f7e-166">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="77f7e-166">Compliance status of the policy report.</span></span> <span data-ttu-id="77f7e-167">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="77f7e-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="77f7e-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="77f7e-168">lastReportedDateTime</span></span>|<span data-ttu-id="77f7e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f7e-169">DateTimeOffset</span></span>|<span data-ttu-id="77f7e-170">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="77f7e-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="77f7e-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="77f7e-171">userPrincipalName</span></span>|<span data-ttu-id="77f7e-172">String</span><span class="sxs-lookup"><span data-stu-id="77f7e-172">String</span></span>|<span data-ttu-id="77f7e-173">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="77f7e-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="77f7e-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="77f7e-174">Response</span></span>
<span data-ttu-id="77f7e-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77f7e-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f7e-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77f7e-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="77f7e-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77f7e-177">Request</span></span>
<span data-ttu-id="77f7e-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77f7e-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
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

### <a name="response"></a><span data-ttu-id="77f7e-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="77f7e-179">Response</span></span>
<span data-ttu-id="77f7e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77f7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 619

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
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





