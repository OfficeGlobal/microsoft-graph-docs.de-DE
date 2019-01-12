---
title: Erstellen von mobileAppInstallStatus
description: Erstellen eines neuen MobileAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2425ee773068eea2446b19534f907f48a43fe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970766"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="52752-103">Erstellen von mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="52752-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="52752-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="52752-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52752-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52752-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="52752-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52752-107">Erstellen eines neuen [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="52752-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52752-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="52752-108">Prerequisites</span></span>
<span data-ttu-id="52752-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52752-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52752-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52752-111">Permission type</span></span>|<span data-ttu-id="52752-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52752-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52752-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52752-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52752-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52752-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52752-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52752-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52752-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52752-116">Not supported.</span></span>|
|<span data-ttu-id="52752-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52752-117">Application</span></span>|<span data-ttu-id="52752-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52752-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52752-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52752-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="52752-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52752-120">Request headers</span></span>
|<span data-ttu-id="52752-121">Header</span><span class="sxs-lookup"><span data-stu-id="52752-121">Header</span></span>|<span data-ttu-id="52752-122">Wert</span><span class="sxs-lookup"><span data-stu-id="52752-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52752-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52752-123">Authorization</span></span>|<span data-ttu-id="52752-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="52752-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52752-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="52752-125">Accept</span></span>|<span data-ttu-id="52752-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52752-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52752-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52752-127">Request body</span></span>
<span data-ttu-id="52752-128">Geben Sie im Textkörper Anforderung für das Objekt MobileAppInstallStatus eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="52752-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="52752-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MobileAppInstallStatus erstellen.</span><span class="sxs-lookup"><span data-stu-id="52752-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="52752-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52752-130">Property</span></span>|<span data-ttu-id="52752-131">Typ</span><span class="sxs-lookup"><span data-stu-id="52752-131">Type</span></span>|<span data-ttu-id="52752-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52752-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52752-133">id</span><span class="sxs-lookup"><span data-stu-id="52752-133">id</span></span>|<span data-ttu-id="52752-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-134">String</span></span>|<span data-ttu-id="52752-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="52752-135">Key of the entity.</span></span>|
|<span data-ttu-id="52752-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="52752-136">deviceName</span></span>|<span data-ttu-id="52752-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-137">String</span></span>|<span data-ttu-id="52752-138">Gerätename</span><span class="sxs-lookup"><span data-stu-id="52752-138">Device name</span></span>|
|<span data-ttu-id="52752-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="52752-139">deviceId</span></span>|<span data-ttu-id="52752-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-140">String</span></span>|<span data-ttu-id="52752-141">Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="52752-141">Device ID</span></span>|
|<span data-ttu-id="52752-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52752-142">lastSyncDateTime</span></span>|<span data-ttu-id="52752-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52752-143">DateTimeOffset</span></span>|<span data-ttu-id="52752-144">Letzte Synchronisierung Datum-Zeit</span><span class="sxs-lookup"><span data-stu-id="52752-144">Last sync date time</span></span>|
|<span data-ttu-id="52752-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="52752-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="52752-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="52752-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="52752-147">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="52752-147">The install state of the app.</span></span> <span data-ttu-id="52752-148">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="52752-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="52752-149">installState</span><span class="sxs-lookup"><span data-stu-id="52752-149">installState</span></span>|[<span data-ttu-id="52752-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="52752-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="52752-151">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="52752-151">The install state of the app.</span></span> <span data-ttu-id="52752-152">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="52752-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="52752-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="52752-153">installStateDetail</span></span>|[<span data-ttu-id="52752-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="52752-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="52752-155">Die Details der Installation Zustand der app.</span><span class="sxs-lookup"><span data-stu-id="52752-155">The install state detail of the app.</span></span> <span data-ttu-id="52752-156">Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="52752-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="52752-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="52752-157">errorCode</span></span>|<span data-ttu-id="52752-158">Int32</span><span class="sxs-lookup"><span data-stu-id="52752-158">Int32</span></span>|<span data-ttu-id="52752-159">Der Fehler im code für die Installation oder Deinstallieren von Fehlern.</span><span class="sxs-lookup"><span data-stu-id="52752-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="52752-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="52752-160">osVersion</span></span>|<span data-ttu-id="52752-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-161">String</span></span>|<span data-ttu-id="52752-162">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="52752-162">OS Version</span></span>|
|<span data-ttu-id="52752-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="52752-163">osDescription</span></span>|<span data-ttu-id="52752-164">String</span><span class="sxs-lookup"><span data-stu-id="52752-164">String</span></span>|<span data-ttu-id="52752-165">OS Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52752-165">OS Description</span></span>|
|<span data-ttu-id="52752-166">userName</span><span class="sxs-lookup"><span data-stu-id="52752-166">userName</span></span>|<span data-ttu-id="52752-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-167">String</span></span>|<span data-ttu-id="52752-168">Name des Aufnahmegeräts Benutzer</span><span class="sxs-lookup"><span data-stu-id="52752-168">Device User Name</span></span>|
|<span data-ttu-id="52752-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52752-169">userPrincipalName</span></span>|<span data-ttu-id="52752-170">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-170">String</span></span>|<span data-ttu-id="52752-171">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="52752-171">User Principal Name</span></span>|
|<span data-ttu-id="52752-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="52752-172">displayVersion</span></span>|<span data-ttu-id="52752-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52752-173">String</span></span>|<span data-ttu-id="52752-174">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="52752-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="52752-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="52752-175">Response</span></span>
<span data-ttu-id="52752-176">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="52752-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52752-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52752-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="52752-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52752-178">Request</span></span>
<span data-ttu-id="52752-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52752-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52752-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="52752-180">Response</span></span>
<span data-ttu-id="52752-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52752-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





