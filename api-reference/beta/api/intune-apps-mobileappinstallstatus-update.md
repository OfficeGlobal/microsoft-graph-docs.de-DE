---
title: MobileAppInstallStatus aktualisieren
description: Aktualisieren der Eigenschaften eines mobileAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1efc73e81894cb6fdd7d352cb067cf164f8bb33c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165744"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="f96fa-103">MobileAppInstallStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f96fa-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="f96fa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f96fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f96fa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f96fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f96fa-106">Aktualisieren der Eigenschaften eines [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f96fa-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f96fa-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f96fa-107">Prerequisites</span></span>
<span data-ttu-id="f96fa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f96fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f96fa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f96fa-110">Permission type</span></span>|<span data-ttu-id="f96fa-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f96fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f96fa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f96fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f96fa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f96fa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f96fa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f96fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f96fa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f96fa-115">Not supported.</span></span>|
|<span data-ttu-id="f96fa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f96fa-116">Application</span></span>|<span data-ttu-id="f96fa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f96fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f96fa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f96fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f96fa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f96fa-119">Request headers</span></span>
|<span data-ttu-id="f96fa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f96fa-120">Header</span></span>|<span data-ttu-id="f96fa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f96fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f96fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f96fa-122">Authorization</span></span>|<span data-ttu-id="f96fa-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f96fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f96fa-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f96fa-124">Accept</span></span>|<span data-ttu-id="f96fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f96fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f96fa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f96fa-126">Request body</span></span>
<span data-ttu-id="f96fa-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f96fa-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="f96fa-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f96fa-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="f96fa-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f96fa-129">Property</span></span>|<span data-ttu-id="f96fa-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f96fa-130">Type</span></span>|<span data-ttu-id="f96fa-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f96fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f96fa-132">id</span><span class="sxs-lookup"><span data-stu-id="f96fa-132">id</span></span>|<span data-ttu-id="f96fa-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f96fa-133">String</span></span>|<span data-ttu-id="f96fa-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f96fa-134">Key of the entity.</span></span>|
|<span data-ttu-id="f96fa-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="f96fa-135">deviceName</span></span>|<span data-ttu-id="f96fa-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f96fa-136">String</span></span>|<span data-ttu-id="f96fa-137">Gerätename</span><span class="sxs-lookup"><span data-stu-id="f96fa-137">Device name</span></span>|
|<span data-ttu-id="f96fa-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="f96fa-138">deviceId</span></span>|<span data-ttu-id="f96fa-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f96fa-139">String</span></span>|<span data-ttu-id="f96fa-140">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="f96fa-140">Device ID</span></span>|
|<span data-ttu-id="f96fa-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f96fa-141">lastSyncDateTime</span></span>|<span data-ttu-id="f96fa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f96fa-142">DateTimeOffset</span></span>|<span data-ttu-id="f96fa-143">Datum der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="f96fa-143">Last sync date time</span></span>|
|<span data-ttu-id="f96fa-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="f96fa-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="f96fa-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="f96fa-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f96fa-146">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="f96fa-146">The install state of the app.</span></span> <span data-ttu-id="f96fa-147">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f96fa-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f96fa-148">installState</span><span class="sxs-lookup"><span data-stu-id="f96fa-148">installState</span></span>|[<span data-ttu-id="f96fa-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="f96fa-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f96fa-150">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="f96fa-150">The install state of the app.</span></span> <span data-ttu-id="f96fa-151">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f96fa-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f96fa-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="f96fa-152">installStateDetail</span></span>|[<span data-ttu-id="f96fa-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="f96fa-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="f96fa-154">Die Installationsstatus Details der app.</span><span class="sxs-lookup"><span data-stu-id="f96fa-154">The install state detail of the app.</span></span> <span data-ttu-id="f96fa-155">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f96fa-155">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="f96fa-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="f96fa-156">errorCode</span></span>|<span data-ttu-id="f96fa-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f96fa-157">Int32</span></span>|<span data-ttu-id="f96fa-158">Der Fehlercode für Installations-oder Deinstallationsfehler.</span><span class="sxs-lookup"><span data-stu-id="f96fa-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="f96fa-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="f96fa-159">osVersion</span></span>|<span data-ttu-id="f96fa-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f96fa-160">String</span></span>|<span data-ttu-id="f96fa-161">Betriebssystem Version</span><span class="sxs-lookup"><span data-stu-id="f96fa-161">OS Version</span></span>|
|<span data-ttu-id="f96fa-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="f96fa-162">osDescription</span></span>|<span data-ttu-id="f96fa-163">String</span><span class="sxs-lookup"><span data-stu-id="f96fa-163">String</span></span>|<span data-ttu-id="f96fa-164">Betriebssystem Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f96fa-164">OS Description</span></span>|
|<span data-ttu-id="f96fa-165">userName</span><span class="sxs-lookup"><span data-stu-id="f96fa-165">userName</span></span>|<span data-ttu-id="f96fa-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f96fa-166">String</span></span>|<span data-ttu-id="f96fa-167">Geräte Benutzer Name</span><span class="sxs-lookup"><span data-stu-id="f96fa-167">Device User Name</span></span>|
|<span data-ttu-id="f96fa-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f96fa-168">userPrincipalName</span></span>|<span data-ttu-id="f96fa-169">String</span><span class="sxs-lookup"><span data-stu-id="f96fa-169">String</span></span>|<span data-ttu-id="f96fa-170">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="f96fa-170">User Principal Name</span></span>|
|<span data-ttu-id="f96fa-171">Display Version</span><span class="sxs-lookup"><span data-stu-id="f96fa-171">displayVersion</span></span>|<span data-ttu-id="f96fa-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f96fa-172">String</span></span>|<span data-ttu-id="f96fa-173">Lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f96fa-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="f96fa-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="f96fa-174">Response</span></span>
<span data-ttu-id="f96fa-175">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f96fa-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f96fa-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f96fa-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f96fa-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f96fa-177">Request</span></span>
<span data-ttu-id="f96fa-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f96fa-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f96fa-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="f96fa-179">Response</span></span>
<span data-ttu-id="f96fa-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f96fa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




