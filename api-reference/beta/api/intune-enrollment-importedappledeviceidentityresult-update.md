---
title: ImportedAppleDeviceIdentityResult aktualisieren
description: Aktualisieren der Eigenschaften eines importedAppleDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85f2446058aa899f8b624b843ee25df148cec416
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154383"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="0320b-103">ImportedAppleDeviceIdentityResult aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0320b-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="0320b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0320b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0320b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0320b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0320b-106">Aktualisieren der Eigenschaften eines [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0320b-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0320b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0320b-107">Prerequisites</span></span>
<span data-ttu-id="0320b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0320b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0320b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0320b-110">Permission type</span></span>|<span data-ttu-id="0320b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0320b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0320b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0320b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0320b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0320b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0320b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0320b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0320b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0320b-115">Not supported.</span></span>|
|<span data-ttu-id="0320b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0320b-116">Application</span></span>|<span data-ttu-id="0320b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0320b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0320b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0320b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0320b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0320b-119">Request headers</span></span>
|<span data-ttu-id="0320b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0320b-120">Header</span></span>|<span data-ttu-id="0320b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0320b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0320b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0320b-122">Authorization</span></span>|<span data-ttu-id="0320b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0320b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0320b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0320b-124">Accept</span></span>|<span data-ttu-id="0320b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0320b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0320b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0320b-126">Request body</span></span>
<span data-ttu-id="0320b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0320b-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="0320b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0320b-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="0320b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0320b-129">Property</span></span>|<span data-ttu-id="0320b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0320b-130">Type</span></span>|<span data-ttu-id="0320b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0320b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0320b-132">id</span><span class="sxs-lookup"><span data-stu-id="0320b-132">id</span></span>|<span data-ttu-id="0320b-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0320b-133">String</span></span>|<span data-ttu-id="0320b-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0320b-134">Key of the entity.</span></span> <span data-ttu-id="0320b-135">Geerbt von [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0320b-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0320b-136">serialNumber</span></span>|<span data-ttu-id="0320b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0320b-137">String</span></span>|<span data-ttu-id="0320b-138">Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbte Geräteseriennummer</span><span class="sxs-lookup"><span data-stu-id="0320b-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="0320b-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="0320b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0320b-140">String</span></span>|<span data-ttu-id="0320b-141">Registrierungsprofil-ID, die vom Administrator für das Gerät während der nächsten von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Registrierung angewendet werden soll</span><span class="sxs-lookup"><span data-stu-id="0320b-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="0320b-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="0320b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0320b-143">DateTimeOffset</span></span>|<span data-ttu-id="0320b-144">Das Zeit Registrierungsprofil wurde dem Gerät zugewiesen, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="0320b-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0320b-145">isSupervised</span></span>|<span data-ttu-id="0320b-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0320b-146">Boolean</span></span>|<span data-ttu-id="0320b-147">Gibt an, ob das Apple-Gerät überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="0320b-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="0320b-148">Weitere Informationen finden Sie unter https://support.apple.com/en-us/HT202837 : Inherited from [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0320b-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="0320b-149">discoverySource</span></span>|[<span data-ttu-id="0320b-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="0320b-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="0320b-151">Apple-Geräte Ermittlungs Quelle.</span><span class="sxs-lookup"><span data-stu-id="0320b-151">Apple device discovery source.</span></span> <span data-ttu-id="0320b-152">Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="0320b-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0320b-153">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="0320b-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="0320b-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0320b-154">createdDateTime</span></span>|<span data-ttu-id="0320b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0320b-155">DateTimeOffset</span></span>|<span data-ttu-id="0320b-156">ErstellungsDatum des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="0320b-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="0320b-157">lastContactedDateTime</span></span>|<span data-ttu-id="0320b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0320b-158">DateTimeOffset</span></span>|<span data-ttu-id="0320b-159">Datum der letzten Kontaktaufnahme des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="0320b-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-160">description</span><span class="sxs-lookup"><span data-stu-id="0320b-160">description</span></span>|<span data-ttu-id="0320b-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0320b-161">String</span></span>|<span data-ttu-id="0320b-162">Die Beschreibung des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="0320b-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0320b-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0320b-163">enrollmentState</span></span>|[<span data-ttu-id="0320b-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0320b-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="0320b-165">Der Status des Geräts in InTune, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="0320b-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0320b-166">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="0320b-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="0320b-167">Plattform</span><span class="sxs-lookup"><span data-stu-id="0320b-167">platform</span></span>|[<span data-ttu-id="0320b-168">Plattform</span><span class="sxs-lookup"><span data-stu-id="0320b-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="0320b-169">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0320b-169">The platform of the Device.</span></span> <span data-ttu-id="0320b-170">Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="0320b-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0320b-171">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="0320b-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="0320b-172">status</span><span class="sxs-lookup"><span data-stu-id="0320b-172">status</span></span>|<span data-ttu-id="0320b-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0320b-173">Boolean</span></span>|<span data-ttu-id="0320b-174">Status der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="0320b-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="0320b-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="0320b-175">Response</span></span>
<span data-ttu-id="0320b-176">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0320b-176">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0320b-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0320b-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="0320b-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0320b-178">Request</span></span>
<span data-ttu-id="0320b-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0320b-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0320b-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="0320b-180">Response</span></span>
<span data-ttu-id="0320b-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0320b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




