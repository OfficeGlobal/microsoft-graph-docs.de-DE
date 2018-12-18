---
title: Erstellen von „iosUpdateDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs iosUpdateDeviceStatus.
author: tfitzmac
ms.openlocfilehash: aa953684b79b4bca2453f55de9be5754a29ba86c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309282"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="6324a-103">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="6324a-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="6324a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6324a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6324a-105">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6324a-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6324a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6324a-106">Prerequisites</span></span>
<span data-ttu-id="6324a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6324a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6324a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6324a-109">Permission type</span></span>|<span data-ttu-id="6324a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6324a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6324a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6324a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6324a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6324a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6324a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6324a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6324a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6324a-114">Not supported.</span></span>|
|<span data-ttu-id="6324a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6324a-115">Application</span></span>|<span data-ttu-id="6324a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6324a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6324a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6324a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6324a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6324a-118">Request headers</span></span>
|<span data-ttu-id="6324a-119">Header</span><span class="sxs-lookup"><span data-stu-id="6324a-119">Header</span></span>|<span data-ttu-id="6324a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6324a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6324a-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6324a-121">Authorization</span></span>|<span data-ttu-id="6324a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6324a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6324a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6324a-123">Accept</span></span>|<span data-ttu-id="6324a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6324a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6324a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6324a-125">Request body</span></span>
<span data-ttu-id="6324a-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="6324a-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="6324a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6324a-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="6324a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6324a-128">Property</span></span>|<span data-ttu-id="6324a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6324a-129">Type</span></span>|<span data-ttu-id="6324a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6324a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6324a-131">id</span><span class="sxs-lookup"><span data-stu-id="6324a-131">id</span></span>|<span data-ttu-id="6324a-132">String</span><span class="sxs-lookup"><span data-stu-id="6324a-132">String</span></span>|<span data-ttu-id="6324a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6324a-133">Key of the entity.</span></span>|
|<span data-ttu-id="6324a-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="6324a-134">installStatus</span></span>|[<span data-ttu-id="6324a-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6324a-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="6324a-136">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="6324a-136">The installation status of the policy report.</span></span> <span data-ttu-id="6324a-137">Mögliche Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="6324a-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="6324a-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="6324a-138">osVersion</span></span>|<span data-ttu-id="6324a-139">String</span><span class="sxs-lookup"><span data-stu-id="6324a-139">String</span></span>|<span data-ttu-id="6324a-140">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="6324a-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="6324a-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="6324a-141">deviceId</span></span>|<span data-ttu-id="6324a-142">String</span><span class="sxs-lookup"><span data-stu-id="6324a-142">String</span></span>|<span data-ttu-id="6324a-143">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="6324a-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="6324a-144">userId</span><span class="sxs-lookup"><span data-stu-id="6324a-144">userId</span></span>|<span data-ttu-id="6324a-145">String</span><span class="sxs-lookup"><span data-stu-id="6324a-145">String</span></span>|<span data-ttu-id="6324a-146">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="6324a-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="6324a-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6324a-147">deviceDisplayName</span></span>|<span data-ttu-id="6324a-148">String</span><span class="sxs-lookup"><span data-stu-id="6324a-148">String</span></span>|<span data-ttu-id="6324a-149">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="6324a-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6324a-150">userName</span><span class="sxs-lookup"><span data-stu-id="6324a-150">userName</span></span>|<span data-ttu-id="6324a-151">String</span><span class="sxs-lookup"><span data-stu-id="6324a-151">String</span></span>|<span data-ttu-id="6324a-152">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="6324a-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="6324a-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6324a-153">deviceModel</span></span>|<span data-ttu-id="6324a-154">String</span><span class="sxs-lookup"><span data-stu-id="6324a-154">String</span></span>|<span data-ttu-id="6324a-155">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="6324a-155">The device model that is being reported</span></span>|
|<span data-ttu-id="6324a-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6324a-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6324a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6324a-157">DateTimeOffset</span></span>|<span data-ttu-id="6324a-158">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="6324a-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6324a-159">status</span><span class="sxs-lookup"><span data-stu-id="6324a-159">status</span></span>|[<span data-ttu-id="6324a-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6324a-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6324a-161">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="6324a-161">Compliance status of the policy report.</span></span> <span data-ttu-id="6324a-162">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6324a-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6324a-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6324a-163">lastReportedDateTime</span></span>|<span data-ttu-id="6324a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6324a-164">DateTimeOffset</span></span>|<span data-ttu-id="6324a-165">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="6324a-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6324a-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6324a-166">userPrincipalName</span></span>|<span data-ttu-id="6324a-167">String</span><span class="sxs-lookup"><span data-stu-id="6324a-167">String</span></span>|<span data-ttu-id="6324a-168">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="6324a-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6324a-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="6324a-169">Response</span></span>
<span data-ttu-id="6324a-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6324a-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6324a-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6324a-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="6324a-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6324a-172">Request</span></span>
<span data-ttu-id="6324a-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6324a-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="6324a-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="6324a-174">Response</span></span>
<span data-ttu-id="6324a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6324a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 601

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
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



