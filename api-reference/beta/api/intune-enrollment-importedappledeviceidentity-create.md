---
title: Erstellen von importedAppleDeviceIdentity
description: Erstellen eines neuen ImportedAppleDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d1c88a7d1621cc386ea5fd299d6fc1b014cb7b05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848419"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="d37c2-103">Erstellen von importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d37c2-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="d37c2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d37c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d37c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d37c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d37c2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d37c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d37c2-107">Erstellen eines neuen [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d37c2-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d37c2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d37c2-108">Prerequisites</span></span>
<span data-ttu-id="d37c2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d37c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d37c2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d37c2-111">Permission type</span></span>|<span data-ttu-id="d37c2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d37c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d37c2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d37c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d37c2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37c2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d37c2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d37c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d37c2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d37c2-116">Not supported.</span></span>|
|<span data-ttu-id="d37c2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d37c2-117">Application</span></span>|<span data-ttu-id="d37c2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d37c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d37c2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d37c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d37c2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d37c2-120">Request headers</span></span>
|<span data-ttu-id="d37c2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d37c2-121">Header</span></span>|<span data-ttu-id="d37c2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d37c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d37c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d37c2-123">Authorization</span></span>|<span data-ttu-id="d37c2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d37c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d37c2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d37c2-125">Accept</span></span>|<span data-ttu-id="d37c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d37c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d37c2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d37c2-127">Request body</span></span>
<span data-ttu-id="d37c2-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedAppleDeviceIdentity eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d37c2-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="d37c2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedAppleDeviceIdentity erstellen.</span><span class="sxs-lookup"><span data-stu-id="d37c2-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="d37c2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d37c2-130">Property</span></span>|<span data-ttu-id="d37c2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d37c2-131">Type</span></span>|<span data-ttu-id="d37c2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d37c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37c2-133">id</span><span class="sxs-lookup"><span data-stu-id="d37c2-133">id</span></span>|<span data-ttu-id="d37c2-134">String</span><span class="sxs-lookup"><span data-stu-id="d37c2-134">String</span></span>|<span data-ttu-id="d37c2-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d37c2-135">Key of the entity.</span></span>|
|<span data-ttu-id="d37c2-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d37c2-136">serialNumber</span></span>|<span data-ttu-id="d37c2-137">String</span><span class="sxs-lookup"><span data-stu-id="d37c2-137">String</span></span>|<span data-ttu-id="d37c2-138">Seriennummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="d37c2-138">Device serial number</span></span>|
|<span data-ttu-id="d37c2-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="d37c2-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="d37c2-140">String</span><span class="sxs-lookup"><span data-stu-id="d37c2-140">String</span></span>|<span data-ttu-id="d37c2-141">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung anwenden</span><span class="sxs-lookup"><span data-stu-id="d37c2-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="d37c2-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="d37c2-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="d37c2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37c2-143">DateTimeOffset</span></span>|<span data-ttu-id="d37c2-144">Das Zeit Registrierung Profil zugewiesen wurde das Gerät</span><span class="sxs-lookup"><span data-stu-id="d37c2-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="d37c2-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d37c2-145">isSupervised</span></span>|<span data-ttu-id="d37c2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37c2-146">Boolean</span></span>|<span data-ttu-id="d37c2-147">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="d37c2-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="d37c2-148">Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="d37c2-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="d37c2-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="d37c2-149">discoverySource</span></span>|[<span data-ttu-id="d37c2-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="d37c2-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="d37c2-151">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="d37c2-151">Apple device discovery source.</span></span> <span data-ttu-id="d37c2-152">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="d37c2-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="d37c2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d37c2-153">createdDateTime</span></span>|<span data-ttu-id="d37c2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37c2-154">DateTimeOffset</span></span>|<span data-ttu-id="d37c2-155">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="d37c2-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="d37c2-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d37c2-156">lastContactedDateTime</span></span>|<span data-ttu-id="d37c2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37c2-157">DateTimeOffset</span></span>|<span data-ttu-id="d37c2-158">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="d37c2-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="d37c2-159">description</span><span class="sxs-lookup"><span data-stu-id="d37c2-159">description</span></span>|<span data-ttu-id="d37c2-160">String</span><span class="sxs-lookup"><span data-stu-id="d37c2-160">String</span></span>|<span data-ttu-id="d37c2-161">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="d37c2-161">The description of the device</span></span>|
|<span data-ttu-id="d37c2-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d37c2-162">enrollmentState</span></span>|[<span data-ttu-id="d37c2-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d37c2-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d37c2-164">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="d37c2-164">The state of the device in Intune.</span></span> <span data-ttu-id="d37c2-165">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d37c2-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d37c2-166">Plattform</span><span class="sxs-lookup"><span data-stu-id="d37c2-166">platform</span></span>|[<span data-ttu-id="d37c2-167">Plattform</span><span class="sxs-lookup"><span data-stu-id="d37c2-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d37c2-168">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d37c2-168">The platform of the Device.</span></span> <span data-ttu-id="d37c2-169">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="d37c2-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="d37c2-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="d37c2-170">Response</span></span>
<span data-ttu-id="d37c2-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d37c2-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d37c2-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d37c2-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="d37c2-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d37c2-173">Request</span></span>
<span data-ttu-id="d37c2-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d37c2-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d37c2-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="d37c2-175">Response</span></span>
<span data-ttu-id="d37c2-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d37c2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





