---
title: Importappledeviceidentitylist aktualisieren
description: Aktualisieren der Eigenschaften eines Importappledeviceidentitylist-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34a48f5e55e2999650bb4034ccfa27eefdc236de
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977415"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="5a46c-103">Importappledeviceidentitylist aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5a46c-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="5a46c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a46c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a46c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5a46c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a46c-106">Aktualisieren der Eigenschaften eines [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a46c-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a46c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a46c-107">Prerequisites</span></span>
<span data-ttu-id="5a46c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a46c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a46c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a46c-110">Permission type</span></span>|<span data-ttu-id="5a46c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a46c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a46c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a46c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a46c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a46c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5a46c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a46c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a46c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a46c-115">Not supported.</span></span>|
|<span data-ttu-id="5a46c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a46c-116">Application</span></span>|<span data-ttu-id="5a46c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a46c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a46c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a46c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="5a46c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a46c-119">Request headers</span></span>
|<span data-ttu-id="5a46c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a46c-120">Header</span></span>|<span data-ttu-id="5a46c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5a46c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a46c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a46c-122">Authorization</span></span>|<span data-ttu-id="5a46c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a46c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a46c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a46c-124">Accept</span></span>|<span data-ttu-id="5a46c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a46c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a46c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a46c-126">Request body</span></span>
<span data-ttu-id="5a46c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="5a46c-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="5a46c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5a46c-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="5a46c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a46c-129">Property</span></span>|<span data-ttu-id="5a46c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5a46c-130">Type</span></span>|<span data-ttu-id="5a46c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a46c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a46c-132">id</span><span class="sxs-lookup"><span data-stu-id="5a46c-132">id</span></span>|<span data-ttu-id="5a46c-133">String</span><span class="sxs-lookup"><span data-stu-id="5a46c-133">String</span></span>|<span data-ttu-id="5a46c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5a46c-134">Key of the entity.</span></span>|
|<span data-ttu-id="5a46c-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5a46c-135">serialNumber</span></span>|<span data-ttu-id="5a46c-136">String</span><span class="sxs-lookup"><span data-stu-id="5a46c-136">String</span></span>|<span data-ttu-id="5a46c-137">Seriennummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="5a46c-137">Device serial number</span></span>|
|<span data-ttu-id="5a46c-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="5a46c-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="5a46c-139">String</span><span class="sxs-lookup"><span data-stu-id="5a46c-139">String</span></span>|<span data-ttu-id="5a46c-140">Registrierungsprofil-ID, die der Administrator während der nächsten Registrierung auf das Gerät anwenden soll</span><span class="sxs-lookup"><span data-stu-id="5a46c-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="5a46c-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="5a46c-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="5a46c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a46c-142">DateTimeOffset</span></span>|<span data-ttu-id="5a46c-143">Das Zeit Registrierungsprofil wurde dem Gerät zugewiesen</span><span class="sxs-lookup"><span data-stu-id="5a46c-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="5a46c-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5a46c-144">isSupervised</span></span>|<span data-ttu-id="5a46c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a46c-145">Boolean</span></span>|<span data-ttu-id="5a46c-146">Gibt an, ob das Apple-Gerät überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="5a46c-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="5a46c-147">Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="5a46c-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="5a46c-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5a46c-148">discoverySource</span></span>|[<span data-ttu-id="5a46c-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5a46c-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="5a46c-150">Apple-Geräte Ermittlungs Quelle.</span><span class="sxs-lookup"><span data-stu-id="5a46c-150">Apple device discovery source.</span></span> <span data-ttu-id="5a46c-151">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="5a46c-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="5a46c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a46c-152">createdDateTime</span></span>|<span data-ttu-id="5a46c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a46c-153">DateTimeOffset</span></span>|<span data-ttu-id="5a46c-154">ErstellungsDatum des Geräts</span><span class="sxs-lookup"><span data-stu-id="5a46c-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="5a46c-155">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a46c-155">lastContactedDateTime</span></span>|<span data-ttu-id="5a46c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a46c-156">DateTimeOffset</span></span>|<span data-ttu-id="5a46c-157">Datum der letzten Kontaktaufnahme des Geräts</span><span class="sxs-lookup"><span data-stu-id="5a46c-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="5a46c-158">description</span><span class="sxs-lookup"><span data-stu-id="5a46c-158">description</span></span>|<span data-ttu-id="5a46c-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a46c-159">String</span></span>|<span data-ttu-id="5a46c-160">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="5a46c-160">The description of the device</span></span>|
|<span data-ttu-id="5a46c-161">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5a46c-161">enrollmentState</span></span>|[<span data-ttu-id="5a46c-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5a46c-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="5a46c-163">Der Status des Geräts in InTune.</span><span class="sxs-lookup"><span data-stu-id="5a46c-163">The state of the device in Intune.</span></span> <span data-ttu-id="5a46c-164">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5a46c-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5a46c-165">Plattform</span><span class="sxs-lookup"><span data-stu-id="5a46c-165">platform</span></span>|[<span data-ttu-id="5a46c-166">Plattform</span><span class="sxs-lookup"><span data-stu-id="5a46c-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5a46c-167">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="5a46c-167">The platform of the Device.</span></span> <span data-ttu-id="5a46c-168">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="5a46c-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="5a46c-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a46c-169">Response</span></span>
<span data-ttu-id="5a46c-170">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5a46c-170">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a46c-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a46c-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a46c-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a46c-172">Request</span></span>
<span data-ttu-id="5a46c-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a46c-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="5a46c-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a46c-174">Response</span></span>
<span data-ttu-id="5a46c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a46c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




