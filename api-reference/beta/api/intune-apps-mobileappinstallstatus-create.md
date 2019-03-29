---
title: MobileAppInstallStatus erstellen
description: Erstellen eines neuen mobileAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13fae27ccc022ce8795d787dbd86923d71e2ab24
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969890"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="4d212-103">MobileAppInstallStatus erstellen</span><span class="sxs-lookup"><span data-stu-id="4d212-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="4d212-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d212-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d212-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4d212-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d212-106">Erstellen eines neuen [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d212-106">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d212-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d212-107">Prerequisites</span></span>
<span data-ttu-id="4d212-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d212-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d212-110">Permission type</span></span>|<span data-ttu-id="4d212-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d212-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d212-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d212-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d212-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d212-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d212-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d212-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d212-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d212-115">Not supported.</span></span>|
|<span data-ttu-id="4d212-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d212-116">Application</span></span>|<span data-ttu-id="4d212-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d212-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d212-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d212-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4d212-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d212-119">Request headers</span></span>
|<span data-ttu-id="4d212-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4d212-120">Header</span></span>|<span data-ttu-id="4d212-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4d212-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d212-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d212-122">Authorization</span></span>|<span data-ttu-id="4d212-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d212-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d212-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d212-124">Accept</span></span>|<span data-ttu-id="4d212-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d212-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d212-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d212-126">Request body</span></span>
<span data-ttu-id="4d212-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das mobileAppInstallStatus-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4d212-127">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="4d212-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der mobileAppInstallStatus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4d212-128">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="4d212-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d212-129">Property</span></span>|<span data-ttu-id="4d212-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4d212-130">Type</span></span>|<span data-ttu-id="4d212-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d212-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d212-132">id</span><span class="sxs-lookup"><span data-stu-id="4d212-132">id</span></span>|<span data-ttu-id="4d212-133">String</span><span class="sxs-lookup"><span data-stu-id="4d212-133">String</span></span>|<span data-ttu-id="4d212-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4d212-134">Key of the entity.</span></span>|
|<span data-ttu-id="4d212-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="4d212-135">deviceName</span></span>|<span data-ttu-id="4d212-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d212-136">String</span></span>|<span data-ttu-id="4d212-137">Gerätename</span><span class="sxs-lookup"><span data-stu-id="4d212-137">Device name</span></span>|
|<span data-ttu-id="4d212-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="4d212-138">deviceId</span></span>|<span data-ttu-id="4d212-139">String</span><span class="sxs-lookup"><span data-stu-id="4d212-139">String</span></span>|<span data-ttu-id="4d212-140">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="4d212-140">Device ID</span></span>|
|<span data-ttu-id="4d212-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4d212-141">lastSyncDateTime</span></span>|<span data-ttu-id="4d212-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d212-142">DateTimeOffset</span></span>|<span data-ttu-id="4d212-143">Datum der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="4d212-143">Last sync date time</span></span>|
|<span data-ttu-id="4d212-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="4d212-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="4d212-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="4d212-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="4d212-146">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="4d212-146">The install state of the app.</span></span> <span data-ttu-id="4d212-147">Mögliche Werte: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="4d212-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="4d212-148">installState</span><span class="sxs-lookup"><span data-stu-id="4d212-148">installState</span></span>|[<span data-ttu-id="4d212-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="4d212-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="4d212-150">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="4d212-150">The install state of the app.</span></span> <span data-ttu-id="4d212-151">Mögliche Werte: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="4d212-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="4d212-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="4d212-152">installStateDetail</span></span>|[<span data-ttu-id="4d212-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="4d212-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="4d212-154">Die Installationsstatus Details der app.</span><span class="sxs-lookup"><span data-stu-id="4d212-154">The install state detail of the app.</span></span> <span data-ttu-id="4d212-155">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="4d212-155">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="4d212-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="4d212-156">errorCode</span></span>|<span data-ttu-id="4d212-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4d212-157">Int32</span></span>|<span data-ttu-id="4d212-158">Der Fehlercode für Installations-oder Deinstallationsfehler.</span><span class="sxs-lookup"><span data-stu-id="4d212-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="4d212-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="4d212-159">osVersion</span></span>|<span data-ttu-id="4d212-160">String</span><span class="sxs-lookup"><span data-stu-id="4d212-160">String</span></span>|<span data-ttu-id="4d212-161">Betriebssystem Version</span><span class="sxs-lookup"><span data-stu-id="4d212-161">OS Version</span></span>|
|<span data-ttu-id="4d212-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="4d212-162">osDescription</span></span>|<span data-ttu-id="4d212-163">String</span><span class="sxs-lookup"><span data-stu-id="4d212-163">String</span></span>|<span data-ttu-id="4d212-164">Betriebssystem Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d212-164">OS Description</span></span>|
|<span data-ttu-id="4d212-165">userName</span><span class="sxs-lookup"><span data-stu-id="4d212-165">userName</span></span>|<span data-ttu-id="4d212-166">String</span><span class="sxs-lookup"><span data-stu-id="4d212-166">String</span></span>|<span data-ttu-id="4d212-167">Geräte Benutzer Name</span><span class="sxs-lookup"><span data-stu-id="4d212-167">Device User Name</span></span>|
|<span data-ttu-id="4d212-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d212-168">userPrincipalName</span></span>|<span data-ttu-id="4d212-169">String</span><span class="sxs-lookup"><span data-stu-id="4d212-169">String</span></span>|<span data-ttu-id="4d212-170">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="4d212-170">User Principal Name</span></span>|
|<span data-ttu-id="4d212-171">Display Version</span><span class="sxs-lookup"><span data-stu-id="4d212-171">displayVersion</span></span>|<span data-ttu-id="4d212-172">String</span><span class="sxs-lookup"><span data-stu-id="4d212-172">String</span></span>|<span data-ttu-id="4d212-173">Lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d212-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="4d212-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d212-174">Response</span></span>
<span data-ttu-id="4d212-175">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4d212-175">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d212-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d212-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d212-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d212-177">Request</span></span>
<span data-ttu-id="4d212-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d212-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="4d212-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d212-179">Response</span></span>
<span data-ttu-id="4d212-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d212-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




