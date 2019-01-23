---
title: ImportedAppleDeviceIdentityResult aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedAppleDeviceIdentityResult-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d721da146e86e05b1e99a53c6570a8681adf7a06
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396455"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="1f8f3-103">ImportedAppleDeviceIdentityResult aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f8f3-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="1f8f3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1f8f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f8f3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f8f3-107">Aktualisieren Sie die Eigenschaften eines [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f8f3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f8f3-108">Prerequisites</span></span>
<span data-ttu-id="1f8f3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f8f3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f8f3-111">Permission type</span></span>|<span data-ttu-id="1f8f3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f8f3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f8f3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f8f3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f8f3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f8f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f8f3-116">Not supported.</span></span>|
|<span data-ttu-id="1f8f3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f8f3-117">Application</span></span>|<span data-ttu-id="1f8f3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f8f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f8f3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f8f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="1f8f3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f8f3-120">Request headers</span></span>
|<span data-ttu-id="1f8f3-121">Header</span><span class="sxs-lookup"><span data-stu-id="1f8f3-121">Header</span></span>|<span data-ttu-id="1f8f3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1f8f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f8f3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1f8f3-123">Authorization</span></span>|<span data-ttu-id="1f8f3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f8f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f8f3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1f8f3-125">Accept</span></span>|<span data-ttu-id="1f8f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f8f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f8f3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f8f3-127">Request body</span></span>
<span data-ttu-id="1f8f3-128">Geben Sie im Textkörper Anforderung für das Objekt [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="1f8f3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="1f8f3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f8f3-130">Property</span></span>|<span data-ttu-id="1f8f3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1f8f3-131">Type</span></span>|<span data-ttu-id="1f8f3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f8f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f8f3-133">id</span><span class="sxs-lookup"><span data-stu-id="1f8f3-133">id</span></span>|<span data-ttu-id="1f8f3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f8f3-134">String</span></span>|<span data-ttu-id="1f8f3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1f8f3-135">Key of the entity.</span></span> <span data-ttu-id="1f8f3-136">Geerbt von [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1f8f3-137">serialNumber</span></span>|<span data-ttu-id="1f8f3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f8f3-138">String</span></span>|<span data-ttu-id="1f8f3-139">Seriennummer des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="1f8f3-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="1f8f3-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f8f3-141">String</span></span>|<span data-ttu-id="1f8f3-142">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) anwenden</span><span class="sxs-lookup"><span data-stu-id="1f8f3-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="1f8f3-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="1f8f3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f8f3-144">DateTimeOffset</span></span>|<span data-ttu-id="1f8f3-145">Das Zeit Registrierung Profil wurde auf das Gerät Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1f8f3-146">isSupervised</span></span>|<span data-ttu-id="1f8f3-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8f3-147">Boolean</span></span>|<span data-ttu-id="1f8f3-148">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="1f8f3-149">Weitere Informationen finden Sie unter: https://support.apple.com/en-us/HT202837 von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1f8f3-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1f8f3-150">discoverySource</span></span>|[<span data-ttu-id="1f8f3-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1f8f3-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="1f8f3-152">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-152">Apple device discovery source.</span></span> <span data-ttu-id="1f8f3-153">Geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f3-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="1f8f3-154">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="1f8f3-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f8f3-155">createdDateTime</span></span>|<span data-ttu-id="1f8f3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f8f3-156">DateTimeOffset</span></span>|<span data-ttu-id="1f8f3-157">Datum-Uhrzeit des Geräts Inherited aus [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="1f8f3-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f8f3-158">lastContactedDateTime</span></span>|<span data-ttu-id="1f8f3-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f8f3-159">DateTimeOffset</span></span>|<span data-ttu-id="1f8f3-160">Letzte kontaktiert Datum-Uhrzeit des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-161">description</span><span class="sxs-lookup"><span data-stu-id="1f8f3-161">description</span></span>|<span data-ttu-id="1f8f3-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f8f3-162">String</span></span>|<span data-ttu-id="1f8f3-163">Die Beschreibung des Geräts Inherited aus [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="1f8f3-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="1f8f3-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1f8f3-164">enrollmentState</span></span>|[<span data-ttu-id="1f8f3-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1f8f3-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="1f8f3-166">Der Zustand des Geräts in Intune geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f3-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="1f8f3-167">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1f8f3-168">Plattform</span><span class="sxs-lookup"><span data-stu-id="1f8f3-168">platform</span></span>|[<span data-ttu-id="1f8f3-169">Plattform</span><span class="sxs-lookup"><span data-stu-id="1f8f3-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1f8f3-170">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-170">The platform of the Device.</span></span> <span data-ttu-id="1f8f3-171">Geerbt von [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f3-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="1f8f3-172">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="1f8f3-173">status</span><span class="sxs-lookup"><span data-stu-id="1f8f3-173">status</span></span>|<span data-ttu-id="1f8f3-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8f3-174">Boolean</span></span>|<span data-ttu-id="1f8f3-175">Status der importierten Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="1f8f3-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="1f8f3-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f8f3-176">Response</span></span>
<span data-ttu-id="1f8f3-177">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-177">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f8f3-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f8f3-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f8f3-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f8f3-179">Request</span></span>
<span data-ttu-id="1f8f3-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="1f8f3-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f8f3-181">Response</span></span>
<span data-ttu-id="1f8f3-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f8f3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




