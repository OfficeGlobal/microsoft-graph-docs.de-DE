---
title: iosUpdateDeviceStatus aktualisieren
description: Aktualisieren der Eigenschaften eines iosUpdateDeviceStatus-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e501171c66b2bfc18f82376d382f026f39291e5a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419814"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="e1a0c-103">iosUpdateDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e1a0c-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="e1a0c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1a0c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1a0c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a0c-107">Aktualisieren der Eigenschaften eines [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1a0c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1a0c-108">Prerequisites</span></span>
<span data-ttu-id="e1a0c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1a0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1a0c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1a0c-111">Permission type</span></span>|<span data-ttu-id="e1a0c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1a0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1a0c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1a0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1a0c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a0c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1a0c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1a0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1a0c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1a0c-116">Not supported.</span></span>|
|<span data-ttu-id="e1a0c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1a0c-117">Application</span></span>|<span data-ttu-id="e1a0c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1a0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1a0c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1a0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e1a0c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1a0c-120">Request headers</span></span>
|<span data-ttu-id="e1a0c-121">Header</span><span class="sxs-lookup"><span data-stu-id="e1a0c-121">Header</span></span>|<span data-ttu-id="e1a0c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e1a0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1a0c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e1a0c-123">Authorization</span></span>|<span data-ttu-id="e1a0c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1a0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1a0c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1a0c-125">Accept</span></span>|<span data-ttu-id="e1a0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1a0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1a0c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1a0c-127">Request body</span></span>
<span data-ttu-id="e1a0c-128">Geben Sie im Anforderungstext eine JSON Darstellung für das Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="e1a0c-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="e1a0c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1a0c-130">Property</span></span>|<span data-ttu-id="e1a0c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e1a0c-131">Type</span></span>|<span data-ttu-id="e1a0c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1a0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a0c-133">id</span><span class="sxs-lookup"><span data-stu-id="e1a0c-133">id</span></span>|<span data-ttu-id="e1a0c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-134">String</span></span>|<span data-ttu-id="e1a0c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e1a0c-135">Key of the entity.</span></span>|
|<span data-ttu-id="e1a0c-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="e1a0c-136">installStatus</span></span>|[<span data-ttu-id="e1a0c-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1a0c-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="e1a0c-138">Installationsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-138">The installation status of the policy report.</span></span> <span data-ttu-id="e1a0c-139">Mögliche Werte sind: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="e1a0c-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="e1a0c-140">osVersion</span></span>|<span data-ttu-id="e1a0c-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-141">String</span></span>|<span data-ttu-id="e1a0c-142">Gemeldete Geräteversion</span><span class="sxs-lookup"><span data-stu-id="e1a0c-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="e1a0c-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="e1a0c-143">deviceId</span></span>|<span data-ttu-id="e1a0c-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-144">String</span></span>|<span data-ttu-id="e1a0c-145">Gemeldete Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="e1a0c-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="e1a0c-146">userId</span><span class="sxs-lookup"><span data-stu-id="e1a0c-146">userId</span></span>|<span data-ttu-id="e1a0c-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-147">String</span></span>|<span data-ttu-id="e1a0c-148">Gemeldete Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="e1a0c-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="e1a0c-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1a0c-149">deviceDisplayName</span></span>|<span data-ttu-id="e1a0c-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-150">String</span></span>|<span data-ttu-id="e1a0c-151">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="e1a0c-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="e1a0c-152">userName</span><span class="sxs-lookup"><span data-stu-id="e1a0c-152">userName</span></span>|<span data-ttu-id="e1a0c-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-153">String</span></span>|<span data-ttu-id="e1a0c-154">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="e1a0c-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="e1a0c-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e1a0c-155">deviceModel</span></span>|<span data-ttu-id="e1a0c-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-156">String</span></span>|<span data-ttu-id="e1a0c-157">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="e1a0c-157">The device model that is being reported</span></span>|
|<span data-ttu-id="e1a0c-158">Plattform</span><span class="sxs-lookup"><span data-stu-id="e1a0c-158">platform</span></span>|<span data-ttu-id="e1a0c-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e1a0c-159">Int32</span></span>|<span data-ttu-id="e1a0c-160">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="e1a0c-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="e1a0c-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e1a0c-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e1a0c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1a0c-162">DateTimeOffset</span></span>|<span data-ttu-id="e1a0c-163">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="e1a0c-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="e1a0c-164">status</span><span class="sxs-lookup"><span data-stu-id="e1a0c-164">status</span></span>|[<span data-ttu-id="e1a0c-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e1a0c-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e1a0c-166">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-166">Compliance status of the policy report.</span></span> <span data-ttu-id="e1a0c-167">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e1a0c-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1a0c-168">lastReportedDateTime</span></span>|<span data-ttu-id="e1a0c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1a0c-169">DateTimeOffset</span></span>|<span data-ttu-id="e1a0c-170">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="e1a0c-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="e1a0c-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1a0c-171">userPrincipalName</span></span>|<span data-ttu-id="e1a0c-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a0c-172">String</span></span>|<span data-ttu-id="e1a0c-173">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="e1a0c-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="e1a0c-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1a0c-174">Response</span></span>
<span data-ttu-id="e1a0c-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1a0c-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1a0c-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1a0c-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1a0c-177">Request</span></span>
<span data-ttu-id="e1a0c-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1a0c-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1a0c-179">Response</span></span>
<span data-ttu-id="e1a0c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1a0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




