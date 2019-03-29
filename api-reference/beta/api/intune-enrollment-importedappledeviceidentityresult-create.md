---
title: ImportedAppleDeviceIdentityResult erstellen
description: Erstellen eines neuen importedAppleDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a03a0c982eda187c8dee2932139ca50e40535f28
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968231"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="c8f81-103">ImportedAppleDeviceIdentityResult erstellen</span><span class="sxs-lookup"><span data-stu-id="c8f81-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="c8f81-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8f81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8f81-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c8f81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8f81-106">Erstellen eines neuen [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c8f81-106">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8f81-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8f81-107">Prerequisites</span></span>
<span data-ttu-id="c8f81-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f81-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8f81-110">Permission type</span></span>|<span data-ttu-id="c8f81-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8f81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8f81-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8f81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8f81-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8f81-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c8f81-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8f81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8f81-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8f81-115">Not supported.</span></span>|
|<span data-ttu-id="c8f81-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8f81-116">Application</span></span>|<span data-ttu-id="c8f81-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8f81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8f81-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8f81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="c8f81-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8f81-119">Request headers</span></span>
|<span data-ttu-id="c8f81-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c8f81-120">Header</span></span>|<span data-ttu-id="c8f81-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c8f81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8f81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8f81-122">Authorization</span></span>|<span data-ttu-id="c8f81-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8f81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8f81-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8f81-124">Accept</span></span>|<span data-ttu-id="c8f81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8f81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f81-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8f81-126">Request body</span></span>
<span data-ttu-id="c8f81-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das importedAppleDeviceIdentityResult-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c8f81-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="c8f81-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedAppleDeviceIdentityResult erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c8f81-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="c8f81-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8f81-129">Property</span></span>|<span data-ttu-id="c8f81-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c8f81-130">Type</span></span>|<span data-ttu-id="c8f81-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8f81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8f81-132">id</span><span class="sxs-lookup"><span data-stu-id="c8f81-132">id</span></span>|<span data-ttu-id="c8f81-133">String</span><span class="sxs-lookup"><span data-stu-id="c8f81-133">String</span></span>|<span data-ttu-id="c8f81-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c8f81-134">Key of the entity.</span></span> <span data-ttu-id="c8f81-135">Geerbt von [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c8f81-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c8f81-136">serialNumber</span></span>|<span data-ttu-id="c8f81-137">String</span><span class="sxs-lookup"><span data-stu-id="c8f81-137">String</span></span>|<span data-ttu-id="c8f81-138">Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbte Geräteseriennummer</span><span class="sxs-lookup"><span data-stu-id="c8f81-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="c8f81-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="c8f81-140">String</span><span class="sxs-lookup"><span data-stu-id="c8f81-140">String</span></span>|<span data-ttu-id="c8f81-141">Registrierungsprofil-ID, die vom Administrator für das Gerät während der nächsten von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Registrierung angewendet werden soll</span><span class="sxs-lookup"><span data-stu-id="c8f81-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="c8f81-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="c8f81-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8f81-143">DateTimeOffset</span></span>|<span data-ttu-id="c8f81-144">Das Zeit Registrierungsprofil wurde dem Gerät zugewiesen, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="c8f81-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c8f81-145">isSupervised</span></span>|<span data-ttu-id="c8f81-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8f81-146">Boolean</span></span>|<span data-ttu-id="c8f81-147">Gibt an, ob das Apple-Gerät überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="c8f81-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="c8f81-148">Weitere Informationen finden Sie unter https://support.apple.com/en-us/HT202837 : Inherited from [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c8f81-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c8f81-149">discoverySource</span></span>|[<span data-ttu-id="c8f81-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c8f81-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="c8f81-151">Apple-Geräte Ermittlungs Quelle.</span><span class="sxs-lookup"><span data-stu-id="c8f81-151">Apple device discovery source.</span></span> <span data-ttu-id="c8f81-152">Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c8f81-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c8f81-153">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="c8f81-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="c8f81-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8f81-154">createdDateTime</span></span>|<span data-ttu-id="c8f81-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8f81-155">DateTimeOffset</span></span>|<span data-ttu-id="c8f81-156">ErstellungsDatum des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="c8f81-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8f81-157">lastContactedDateTime</span></span>|<span data-ttu-id="c8f81-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8f81-158">DateTimeOffset</span></span>|<span data-ttu-id="c8f81-159">Datum der letzten Kontaktaufnahme des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="c8f81-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-160">description</span><span class="sxs-lookup"><span data-stu-id="c8f81-160">description</span></span>|<span data-ttu-id="c8f81-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8f81-161">String</span></span>|<span data-ttu-id="c8f81-162">Die Beschreibung des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="c8f81-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="c8f81-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c8f81-163">enrollmentState</span></span>|[<span data-ttu-id="c8f81-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c8f81-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="c8f81-165">Der Status des Geräts in InTune, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="c8f81-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c8f81-166">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="c8f81-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c8f81-167">Plattform</span><span class="sxs-lookup"><span data-stu-id="c8f81-167">platform</span></span>|[<span data-ttu-id="c8f81-168">Plattform</span><span class="sxs-lookup"><span data-stu-id="c8f81-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="c8f81-169">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="c8f81-169">The platform of the Device.</span></span> <span data-ttu-id="c8f81-170">Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c8f81-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="c8f81-171">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="c8f81-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="c8f81-172">status</span><span class="sxs-lookup"><span data-stu-id="c8f81-172">status</span></span>|<span data-ttu-id="c8f81-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c8f81-173">Boolean</span></span>|<span data-ttu-id="c8f81-174">Status der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="c8f81-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="c8f81-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8f81-175">Response</span></span>
<span data-ttu-id="c8f81-176">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c8f81-176">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f81-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8f81-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8f81-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8f81-178">Request</span></span>
<span data-ttu-id="c8f81-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8f81-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8f81-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8f81-180">Response</span></span>
<span data-ttu-id="c8f81-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8f81-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




