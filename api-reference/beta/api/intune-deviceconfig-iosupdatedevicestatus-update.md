---
title: iosUpdateDeviceStatus aktualisieren
description: Aktualisieren der Eigenschaften eines iosUpdateDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5917e256357305b1967789507dbcfaf69fd98a0c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162804"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="e6e84-103">iosUpdateDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e6e84-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="e6e84-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6e84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6e84-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e6e84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6e84-106">Aktualisieren der Eigenschaften eines [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6e84-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6e84-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e6e84-107">Prerequisites</span></span>
<span data-ttu-id="e6e84-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6e84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6e84-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6e84-110">Permission type</span></span>|<span data-ttu-id="e6e84-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6e84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6e84-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6e84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6e84-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6e84-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6e84-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6e84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6e84-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6e84-115">Not supported.</span></span>|
|<span data-ttu-id="e6e84-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6e84-116">Application</span></span>|<span data-ttu-id="e6e84-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6e84-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6e84-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6e84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e6e84-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6e84-119">Request headers</span></span>
|<span data-ttu-id="e6e84-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e6e84-120">Header</span></span>|<span data-ttu-id="e6e84-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e6e84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6e84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6e84-122">Authorization</span></span>|<span data-ttu-id="e6e84-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e6e84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6e84-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e6e84-124">Accept</span></span>|<span data-ttu-id="e6e84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6e84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6e84-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6e84-126">Request body</span></span>
<span data-ttu-id="e6e84-127">Geben Sie im Anforderungstext eine JSON Darstellung für das Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="e6e84-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="e6e84-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e6e84-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="e6e84-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6e84-129">Property</span></span>|<span data-ttu-id="e6e84-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e6e84-130">Type</span></span>|<span data-ttu-id="e6e84-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6e84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6e84-132">id</span><span class="sxs-lookup"><span data-stu-id="e6e84-132">id</span></span>|<span data-ttu-id="e6e84-133">String</span><span class="sxs-lookup"><span data-stu-id="e6e84-133">String</span></span>|<span data-ttu-id="e6e84-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e6e84-134">Key of the entity.</span></span>|
|<span data-ttu-id="e6e84-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="e6e84-135">installStatus</span></span>|[<span data-ttu-id="e6e84-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e6e84-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="e6e84-137">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="e6e84-137">The installation status of the policy report.</span></span> <span data-ttu-id="e6e84-138">Mögliche Werte sind: `success`, `available`, `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed`,,,, `notSupportedOperation`,,,,,,,,,, `sharedDeviceUserLoggedInError` `downloadInsufficientSpace` `downloadInsufficientPower`</span><span class="sxs-lookup"><span data-stu-id="e6e84-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="e6e84-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="e6e84-139">osVersion</span></span>|<span data-ttu-id="e6e84-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6e84-140">String</span></span>|<span data-ttu-id="e6e84-141">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="e6e84-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="e6e84-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6e84-142">deviceId</span></span>|<span data-ttu-id="e6e84-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6e84-143">String</span></span>|<span data-ttu-id="e6e84-144">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="e6e84-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="e6e84-145">userId</span><span class="sxs-lookup"><span data-stu-id="e6e84-145">userId</span></span>|<span data-ttu-id="e6e84-146">String</span><span class="sxs-lookup"><span data-stu-id="e6e84-146">String</span></span>|<span data-ttu-id="e6e84-147">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="e6e84-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="e6e84-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6e84-148">deviceDisplayName</span></span>|<span data-ttu-id="e6e84-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6e84-149">String</span></span>|<span data-ttu-id="e6e84-150">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="e6e84-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="e6e84-151">userName</span><span class="sxs-lookup"><span data-stu-id="e6e84-151">userName</span></span>|<span data-ttu-id="e6e84-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6e84-152">String</span></span>|<span data-ttu-id="e6e84-153">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="e6e84-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="e6e84-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e6e84-154">deviceModel</span></span>|<span data-ttu-id="e6e84-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6e84-155">String</span></span>|<span data-ttu-id="e6e84-156">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="e6e84-156">The device model that is being reported</span></span>|
|<span data-ttu-id="e6e84-157">Plattform</span><span class="sxs-lookup"><span data-stu-id="e6e84-157">platform</span></span>|<span data-ttu-id="e6e84-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e6e84-158">Int32</span></span>|<span data-ttu-id="e6e84-159">Plattform des gemeldeten Geräts</span><span class="sxs-lookup"><span data-stu-id="e6e84-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="e6e84-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e6e84-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e6e84-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6e84-161">DateTimeOffset</span></span>|<span data-ttu-id="e6e84-162">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="e6e84-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="e6e84-163">status</span><span class="sxs-lookup"><span data-stu-id="e6e84-163">status</span></span>|[<span data-ttu-id="e6e84-164">Wurde</span><span class="sxs-lookup"><span data-stu-id="e6e84-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e6e84-165">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="e6e84-165">Compliance status of the policy report.</span></span> <span data-ttu-id="e6e84-166">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e6e84-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e6e84-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6e84-167">lastReportedDateTime</span></span>|<span data-ttu-id="e6e84-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6e84-168">DateTimeOffset</span></span>|<span data-ttu-id="e6e84-169">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="e6e84-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="e6e84-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6e84-170">userPrincipalName</span></span>|<span data-ttu-id="e6e84-171">String</span><span class="sxs-lookup"><span data-stu-id="e6e84-171">String</span></span>|<span data-ttu-id="e6e84-172">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="e6e84-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="e6e84-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6e84-173">Response</span></span>
<span data-ttu-id="e6e84-174">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e6e84-174">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6e84-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6e84-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6e84-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6e84-176">Request</span></span>
<span data-ttu-id="e6e84-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6e84-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="e6e84-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6e84-178">Response</span></span>
<span data-ttu-id="e6e84-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6e84-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




