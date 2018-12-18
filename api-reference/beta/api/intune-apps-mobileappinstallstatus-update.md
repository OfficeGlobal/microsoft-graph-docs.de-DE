---
title: MobileAppInstallStatus aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MobileAppInstallStatus-Objekts.
author: tfitzmac
ms.openlocfilehash: dbf65aa07258b48a8ce64cf01db0a5ef00097f3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336323"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="6637a-103">MobileAppInstallStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6637a-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="6637a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6637a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6637a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6637a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6637a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6637a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6637a-107">Aktualisieren Sie die Eigenschaften eines [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6637a-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6637a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6637a-108">Prerequisites</span></span>
<span data-ttu-id="6637a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6637a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6637a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6637a-111">Permission type</span></span>|<span data-ttu-id="6637a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6637a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6637a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6637a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6637a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6637a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6637a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6637a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6637a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6637a-116">Not supported.</span></span>|
|<span data-ttu-id="6637a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6637a-117">Application</span></span>|<span data-ttu-id="6637a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6637a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6637a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6637a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6637a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6637a-120">Request headers</span></span>
|<span data-ttu-id="6637a-121">Header</span><span class="sxs-lookup"><span data-stu-id="6637a-121">Header</span></span>|<span data-ttu-id="6637a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6637a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6637a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6637a-123">Authorization</span></span>|<span data-ttu-id="6637a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6637a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6637a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6637a-125">Accept</span></span>|<span data-ttu-id="6637a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6637a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6637a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6637a-127">Request body</span></span>
<span data-ttu-id="6637a-128">Geben Sie im Textkörper Anforderung für das Objekt [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6637a-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="6637a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="6637a-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="6637a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6637a-130">Property</span></span>|<span data-ttu-id="6637a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6637a-131">Type</span></span>|<span data-ttu-id="6637a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6637a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6637a-133">id</span><span class="sxs-lookup"><span data-stu-id="6637a-133">id</span></span>|<span data-ttu-id="6637a-134">String</span><span class="sxs-lookup"><span data-stu-id="6637a-134">String</span></span>|<span data-ttu-id="6637a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6637a-135">Key of the entity.</span></span>|
|<span data-ttu-id="6637a-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="6637a-136">deviceName</span></span>|<span data-ttu-id="6637a-137">String</span><span class="sxs-lookup"><span data-stu-id="6637a-137">String</span></span>|<span data-ttu-id="6637a-138">Gerätename</span><span class="sxs-lookup"><span data-stu-id="6637a-138">Device name</span></span>|
|<span data-ttu-id="6637a-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="6637a-139">deviceId</span></span>|<span data-ttu-id="6637a-140">String</span><span class="sxs-lookup"><span data-stu-id="6637a-140">String</span></span>|<span data-ttu-id="6637a-141">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="6637a-141">Device ID</span></span>|
|<span data-ttu-id="6637a-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6637a-142">lastSyncDateTime</span></span>|<span data-ttu-id="6637a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6637a-143">DateTimeOffset</span></span>|<span data-ttu-id="6637a-144">Letzte Synchronisierung Datum-Zeit</span><span class="sxs-lookup"><span data-stu-id="6637a-144">Last sync date time</span></span>|
|<span data-ttu-id="6637a-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="6637a-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="6637a-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="6637a-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="6637a-147">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="6637a-147">The install state of the app.</span></span> <span data-ttu-id="6637a-148">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="6637a-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="6637a-149">installState</span><span class="sxs-lookup"><span data-stu-id="6637a-149">installState</span></span>|[<span data-ttu-id="6637a-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="6637a-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="6637a-151">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="6637a-151">The install state of the app.</span></span> <span data-ttu-id="6637a-152">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="6637a-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="6637a-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="6637a-153">installStateDetail</span></span>|[<span data-ttu-id="6637a-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="6637a-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="6637a-155">Die Details der Installation Zustand der app.</span><span class="sxs-lookup"><span data-stu-id="6637a-155">The install state detail of the app.</span></span> <span data-ttu-id="6637a-156">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="6637a-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="6637a-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="6637a-157">errorCode</span></span>|<span data-ttu-id="6637a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6637a-158">Int32</span></span>|<span data-ttu-id="6637a-159">Der Fehler im code für die Installation oder Deinstallieren von Fehlern.</span><span class="sxs-lookup"><span data-stu-id="6637a-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="6637a-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="6637a-160">osVersion</span></span>|<span data-ttu-id="6637a-161">String</span><span class="sxs-lookup"><span data-stu-id="6637a-161">String</span></span>|<span data-ttu-id="6637a-162">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="6637a-162">OS Version</span></span>|
|<span data-ttu-id="6637a-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="6637a-163">osDescription</span></span>|<span data-ttu-id="6637a-164">String</span><span class="sxs-lookup"><span data-stu-id="6637a-164">String</span></span>|<span data-ttu-id="6637a-165">OS Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6637a-165">OS Description</span></span>|
|<span data-ttu-id="6637a-166">userName</span><span class="sxs-lookup"><span data-stu-id="6637a-166">userName</span></span>|<span data-ttu-id="6637a-167">String</span><span class="sxs-lookup"><span data-stu-id="6637a-167">String</span></span>|<span data-ttu-id="6637a-168">Name des Aufnahmegeräts Benutzer</span><span class="sxs-lookup"><span data-stu-id="6637a-168">Device User Name</span></span>|
|<span data-ttu-id="6637a-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6637a-169">userPrincipalName</span></span>|<span data-ttu-id="6637a-170">String</span><span class="sxs-lookup"><span data-stu-id="6637a-170">String</span></span>|<span data-ttu-id="6637a-171">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="6637a-171">User Principal Name</span></span>|
|<span data-ttu-id="6637a-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="6637a-172">displayVersion</span></span>|<span data-ttu-id="6637a-173">String</span><span class="sxs-lookup"><span data-stu-id="6637a-173">String</span></span>|<span data-ttu-id="6637a-174">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="6637a-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="6637a-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="6637a-175">Response</span></span>
<span data-ttu-id="6637a-176">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6637a-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6637a-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6637a-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="6637a-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6637a-178">Request</span></span>
<span data-ttu-id="6637a-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6637a-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 488

{
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

### <a name="response"></a><span data-ttu-id="6637a-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="6637a-180">Response</span></span>
<span data-ttu-id="6637a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6637a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





