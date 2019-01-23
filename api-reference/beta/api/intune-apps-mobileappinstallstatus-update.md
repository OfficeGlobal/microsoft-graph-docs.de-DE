---
title: MobileAppInstallStatus aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MobileAppInstallStatus-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e28404181248cef1deae4bec2752de51f553373b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394544"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="98973-103">MobileAppInstallStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="98973-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="98973-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="98973-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98973-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98973-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98973-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="98973-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98973-107">Aktualisieren Sie die Eigenschaften eines [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="98973-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98973-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="98973-108">Prerequisites</span></span>
<span data-ttu-id="98973-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="98973-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98973-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98973-111">Permission type</span></span>|<span data-ttu-id="98973-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98973-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98973-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98973-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98973-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98973-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98973-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98973-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98973-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98973-116">Not supported.</span></span>|
|<span data-ttu-id="98973-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98973-117">Application</span></span>|<span data-ttu-id="98973-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98973-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98973-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98973-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="98973-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98973-120">Request headers</span></span>
|<span data-ttu-id="98973-121">Header</span><span class="sxs-lookup"><span data-stu-id="98973-121">Header</span></span>|<span data-ttu-id="98973-122">Wert</span><span class="sxs-lookup"><span data-stu-id="98973-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98973-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="98973-123">Authorization</span></span>|<span data-ttu-id="98973-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="98973-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98973-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="98973-125">Accept</span></span>|<span data-ttu-id="98973-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98973-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98973-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98973-127">Request body</span></span>
<span data-ttu-id="98973-128">Geben Sie im Textkörper Anforderung für das Objekt [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="98973-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="98973-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="98973-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="98973-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98973-130">Property</span></span>|<span data-ttu-id="98973-131">Typ</span><span class="sxs-lookup"><span data-stu-id="98973-131">Type</span></span>|<span data-ttu-id="98973-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98973-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98973-133">id</span><span class="sxs-lookup"><span data-stu-id="98973-133">id</span></span>|<span data-ttu-id="98973-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-134">String</span></span>|<span data-ttu-id="98973-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="98973-135">Key of the entity.</span></span>|
|<span data-ttu-id="98973-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="98973-136">deviceName</span></span>|<span data-ttu-id="98973-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-137">String</span></span>|<span data-ttu-id="98973-138">Gerätename</span><span class="sxs-lookup"><span data-stu-id="98973-138">Device name</span></span>|
|<span data-ttu-id="98973-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="98973-139">deviceId</span></span>|<span data-ttu-id="98973-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-140">String</span></span>|<span data-ttu-id="98973-141">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="98973-141">Device ID</span></span>|
|<span data-ttu-id="98973-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="98973-142">lastSyncDateTime</span></span>|<span data-ttu-id="98973-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98973-143">DateTimeOffset</span></span>|<span data-ttu-id="98973-144">Letzte Synchronisierung Datum-Zeit</span><span class="sxs-lookup"><span data-stu-id="98973-144">Last sync date time</span></span>|
|<span data-ttu-id="98973-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="98973-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="98973-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="98973-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="98973-147">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="98973-147">The install state of the app.</span></span> <span data-ttu-id="98973-148">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="98973-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="98973-149">installState</span><span class="sxs-lookup"><span data-stu-id="98973-149">installState</span></span>|[<span data-ttu-id="98973-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="98973-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="98973-151">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="98973-151">The install state of the app.</span></span> <span data-ttu-id="98973-152">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="98973-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="98973-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="98973-153">installStateDetail</span></span>|[<span data-ttu-id="98973-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="98973-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="98973-155">Die Details der Installation Zustand der app.</span><span class="sxs-lookup"><span data-stu-id="98973-155">The install state detail of the app.</span></span> <span data-ttu-id="98973-156">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="98973-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="98973-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="98973-157">errorCode</span></span>|<span data-ttu-id="98973-158">Int32</span><span class="sxs-lookup"><span data-stu-id="98973-158">Int32</span></span>|<span data-ttu-id="98973-159">Der Fehler im code für die Installation oder Deinstallieren von Fehlern.</span><span class="sxs-lookup"><span data-stu-id="98973-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="98973-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="98973-160">osVersion</span></span>|<span data-ttu-id="98973-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-161">String</span></span>|<span data-ttu-id="98973-162">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="98973-162">OS Version</span></span>|
|<span data-ttu-id="98973-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="98973-163">osDescription</span></span>|<span data-ttu-id="98973-164">String</span><span class="sxs-lookup"><span data-stu-id="98973-164">String</span></span>|<span data-ttu-id="98973-165">OS Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98973-165">OS Description</span></span>|
|<span data-ttu-id="98973-166">userName</span><span class="sxs-lookup"><span data-stu-id="98973-166">userName</span></span>|<span data-ttu-id="98973-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-167">String</span></span>|<span data-ttu-id="98973-168">Name des Aufnahmegeräts Benutzer</span><span class="sxs-lookup"><span data-stu-id="98973-168">Device User Name</span></span>|
|<span data-ttu-id="98973-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98973-169">userPrincipalName</span></span>|<span data-ttu-id="98973-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-170">String</span></span>|<span data-ttu-id="98973-171">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="98973-171">User Principal Name</span></span>|
|<span data-ttu-id="98973-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="98973-172">displayVersion</span></span>|<span data-ttu-id="98973-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="98973-173">String</span></span>|<span data-ttu-id="98973-174">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="98973-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="98973-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="98973-175">Response</span></span>
<span data-ttu-id="98973-176">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="98973-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98973-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98973-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="98973-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98973-178">Request</span></span>
<span data-ttu-id="98973-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="98973-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="98973-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="98973-180">Response</span></span>
<span data-ttu-id="98973-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98973-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```




