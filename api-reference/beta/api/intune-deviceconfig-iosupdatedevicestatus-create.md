---
title: Erstellen von „iosUpdateDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d83f9d72c32a6d7cf5391b24fe58d67f2b6b73dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162447"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="952d5-103">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="952d5-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="952d5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="952d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="952d5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="952d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="952d5-106">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="952d5-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="952d5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="952d5-107">Prerequisites</span></span>
<span data-ttu-id="952d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="952d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="952d5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="952d5-110">Permission type</span></span>|<span data-ttu-id="952d5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="952d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="952d5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="952d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="952d5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="952d5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="952d5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="952d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="952d5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="952d5-115">Not supported.</span></span>|
|<span data-ttu-id="952d5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="952d5-116">Application</span></span>|<span data-ttu-id="952d5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="952d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="952d5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="952d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="952d5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="952d5-119">Request headers</span></span>
|<span data-ttu-id="952d5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="952d5-120">Header</span></span>|<span data-ttu-id="952d5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="952d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="952d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="952d5-122">Authorization</span></span>|<span data-ttu-id="952d5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="952d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="952d5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="952d5-124">Accept</span></span>|<span data-ttu-id="952d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="952d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="952d5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="952d5-126">Request body</span></span>
<span data-ttu-id="952d5-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="952d5-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="952d5-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="952d5-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="952d5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="952d5-129">Property</span></span>|<span data-ttu-id="952d5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="952d5-130">Type</span></span>|<span data-ttu-id="952d5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="952d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="952d5-132">id</span><span class="sxs-lookup"><span data-stu-id="952d5-132">id</span></span>|<span data-ttu-id="952d5-133">String</span><span class="sxs-lookup"><span data-stu-id="952d5-133">String</span></span>|<span data-ttu-id="952d5-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="952d5-134">Key of the entity.</span></span>|
|<span data-ttu-id="952d5-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="952d5-135">installStatus</span></span>|[<span data-ttu-id="952d5-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="952d5-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="952d5-137">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="952d5-137">The installation status of the policy report.</span></span> <span data-ttu-id="952d5-138">Mögliche Werte sind: `success`, `available`, `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed`,,,, `notSupportedOperation`,,,,,,,,,, `sharedDeviceUserLoggedInError` `downloadInsufficientSpace` `downloadInsufficientPower`</span><span class="sxs-lookup"><span data-stu-id="952d5-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="952d5-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="952d5-139">osVersion</span></span>|<span data-ttu-id="952d5-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="952d5-140">String</span></span>|<span data-ttu-id="952d5-141">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="952d5-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="952d5-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="952d5-142">deviceId</span></span>|<span data-ttu-id="952d5-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="952d5-143">String</span></span>|<span data-ttu-id="952d5-144">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="952d5-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="952d5-145">userId</span><span class="sxs-lookup"><span data-stu-id="952d5-145">userId</span></span>|<span data-ttu-id="952d5-146">String</span><span class="sxs-lookup"><span data-stu-id="952d5-146">String</span></span>|<span data-ttu-id="952d5-147">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="952d5-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="952d5-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="952d5-148">deviceDisplayName</span></span>|<span data-ttu-id="952d5-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="952d5-149">String</span></span>|<span data-ttu-id="952d5-150">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="952d5-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="952d5-151">userName</span><span class="sxs-lookup"><span data-stu-id="952d5-151">userName</span></span>|<span data-ttu-id="952d5-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="952d5-152">String</span></span>|<span data-ttu-id="952d5-153">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="952d5-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="952d5-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="952d5-154">deviceModel</span></span>|<span data-ttu-id="952d5-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="952d5-155">String</span></span>|<span data-ttu-id="952d5-156">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="952d5-156">The device model that is being reported</span></span>|
|<span data-ttu-id="952d5-157">Plattform</span><span class="sxs-lookup"><span data-stu-id="952d5-157">platform</span></span>|<span data-ttu-id="952d5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="952d5-158">Int32</span></span>|<span data-ttu-id="952d5-159">Plattform des gemeldeten Geräts</span><span class="sxs-lookup"><span data-stu-id="952d5-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="952d5-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="952d5-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="952d5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952d5-161">DateTimeOffset</span></span>|<span data-ttu-id="952d5-162">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="952d5-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="952d5-163">status</span><span class="sxs-lookup"><span data-stu-id="952d5-163">status</span></span>|[<span data-ttu-id="952d5-164">Wurde</span><span class="sxs-lookup"><span data-stu-id="952d5-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="952d5-165">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="952d5-165">Compliance status of the policy report.</span></span> <span data-ttu-id="952d5-166">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="952d5-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="952d5-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="952d5-167">lastReportedDateTime</span></span>|<span data-ttu-id="952d5-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952d5-168">DateTimeOffset</span></span>|<span data-ttu-id="952d5-169">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="952d5-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="952d5-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="952d5-170">userPrincipalName</span></span>|<span data-ttu-id="952d5-171">String</span><span class="sxs-lookup"><span data-stu-id="952d5-171">String</span></span>|<span data-ttu-id="952d5-172">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="952d5-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="952d5-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="952d5-173">Response</span></span>
<span data-ttu-id="952d5-174">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="952d5-174">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="952d5-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="952d5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="952d5-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="952d5-176">Request</span></span>
<span data-ttu-id="952d5-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="952d5-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="952d5-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="952d5-178">Response</span></span>
<span data-ttu-id="952d5-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="952d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




