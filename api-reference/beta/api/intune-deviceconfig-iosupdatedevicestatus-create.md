---
title: Erstellen von „iosUpdateDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs iosUpdateDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: edfc360460b60fa91bf304f4dbf492d91c9ce7f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400508"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="ebad1-103">Erstellen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="ebad1-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="ebad1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ebad1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ebad1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebad1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebad1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebad1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebad1-107">Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ebad1-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebad1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ebad1-108">Prerequisites</span></span>
<span data-ttu-id="ebad1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebad1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ebad1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebad1-111">Permission type</span></span>|<span data-ttu-id="ebad1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebad1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebad1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebad1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebad1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebad1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebad1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebad1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebad1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebad1-116">Not supported.</span></span>|
|<span data-ttu-id="ebad1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebad1-117">Application</span></span>|<span data-ttu-id="ebad1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebad1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebad1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebad1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ebad1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebad1-120">Request headers</span></span>
|<span data-ttu-id="ebad1-121">Header</span><span class="sxs-lookup"><span data-stu-id="ebad1-121">Header</span></span>|<span data-ttu-id="ebad1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ebad1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebad1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ebad1-123">Authorization</span></span>|<span data-ttu-id="ebad1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ebad1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebad1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ebad1-125">Accept</span></span>|<span data-ttu-id="ebad1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebad1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebad1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebad1-127">Request body</span></span>
<span data-ttu-id="ebad1-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="ebad1-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="ebad1-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ebad1-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="ebad1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebad1-130">Property</span></span>|<span data-ttu-id="ebad1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ebad1-131">Type</span></span>|<span data-ttu-id="ebad1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebad1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebad1-133">id</span><span class="sxs-lookup"><span data-stu-id="ebad1-133">id</span></span>|<span data-ttu-id="ebad1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-134">String</span></span>|<span data-ttu-id="ebad1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ebad1-135">Key of the entity.</span></span>|
|<span data-ttu-id="ebad1-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="ebad1-136">installStatus</span></span>|[<span data-ttu-id="ebad1-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ebad1-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="ebad1-138">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="ebad1-138">The installation status of the policy report.</span></span> <span data-ttu-id="ebad1-139">Mögliche Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="ebad1-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="ebad1-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="ebad1-140">osVersion</span></span>|<span data-ttu-id="ebad1-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-141">String</span></span>|<span data-ttu-id="ebad1-142">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="ebad1-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="ebad1-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="ebad1-143">deviceId</span></span>|<span data-ttu-id="ebad1-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-144">String</span></span>|<span data-ttu-id="ebad1-145">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="ebad1-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="ebad1-146">userId</span><span class="sxs-lookup"><span data-stu-id="ebad1-146">userId</span></span>|<span data-ttu-id="ebad1-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-147">String</span></span>|<span data-ttu-id="ebad1-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="ebad1-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="ebad1-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ebad1-149">deviceDisplayName</span></span>|<span data-ttu-id="ebad1-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-150">String</span></span>|<span data-ttu-id="ebad1-151">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="ebad1-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ebad1-152">userName</span><span class="sxs-lookup"><span data-stu-id="ebad1-152">userName</span></span>|<span data-ttu-id="ebad1-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-153">String</span></span>|<span data-ttu-id="ebad1-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="ebad1-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="ebad1-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ebad1-155">deviceModel</span></span>|<span data-ttu-id="ebad1-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-156">String</span></span>|<span data-ttu-id="ebad1-157">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="ebad1-157">The device model that is being reported</span></span>|
|<span data-ttu-id="ebad1-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="ebad1-158">platform</span></span>|<span data-ttu-id="ebad1-159">Int32</span><span class="sxs-lookup"><span data-stu-id="ebad1-159">Int32</span></span>|<span data-ttu-id="ebad1-160">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="ebad1-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="ebad1-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ebad1-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ebad1-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebad1-162">DateTimeOffset</span></span>|<span data-ttu-id="ebad1-163">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="ebad1-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ebad1-164">status</span><span class="sxs-lookup"><span data-stu-id="ebad1-164">status</span></span>|[<span data-ttu-id="ebad1-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ebad1-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ebad1-166">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="ebad1-166">Compliance status of the policy report.</span></span> <span data-ttu-id="ebad1-167">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ebad1-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ebad1-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebad1-168">lastReportedDateTime</span></span>|<span data-ttu-id="ebad1-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebad1-169">DateTimeOffset</span></span>|<span data-ttu-id="ebad1-170">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="ebad1-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ebad1-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ebad1-171">userPrincipalName</span></span>|<span data-ttu-id="ebad1-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebad1-172">String</span></span>|<span data-ttu-id="ebad1-173">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="ebad1-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ebad1-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebad1-174">Response</span></span>
<span data-ttu-id="ebad1-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ebad1-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebad1-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebad1-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebad1-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebad1-177">Request</span></span>
<span data-ttu-id="ebad1-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebad1-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebad1-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebad1-179">Response</span></span>
<span data-ttu-id="ebad1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebad1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




