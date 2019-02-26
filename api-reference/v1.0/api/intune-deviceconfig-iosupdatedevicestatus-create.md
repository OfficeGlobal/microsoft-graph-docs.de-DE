---
title: Erstellen von „iosUpdateDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc97746eb2f22447f0d77cfd873cd2156ef15c73
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262622"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="a7eda-103">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="a7eda-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="a7eda-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a7eda-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7eda-105">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a7eda-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7eda-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a7eda-106">Prerequisites</span></span>
<span data-ttu-id="a7eda-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7eda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7eda-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7eda-109">Permission type</span></span>|<span data-ttu-id="a7eda-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7eda-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7eda-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7eda-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7eda-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7eda-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7eda-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7eda-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7eda-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7eda-114">Not supported.</span></span>|
|<span data-ttu-id="a7eda-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7eda-115">Application</span></span>|<span data-ttu-id="a7eda-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7eda-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7eda-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7eda-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a7eda-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7eda-118">Request headers</span></span>
|<span data-ttu-id="a7eda-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a7eda-119">Header</span></span>|<span data-ttu-id="a7eda-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a7eda-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7eda-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7eda-121">Authorization</span></span>|<span data-ttu-id="a7eda-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a7eda-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7eda-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a7eda-123">Accept</span></span>|<span data-ttu-id="a7eda-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7eda-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7eda-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7eda-125">Request body</span></span>
<span data-ttu-id="a7eda-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="a7eda-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="a7eda-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a7eda-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="a7eda-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a7eda-128">Property</span></span>|<span data-ttu-id="a7eda-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a7eda-129">Type</span></span>|<span data-ttu-id="a7eda-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7eda-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7eda-131">id</span><span class="sxs-lookup"><span data-stu-id="a7eda-131">id</span></span>|<span data-ttu-id="a7eda-132">String</span><span class="sxs-lookup"><span data-stu-id="a7eda-132">String</span></span>|<span data-ttu-id="a7eda-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a7eda-133">Key of the entity.</span></span>|
|<span data-ttu-id="a7eda-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="a7eda-134">installStatus</span></span>|[<span data-ttu-id="a7eda-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="a7eda-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="a7eda-136">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="a7eda-136">The installation status of the policy report.</span></span> <span data-ttu-id="a7eda-137">Mögliche Werte sind: `success`, `available`, `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed`,,,, `notSupportedOperation`,,,,,,,,,, `sharedDeviceUserLoggedInError` `downloadInsufficientSpace` `downloadInsufficientPower`</span><span class="sxs-lookup"><span data-stu-id="a7eda-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="a7eda-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="a7eda-138">osVersion</span></span>|<span data-ttu-id="a7eda-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7eda-139">String</span></span>|<span data-ttu-id="a7eda-140">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="a7eda-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="a7eda-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="a7eda-141">deviceId</span></span>|<span data-ttu-id="a7eda-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7eda-142">String</span></span>|<span data-ttu-id="a7eda-143">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="a7eda-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="a7eda-144">userId</span><span class="sxs-lookup"><span data-stu-id="a7eda-144">userId</span></span>|<span data-ttu-id="a7eda-145">String</span><span class="sxs-lookup"><span data-stu-id="a7eda-145">String</span></span>|<span data-ttu-id="a7eda-146">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="a7eda-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="a7eda-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7eda-147">deviceDisplayName</span></span>|<span data-ttu-id="a7eda-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7eda-148">String</span></span>|<span data-ttu-id="a7eda-149">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="a7eda-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a7eda-150">userName</span><span class="sxs-lookup"><span data-stu-id="a7eda-150">userName</span></span>|<span data-ttu-id="a7eda-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7eda-151">String</span></span>|<span data-ttu-id="a7eda-152">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="a7eda-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="a7eda-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a7eda-153">deviceModel</span></span>|<span data-ttu-id="a7eda-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7eda-154">String</span></span>|<span data-ttu-id="a7eda-155">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="a7eda-155">The device model that is being reported</span></span>|
|<span data-ttu-id="a7eda-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a7eda-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a7eda-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7eda-157">DateTimeOffset</span></span>|<span data-ttu-id="a7eda-158">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="a7eda-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a7eda-159">status</span><span class="sxs-lookup"><span data-stu-id="a7eda-159">status</span></span>|[<span data-ttu-id="a7eda-160">Wurde</span><span class="sxs-lookup"><span data-stu-id="a7eda-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a7eda-161">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="a7eda-161">Compliance status of the policy report.</span></span> <span data-ttu-id="a7eda-162">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a7eda-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a7eda-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7eda-163">lastReportedDateTime</span></span>|<span data-ttu-id="a7eda-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7eda-164">DateTimeOffset</span></span>|<span data-ttu-id="a7eda-165">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="a7eda-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a7eda-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7eda-166">userPrincipalName</span></span>|<span data-ttu-id="a7eda-167">String</span><span class="sxs-lookup"><span data-stu-id="a7eda-167">String</span></span>|<span data-ttu-id="a7eda-168">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="a7eda-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a7eda-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7eda-169">Response</span></span>
<span data-ttu-id="a7eda-170">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a7eda-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7eda-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7eda-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7eda-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7eda-172">Request</span></span>
<span data-ttu-id="a7eda-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a7eda-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7eda-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7eda-174">Response</span></span>
<span data-ttu-id="a7eda-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7eda-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



