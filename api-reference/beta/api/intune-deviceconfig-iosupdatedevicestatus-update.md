---
title: iosUpdateDeviceStatus aktualisieren
description: Aktualisieren der Eigenschaften eines iosUpdateDeviceStatus-Objekts.
ms.openlocfilehash: 2b652dd6208dee20f164d57c92a8f0d322a58d8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063119"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="2c706-103">iosUpdateDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2c706-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="2c706-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2c706-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c706-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c706-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c706-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2c706-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c706-107">Aktualisieren der Eigenschaften eines [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c706-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2c706-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2c706-108">Prerequisites</span></span>
<span data-ttu-id="2c706-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c706-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c706-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c706-111">Permission type</span></span>|<span data-ttu-id="2c706-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c706-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c706-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c706-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c706-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c706-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c706-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c706-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c706-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c706-116">Not supported.</span></span>|
|<span data-ttu-id="2c706-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2c706-117">Application</span></span>|<span data-ttu-id="2c706-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c706-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c706-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c706-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2c706-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2c706-120">Request headers</span></span>
|<span data-ttu-id="2c706-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2c706-121">Header</span></span>|<span data-ttu-id="2c706-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2c706-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c706-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c706-123">Authorization</span></span>|<span data-ttu-id="2c706-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2c706-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c706-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c706-125">Accept</span></span>|<span data-ttu-id="2c706-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c706-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c706-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c706-127">Request body</span></span>
<span data-ttu-id="2c706-128">Geben Sie im Anforderungstext eine JSON Darstellung für das Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="2c706-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="2c706-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2c706-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="2c706-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c706-130">Property</span></span>|<span data-ttu-id="2c706-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2c706-131">Type</span></span>|<span data-ttu-id="2c706-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c706-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c706-133">id</span><span class="sxs-lookup"><span data-stu-id="2c706-133">id</span></span>|<span data-ttu-id="2c706-134">String</span><span class="sxs-lookup"><span data-stu-id="2c706-134">String</span></span>|<span data-ttu-id="2c706-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2c706-135">Key of the entity.</span></span>|
|<span data-ttu-id="2c706-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="2c706-136">installStatus</span></span>|[<span data-ttu-id="2c706-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2c706-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="2c706-138">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="2c706-138">The installation status of the policy report.</span></span> <span data-ttu-id="2c706-139">Mögliche Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="2c706-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="2c706-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="2c706-140">osVersion</span></span>|<span data-ttu-id="2c706-141">String</span><span class="sxs-lookup"><span data-stu-id="2c706-141">String</span></span>|<span data-ttu-id="2c706-142">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="2c706-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="2c706-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="2c706-143">deviceId</span></span>|<span data-ttu-id="2c706-144">String</span><span class="sxs-lookup"><span data-stu-id="2c706-144">String</span></span>|<span data-ttu-id="2c706-145">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="2c706-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="2c706-146">userId</span><span class="sxs-lookup"><span data-stu-id="2c706-146">userId</span></span>|<span data-ttu-id="2c706-147">String</span><span class="sxs-lookup"><span data-stu-id="2c706-147">String</span></span>|<span data-ttu-id="2c706-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="2c706-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="2c706-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2c706-149">deviceDisplayName</span></span>|<span data-ttu-id="2c706-150">String</span><span class="sxs-lookup"><span data-stu-id="2c706-150">String</span></span>|<span data-ttu-id="2c706-151">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="2c706-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2c706-152">userName</span><span class="sxs-lookup"><span data-stu-id="2c706-152">userName</span></span>|<span data-ttu-id="2c706-153">String</span><span class="sxs-lookup"><span data-stu-id="2c706-153">String</span></span>|<span data-ttu-id="2c706-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="2c706-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="2c706-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2c706-155">deviceModel</span></span>|<span data-ttu-id="2c706-156">String</span><span class="sxs-lookup"><span data-stu-id="2c706-156">String</span></span>|<span data-ttu-id="2c706-157">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="2c706-157">The device model that is being reported</span></span>|
|<span data-ttu-id="2c706-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="2c706-158">platform</span></span>|<span data-ttu-id="2c706-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2c706-159">Int32</span></span>|<span data-ttu-id="2c706-160">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="2c706-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2c706-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2c706-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2c706-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c706-162">DateTimeOffset</span></span>|<span data-ttu-id="2c706-163">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="2c706-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2c706-164">status</span><span class="sxs-lookup"><span data-stu-id="2c706-164">status</span></span>|[<span data-ttu-id="2c706-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2c706-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2c706-166">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="2c706-166">Compliance status of the policy report.</span></span> <span data-ttu-id="2c706-167">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2c706-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2c706-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c706-168">lastReportedDateTime</span></span>|<span data-ttu-id="2c706-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c706-169">DateTimeOffset</span></span>|<span data-ttu-id="2c706-170">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="2c706-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2c706-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2c706-171">userPrincipalName</span></span>|<span data-ttu-id="2c706-172">String</span><span class="sxs-lookup"><span data-stu-id="2c706-172">String</span></span>|<span data-ttu-id="2c706-173">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="2c706-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2c706-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c706-174">Response</span></span>
<span data-ttu-id="2c706-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2c706-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c706-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2c706-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="2c706-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c706-177">Request</span></span>
<span data-ttu-id="2c706-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2c706-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 510

{
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

### <a name="response"></a><span data-ttu-id="2c706-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c706-179">Response</span></span>
<span data-ttu-id="2c706-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c706-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





