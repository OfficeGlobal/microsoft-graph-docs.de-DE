---
title: Erstellen von importedAppleDeviceIdentityResult
description: Erstellen eines neuen ImportedAppleDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4d8a585aa2e6745d563d1a886fa5c7870ced9a87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817415"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="c776d-103">Erstellen von importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="c776d-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="c776d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c776d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c776d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c776d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c776d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c776d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c776d-107">Erstellen eines neuen [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c776d-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c776d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c776d-108">Prerequisites</span></span>
<span data-ttu-id="c776d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c776d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c776d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c776d-111">Permission type</span></span>|<span data-ttu-id="c776d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c776d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c776d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c776d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c776d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c776d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c776d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c776d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c776d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c776d-116">Not supported.</span></span>|
|<span data-ttu-id="c776d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c776d-117">Application</span></span>|<span data-ttu-id="c776d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c776d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c776d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c776d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="c776d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c776d-120">Request headers</span></span>
|<span data-ttu-id="c776d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c776d-121">Header</span></span>|<span data-ttu-id="c776d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c776d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c776d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c776d-123">Authorization</span></span>|<span data-ttu-id="c776d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c776d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c776d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c776d-125">Accept</span></span>|<span data-ttu-id="c776d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c776d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c776d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c776d-127">Request body</span></span>
<span data-ttu-id="c776d-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedAppleDeviceIdentityResult eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c776d-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="c776d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedAppleDeviceIdentityResult erstellen.</span><span class="sxs-lookup"><span data-stu-id="c776d-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="c776d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c776d-130">Property</span></span>|<span data-ttu-id="c776d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c776d-131">Type</span></span>|<span data-ttu-id="c776d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c776d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c776d-133">id</span><span class="sxs-lookup"><span data-stu-id="c776d-133">id</span></span>|<span data-ttu-id="c776d-134">String</span><span class="sxs-lookup"><span data-stu-id="c776d-134">String</span></span>|<span data-ttu-id="c776d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c776d-135">Key of the entity.</span></span> <span data-ttu-id="c776d-136">Geerbt von [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c776d-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c776d-137">serialNumber</span></span>|<span data-ttu-id="c776d-138">String</span><span class="sxs-lookup"><span data-stu-id="c776d-138">String</span></span>|<span data-ttu-id="c776d-139">Seriennummer des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c776d-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="c776d-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="c776d-141">String</span><span class="sxs-lookup"><span data-stu-id="c776d-141">String</span></span>|<span data-ttu-id="c776d-142">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) anwenden</span><span class="sxs-lookup"><span data-stu-id="c776d-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="c776d-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="c776d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c776d-144">DateTimeOffset</span></span>|<span data-ttu-id="c776d-145">Das Zeit Registrierung Profil wurde auf das Gerät Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="c776d-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c776d-146">isSupervised</span></span>|<span data-ttu-id="c776d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c776d-147">Boolean</span></span>|<span data-ttu-id="c776d-148">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="c776d-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="c776d-149">Weitere Informationen finden Sie unter: https://support.apple.com/en-us/HT202837 von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="c776d-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c776d-150">discoverySource</span></span>|[<span data-ttu-id="c776d-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c776d-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="c776d-152">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="c776d-152">Apple device discovery source.</span></span> <span data-ttu-id="c776d-153">Geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="c776d-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c776d-154">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="c776d-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="c776d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c776d-155">createdDateTime</span></span>|<span data-ttu-id="c776d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c776d-156">DateTimeOffset</span></span>|<span data-ttu-id="c776d-157">Datum-Uhrzeit des Geräts Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="c776d-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c776d-158">lastContactedDateTime</span></span>|<span data-ttu-id="c776d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c776d-159">DateTimeOffset</span></span>|<span data-ttu-id="c776d-160">Letzte kontaktiert Datum-Uhrzeit des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c776d-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-161">description</span><span class="sxs-lookup"><span data-stu-id="c776d-161">description</span></span>|<span data-ttu-id="c776d-162">String</span><span class="sxs-lookup"><span data-stu-id="c776d-162">String</span></span>|<span data-ttu-id="c776d-163">Die Beschreibung des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c776d-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c776d-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c776d-164">enrollmentState</span></span>|[<span data-ttu-id="c776d-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c776d-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="c776d-166">Der Zustand des Geräts in Intune geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="c776d-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c776d-167">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="c776d-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c776d-168">Plattform</span><span class="sxs-lookup"><span data-stu-id="c776d-168">platform</span></span>|[<span data-ttu-id="c776d-169">Plattform</span><span class="sxs-lookup"><span data-stu-id="c776d-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="c776d-170">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="c776d-170">The platform of the Device.</span></span> <span data-ttu-id="c776d-171">Geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="c776d-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c776d-172">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="c776d-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="c776d-173">status</span><span class="sxs-lookup"><span data-stu-id="c776d-173">status</span></span>|<span data-ttu-id="c776d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c776d-174">Boolean</span></span>|<span data-ttu-id="c776d-175">Status der importierten Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="c776d-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="c776d-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="c776d-176">Response</span></span>
<span data-ttu-id="c776d-177">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c776d-177">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c776d-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c776d-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="c776d-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c776d-179">Request</span></span>
<span data-ttu-id="c776d-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c776d-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="c776d-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="c776d-181">Response</span></span>
<span data-ttu-id="c776d-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c776d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





