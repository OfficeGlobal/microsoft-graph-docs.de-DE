---
title: Erstellen von importedAppleDeviceIdentityResult
description: Erstellen eines neuen ImportedAppleDeviceIdentityResult-Objekts.
author: tfitzmac
ms.openlocfilehash: 1560f8e05057327a6aafc5258e7c5c46b9bcb781
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316051"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="342be-103">Erstellen von importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="342be-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="342be-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="342be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="342be-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="342be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="342be-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="342be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="342be-107">Erstellen eines neuen [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="342be-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="342be-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="342be-108">Prerequisites</span></span>
<span data-ttu-id="342be-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="342be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="342be-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="342be-111">Permission type</span></span>|<span data-ttu-id="342be-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="342be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="342be-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="342be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="342be-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="342be-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="342be-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="342be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="342be-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="342be-116">Not supported.</span></span>|
|<span data-ttu-id="342be-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="342be-117">Application</span></span>|<span data-ttu-id="342be-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="342be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="342be-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="342be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="342be-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="342be-120">Request headers</span></span>
|<span data-ttu-id="342be-121">Header</span><span class="sxs-lookup"><span data-stu-id="342be-121">Header</span></span>|<span data-ttu-id="342be-122">Wert</span><span class="sxs-lookup"><span data-stu-id="342be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="342be-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="342be-123">Authorization</span></span>|<span data-ttu-id="342be-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="342be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="342be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="342be-125">Accept</span></span>|<span data-ttu-id="342be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="342be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="342be-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="342be-127">Request body</span></span>
<span data-ttu-id="342be-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedAppleDeviceIdentityResult eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="342be-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="342be-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedAppleDeviceIdentityResult erstellen.</span><span class="sxs-lookup"><span data-stu-id="342be-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="342be-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="342be-130">Property</span></span>|<span data-ttu-id="342be-131">Typ</span><span class="sxs-lookup"><span data-stu-id="342be-131">Type</span></span>|<span data-ttu-id="342be-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="342be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="342be-133">id</span><span class="sxs-lookup"><span data-stu-id="342be-133">id</span></span>|<span data-ttu-id="342be-134">String</span><span class="sxs-lookup"><span data-stu-id="342be-134">String</span></span>|<span data-ttu-id="342be-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="342be-135">Key of the entity.</span></span> <span data-ttu-id="342be-136">Geerbt von [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="342be-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="342be-137">serialNumber</span></span>|<span data-ttu-id="342be-138">String</span><span class="sxs-lookup"><span data-stu-id="342be-138">String</span></span>|<span data-ttu-id="342be-139">Seriennummer des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="342be-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="342be-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="342be-141">String</span><span class="sxs-lookup"><span data-stu-id="342be-141">String</span></span>|<span data-ttu-id="342be-142">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) anwenden</span><span class="sxs-lookup"><span data-stu-id="342be-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="342be-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="342be-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="342be-144">DateTimeOffset</span></span>|<span data-ttu-id="342be-145">Das Zeit Registrierung Profil wurde auf das Gerät Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="342be-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="342be-146">isSupervised</span></span>|<span data-ttu-id="342be-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="342be-147">Boolean</span></span>|<span data-ttu-id="342be-148">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="342be-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="342be-149">Weitere Informationen finden Sie unter: https://support.apple.com/en-us/HT202837 von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="342be-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="342be-150">discoverySource</span></span>|[<span data-ttu-id="342be-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="342be-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="342be-152">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="342be-152">Apple device discovery source.</span></span> <span data-ttu-id="342be-153">Geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="342be-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="342be-154">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="342be-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="342be-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="342be-155">createdDateTime</span></span>|<span data-ttu-id="342be-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="342be-156">DateTimeOffset</span></span>|<span data-ttu-id="342be-157">Datum-Uhrzeit des Geräts Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="342be-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="342be-158">lastContactedDateTime</span></span>|<span data-ttu-id="342be-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="342be-159">DateTimeOffset</span></span>|<span data-ttu-id="342be-160">Letzte kontaktiert Datum-Uhrzeit des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="342be-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-161">description</span><span class="sxs-lookup"><span data-stu-id="342be-161">description</span></span>|<span data-ttu-id="342be-162">String</span><span class="sxs-lookup"><span data-stu-id="342be-162">String</span></span>|<span data-ttu-id="342be-163">Die Beschreibung des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="342be-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="342be-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="342be-164">enrollmentState</span></span>|[<span data-ttu-id="342be-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="342be-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="342be-166">Der Zustand des Geräts in Intune geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="342be-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="342be-167">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="342be-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="342be-168">Plattform</span><span class="sxs-lookup"><span data-stu-id="342be-168">platform</span></span>|[<span data-ttu-id="342be-169">Plattform</span><span class="sxs-lookup"><span data-stu-id="342be-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="342be-170">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="342be-170">The platform of the Device.</span></span> <span data-ttu-id="342be-171">Geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="342be-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="342be-172">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="342be-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="342be-173">status</span><span class="sxs-lookup"><span data-stu-id="342be-173">status</span></span>|<span data-ttu-id="342be-174">Boolesch</span><span class="sxs-lookup"><span data-stu-id="342be-174">Boolean</span></span>|<span data-ttu-id="342be-175">Status der importierten Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="342be-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="342be-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="342be-176">Response</span></span>
<span data-ttu-id="342be-177">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="342be-177">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="342be-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="342be-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="342be-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="342be-179">Request</span></span>
<span data-ttu-id="342be-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="342be-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="342be-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="342be-181">Response</span></span>
<span data-ttu-id="342be-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="342be-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





