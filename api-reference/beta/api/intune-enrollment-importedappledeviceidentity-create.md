---
title: Erstellen von importedAppleDeviceIdentity
description: Erstellen eines neuen ImportedAppleDeviceIdentity-Objekts.
ms.openlocfilehash: dae2d56990c9f6cdfb5c0adc5c6a457ade52e161
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058868"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="26e5e-103">Erstellen von importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="26e5e-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="26e5e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="26e5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26e5e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26e5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26e5e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="26e5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26e5e-107">Erstellen eines neuen [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="26e5e-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26e5e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="26e5e-108">Prerequisites</span></span>
<span data-ttu-id="26e5e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e5e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26e5e-111">Permission type</span></span>|<span data-ttu-id="26e5e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26e5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e5e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26e5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26e5e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e5e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26e5e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26e5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e5e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26e5e-116">Not supported.</span></span>|
|<span data-ttu-id="26e5e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26e5e-117">Application</span></span>|<span data-ttu-id="26e5e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26e5e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e5e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26e5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="26e5e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26e5e-120">Request headers</span></span>
|<span data-ttu-id="26e5e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="26e5e-121">Header</span></span>|<span data-ttu-id="26e5e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="26e5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26e5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26e5e-123">Authorization</span></span>|<span data-ttu-id="26e5e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="26e5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26e5e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26e5e-125">Accept</span></span>|<span data-ttu-id="26e5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26e5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e5e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26e5e-127">Request body</span></span>
<span data-ttu-id="26e5e-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedAppleDeviceIdentity eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="26e5e-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="26e5e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedAppleDeviceIdentity erstellen.</span><span class="sxs-lookup"><span data-stu-id="26e5e-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="26e5e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26e5e-130">Property</span></span>|<span data-ttu-id="26e5e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="26e5e-131">Type</span></span>|<span data-ttu-id="26e5e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26e5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e5e-133">id</span><span class="sxs-lookup"><span data-stu-id="26e5e-133">id</span></span>|<span data-ttu-id="26e5e-134">String</span><span class="sxs-lookup"><span data-stu-id="26e5e-134">String</span></span>|<span data-ttu-id="26e5e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="26e5e-135">Key of the entity.</span></span>|
|<span data-ttu-id="26e5e-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="26e5e-136">serialNumber</span></span>|<span data-ttu-id="26e5e-137">String</span><span class="sxs-lookup"><span data-stu-id="26e5e-137">String</span></span>|<span data-ttu-id="26e5e-138">Seriennummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="26e5e-138">Device serial number</span></span>|
|<span data-ttu-id="26e5e-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="26e5e-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="26e5e-140">String</span><span class="sxs-lookup"><span data-stu-id="26e5e-140">String</span></span>|<span data-ttu-id="26e5e-141">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung anwenden</span><span class="sxs-lookup"><span data-stu-id="26e5e-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="26e5e-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="26e5e-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="26e5e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e5e-143">DateTimeOffset</span></span>|<span data-ttu-id="26e5e-144">Das Zeit Registrierung Profil zugewiesen wurde das Gerät</span><span class="sxs-lookup"><span data-stu-id="26e5e-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="26e5e-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="26e5e-145">isSupervised</span></span>|<span data-ttu-id="26e5e-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="26e5e-146">Boolean</span></span>|<span data-ttu-id="26e5e-147">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="26e5e-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="26e5e-148">Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="26e5e-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="26e5e-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="26e5e-149">discoverySource</span></span>|[<span data-ttu-id="26e5e-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="26e5e-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="26e5e-151">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="26e5e-151">Apple device discovery source.</span></span> <span data-ttu-id="26e5e-152">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="26e5e-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="26e5e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26e5e-153">createdDateTime</span></span>|<span data-ttu-id="26e5e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e5e-154">DateTimeOffset</span></span>|<span data-ttu-id="26e5e-155">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="26e5e-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="26e5e-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="26e5e-156">lastContactedDateTime</span></span>|<span data-ttu-id="26e5e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e5e-157">DateTimeOffset</span></span>|<span data-ttu-id="26e5e-158">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="26e5e-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="26e5e-159">description</span><span class="sxs-lookup"><span data-stu-id="26e5e-159">description</span></span>|<span data-ttu-id="26e5e-160">String</span><span class="sxs-lookup"><span data-stu-id="26e5e-160">String</span></span>|<span data-ttu-id="26e5e-161">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="26e5e-161">The description of the device</span></span>|
|<span data-ttu-id="26e5e-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="26e5e-162">enrollmentState</span></span>|[<span data-ttu-id="26e5e-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="26e5e-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="26e5e-164">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="26e5e-164">The state of the device in Intune.</span></span> <span data-ttu-id="26e5e-165">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="26e5e-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="26e5e-166">Plattform</span><span class="sxs-lookup"><span data-stu-id="26e5e-166">platform</span></span>|[<span data-ttu-id="26e5e-167">Plattform</span><span class="sxs-lookup"><span data-stu-id="26e5e-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="26e5e-168">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="26e5e-168">The platform of the Device.</span></span> <span data-ttu-id="26e5e-169">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="26e5e-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="26e5e-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="26e5e-170">Response</span></span>
<span data-ttu-id="26e5e-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="26e5e-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e5e-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26e5e-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="26e5e-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26e5e-173">Request</span></span>
<span data-ttu-id="26e5e-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26e5e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="26e5e-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="26e5e-175">Response</span></span>
<span data-ttu-id="26e5e-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26e5e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





