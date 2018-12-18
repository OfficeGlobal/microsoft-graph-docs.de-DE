---
title: Erstellen von mobileAppInstallStatus
description: Erstellen eines neuen MobileAppInstallStatus-Objekts.
author: tfitzmac
ms.openlocfilehash: 12dfa8e7f827ef2d2933249a6089d000ef868769
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318109"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="f32dd-103">Erstellen von mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f32dd-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="f32dd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f32dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f32dd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f32dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f32dd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f32dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f32dd-107">Erstellen eines neuen [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f32dd-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f32dd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f32dd-108">Prerequisites</span></span>
<span data-ttu-id="f32dd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f32dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f32dd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f32dd-111">Permission type</span></span>|<span data-ttu-id="f32dd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f32dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f32dd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f32dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f32dd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32dd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f32dd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f32dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f32dd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f32dd-116">Not supported.</span></span>|
|<span data-ttu-id="f32dd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f32dd-117">Application</span></span>|<span data-ttu-id="f32dd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f32dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f32dd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f32dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f32dd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f32dd-120">Request headers</span></span>
|<span data-ttu-id="f32dd-121">Header</span><span class="sxs-lookup"><span data-stu-id="f32dd-121">Header</span></span>|<span data-ttu-id="f32dd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f32dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f32dd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f32dd-123">Authorization</span></span>|<span data-ttu-id="f32dd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f32dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f32dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f32dd-125">Accept</span></span>|<span data-ttu-id="f32dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f32dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f32dd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f32dd-127">Request body</span></span>
<span data-ttu-id="f32dd-128">Geben Sie im Textkörper Anforderung für das Objekt MobileAppInstallStatus eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f32dd-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="f32dd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MobileAppInstallStatus erstellen.</span><span class="sxs-lookup"><span data-stu-id="f32dd-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="f32dd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f32dd-130">Property</span></span>|<span data-ttu-id="f32dd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f32dd-131">Type</span></span>|<span data-ttu-id="f32dd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f32dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f32dd-133">id</span><span class="sxs-lookup"><span data-stu-id="f32dd-133">id</span></span>|<span data-ttu-id="f32dd-134">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-134">String</span></span>|<span data-ttu-id="f32dd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f32dd-135">Key of the entity.</span></span>|
|<span data-ttu-id="f32dd-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="f32dd-136">deviceName</span></span>|<span data-ttu-id="f32dd-137">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-137">String</span></span>|<span data-ttu-id="f32dd-138">Gerätename</span><span class="sxs-lookup"><span data-stu-id="f32dd-138">Device name</span></span>|
|<span data-ttu-id="f32dd-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f32dd-139">deviceId</span></span>|<span data-ttu-id="f32dd-140">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-140">String</span></span>|<span data-ttu-id="f32dd-141">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="f32dd-141">Device ID</span></span>|
|<span data-ttu-id="f32dd-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f32dd-142">lastSyncDateTime</span></span>|<span data-ttu-id="f32dd-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32dd-143">DateTimeOffset</span></span>|<span data-ttu-id="f32dd-144">Letzte Synchronisierung Datum-Zeit</span><span class="sxs-lookup"><span data-stu-id="f32dd-144">Last sync date time</span></span>|
|<span data-ttu-id="f32dd-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="f32dd-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="f32dd-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="f32dd-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f32dd-147">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="f32dd-147">The install state of the app.</span></span> <span data-ttu-id="f32dd-148">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f32dd-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f32dd-149">installState</span><span class="sxs-lookup"><span data-stu-id="f32dd-149">installState</span></span>|[<span data-ttu-id="f32dd-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="f32dd-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f32dd-151">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="f32dd-151">The install state of the app.</span></span> <span data-ttu-id="f32dd-152">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f32dd-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f32dd-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="f32dd-153">installStateDetail</span></span>|[<span data-ttu-id="f32dd-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="f32dd-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="f32dd-155">Die Details der Installation Zustand der app.</span><span class="sxs-lookup"><span data-stu-id="f32dd-155">The install state detail of the app.</span></span> <span data-ttu-id="f32dd-156">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f32dd-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="f32dd-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="f32dd-157">errorCode</span></span>|<span data-ttu-id="f32dd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f32dd-158">Int32</span></span>|<span data-ttu-id="f32dd-159">Der Fehler im code für die Installation oder Deinstallieren von Fehlern.</span><span class="sxs-lookup"><span data-stu-id="f32dd-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="f32dd-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="f32dd-160">osVersion</span></span>|<span data-ttu-id="f32dd-161">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-161">String</span></span>|<span data-ttu-id="f32dd-162">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="f32dd-162">OS Version</span></span>|
|<span data-ttu-id="f32dd-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="f32dd-163">osDescription</span></span>|<span data-ttu-id="f32dd-164">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-164">String</span></span>|<span data-ttu-id="f32dd-165">OS Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f32dd-165">OS Description</span></span>|
|<span data-ttu-id="f32dd-166">userName</span><span class="sxs-lookup"><span data-stu-id="f32dd-166">userName</span></span>|<span data-ttu-id="f32dd-167">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-167">String</span></span>|<span data-ttu-id="f32dd-168">Name des Aufnahmegeräts Benutzer</span><span class="sxs-lookup"><span data-stu-id="f32dd-168">Device User Name</span></span>|
|<span data-ttu-id="f32dd-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f32dd-169">userPrincipalName</span></span>|<span data-ttu-id="f32dd-170">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-170">String</span></span>|<span data-ttu-id="f32dd-171">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="f32dd-171">User Principal Name</span></span>|
|<span data-ttu-id="f32dd-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="f32dd-172">displayVersion</span></span>|<span data-ttu-id="f32dd-173">String</span><span class="sxs-lookup"><span data-stu-id="f32dd-173">String</span></span>|<span data-ttu-id="f32dd-174">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f32dd-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="f32dd-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="f32dd-175">Response</span></span>
<span data-ttu-id="f32dd-176">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f32dd-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f32dd-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f32dd-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="f32dd-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f32dd-178">Request</span></span>
<span data-ttu-id="f32dd-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f32dd-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f32dd-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="f32dd-180">Response</span></span>
<span data-ttu-id="f32dd-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f32dd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





