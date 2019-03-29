---
title: MobileAppInstallStatus aktualisieren
description: Aktualisieren der Eigenschaften eines mobileAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe31b91c8091d96b44ff0ea9435a3588068919de
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969477"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="ec18d-103">MobileAppInstallStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ec18d-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="ec18d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec18d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec18d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ec18d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec18d-106">Aktualisieren der Eigenschaften eines [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ec18d-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec18d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec18d-107">Prerequisites</span></span>
<span data-ttu-id="ec18d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec18d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec18d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec18d-110">Permission type</span></span>|<span data-ttu-id="ec18d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec18d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec18d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec18d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec18d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec18d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec18d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec18d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec18d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec18d-115">Not supported.</span></span>|
|<span data-ttu-id="ec18d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec18d-116">Application</span></span>|<span data-ttu-id="ec18d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec18d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec18d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec18d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ec18d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec18d-119">Request headers</span></span>
|<span data-ttu-id="ec18d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec18d-120">Header</span></span>|<span data-ttu-id="ec18d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ec18d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec18d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec18d-122">Authorization</span></span>|<span data-ttu-id="ec18d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec18d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec18d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ec18d-124">Accept</span></span>|<span data-ttu-id="ec18d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec18d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec18d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec18d-126">Request body</span></span>
<span data-ttu-id="ec18d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ec18d-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="ec18d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ec18d-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="ec18d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec18d-129">Property</span></span>|<span data-ttu-id="ec18d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ec18d-130">Type</span></span>|<span data-ttu-id="ec18d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec18d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec18d-132">id</span><span class="sxs-lookup"><span data-stu-id="ec18d-132">id</span></span>|<span data-ttu-id="ec18d-133">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-133">String</span></span>|<span data-ttu-id="ec18d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ec18d-134">Key of the entity.</span></span>|
|<span data-ttu-id="ec18d-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="ec18d-135">deviceName</span></span>|<span data-ttu-id="ec18d-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec18d-136">String</span></span>|<span data-ttu-id="ec18d-137">Gerätename</span><span class="sxs-lookup"><span data-stu-id="ec18d-137">Device name</span></span>|
|<span data-ttu-id="ec18d-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="ec18d-138">deviceId</span></span>|<span data-ttu-id="ec18d-139">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-139">String</span></span>|<span data-ttu-id="ec18d-140">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="ec18d-140">Device ID</span></span>|
|<span data-ttu-id="ec18d-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec18d-141">lastSyncDateTime</span></span>|<span data-ttu-id="ec18d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec18d-142">DateTimeOffset</span></span>|<span data-ttu-id="ec18d-143">Datum der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="ec18d-143">Last sync date time</span></span>|
|<span data-ttu-id="ec18d-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="ec18d-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="ec18d-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ec18d-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ec18d-146">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="ec18d-146">The install state of the app.</span></span> <span data-ttu-id="ec18d-147">Mögliche Werte: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ec18d-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ec18d-148">installState</span><span class="sxs-lookup"><span data-stu-id="ec18d-148">installState</span></span>|[<span data-ttu-id="ec18d-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ec18d-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ec18d-150">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="ec18d-150">The install state of the app.</span></span> <span data-ttu-id="ec18d-151">Mögliche Werte: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ec18d-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ec18d-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="ec18d-152">installStateDetail</span></span>|[<span data-ttu-id="ec18d-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="ec18d-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="ec18d-154">Die Installationsstatus Details der app.</span><span class="sxs-lookup"><span data-stu-id="ec18d-154">The install state detail of the app.</span></span> <span data-ttu-id="ec18d-155">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ec18d-155">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="ec18d-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="ec18d-156">errorCode</span></span>|<span data-ttu-id="ec18d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ec18d-157">Int32</span></span>|<span data-ttu-id="ec18d-158">Der Fehlercode für Installations-oder Deinstallationsfehler.</span><span class="sxs-lookup"><span data-stu-id="ec18d-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="ec18d-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="ec18d-159">osVersion</span></span>|<span data-ttu-id="ec18d-160">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-160">String</span></span>|<span data-ttu-id="ec18d-161">Betriebssystem Version</span><span class="sxs-lookup"><span data-stu-id="ec18d-161">OS Version</span></span>|
|<span data-ttu-id="ec18d-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="ec18d-162">osDescription</span></span>|<span data-ttu-id="ec18d-163">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-163">String</span></span>|<span data-ttu-id="ec18d-164">Betriebssystem Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec18d-164">OS Description</span></span>|
|<span data-ttu-id="ec18d-165">userName</span><span class="sxs-lookup"><span data-stu-id="ec18d-165">userName</span></span>|<span data-ttu-id="ec18d-166">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-166">String</span></span>|<span data-ttu-id="ec18d-167">Geräte Benutzer Name</span><span class="sxs-lookup"><span data-stu-id="ec18d-167">Device User Name</span></span>|
|<span data-ttu-id="ec18d-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec18d-168">userPrincipalName</span></span>|<span data-ttu-id="ec18d-169">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-169">String</span></span>|<span data-ttu-id="ec18d-170">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="ec18d-170">User Principal Name</span></span>|
|<span data-ttu-id="ec18d-171">Display Version</span><span class="sxs-lookup"><span data-stu-id="ec18d-171">displayVersion</span></span>|<span data-ttu-id="ec18d-172">String</span><span class="sxs-lookup"><span data-stu-id="ec18d-172">String</span></span>|<span data-ttu-id="ec18d-173">Lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec18d-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="ec18d-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec18d-174">Response</span></span>
<span data-ttu-id="ec18d-175">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ec18d-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec18d-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec18d-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec18d-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec18d-177">Request</span></span>
<span data-ttu-id="ec18d-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec18d-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec18d-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec18d-179">Response</span></span>
<span data-ttu-id="ec18d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec18d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




