---
title: ImportedAppleDeviceIdentity aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedAppleDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 53f80608d2236b1afe6d7f9f80c5e4816d76ec50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990985"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="50536-103">ImportedAppleDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="50536-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="50536-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50536-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50536-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50536-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50536-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50536-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50536-107">Aktualisieren Sie die Eigenschaften eines [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50536-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50536-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50536-108">Prerequisites</span></span>
<span data-ttu-id="50536-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50536-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50536-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50536-111">Permission type</span></span>|<span data-ttu-id="50536-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50536-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50536-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50536-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50536-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50536-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50536-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50536-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50536-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50536-116">Not supported.</span></span>|
|<span data-ttu-id="50536-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50536-117">Application</span></span>|<span data-ttu-id="50536-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50536-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50536-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50536-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="50536-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50536-120">Request headers</span></span>
|<span data-ttu-id="50536-121">Header</span><span class="sxs-lookup"><span data-stu-id="50536-121">Header</span></span>|<span data-ttu-id="50536-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50536-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50536-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50536-123">Authorization</span></span>|<span data-ttu-id="50536-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50536-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50536-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50536-125">Accept</span></span>|<span data-ttu-id="50536-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50536-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50536-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50536-127">Request body</span></span>
<span data-ttu-id="50536-128">Geben Sie im Textkörper Anforderung für das Objekt [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="50536-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="50536-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="50536-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="50536-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50536-130">Property</span></span>|<span data-ttu-id="50536-131">Typ</span><span class="sxs-lookup"><span data-stu-id="50536-131">Type</span></span>|<span data-ttu-id="50536-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50536-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50536-133">id</span><span class="sxs-lookup"><span data-stu-id="50536-133">id</span></span>|<span data-ttu-id="50536-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50536-134">String</span></span>|<span data-ttu-id="50536-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="50536-135">Key of the entity.</span></span>|
|<span data-ttu-id="50536-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="50536-136">serialNumber</span></span>|<span data-ttu-id="50536-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50536-137">String</span></span>|<span data-ttu-id="50536-138">Seriennummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="50536-138">Device serial number</span></span>|
|<span data-ttu-id="50536-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="50536-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="50536-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50536-140">String</span></span>|<span data-ttu-id="50536-141">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung anwenden</span><span class="sxs-lookup"><span data-stu-id="50536-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="50536-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="50536-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="50536-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50536-143">DateTimeOffset</span></span>|<span data-ttu-id="50536-144">Das Zeit Registrierung Profil zugewiesen wurde das Gerät</span><span class="sxs-lookup"><span data-stu-id="50536-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="50536-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="50536-145">isSupervised</span></span>|<span data-ttu-id="50536-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="50536-146">Boolean</span></span>|<span data-ttu-id="50536-147">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="50536-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="50536-148">Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="50536-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="50536-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="50536-149">discoverySource</span></span>|[<span data-ttu-id="50536-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="50536-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="50536-151">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="50536-151">Apple device discovery source.</span></span> <span data-ttu-id="50536-152">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="50536-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="50536-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50536-153">createdDateTime</span></span>|<span data-ttu-id="50536-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50536-154">DateTimeOffset</span></span>|<span data-ttu-id="50536-155">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="50536-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="50536-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="50536-156">lastContactedDateTime</span></span>|<span data-ttu-id="50536-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50536-157">DateTimeOffset</span></span>|<span data-ttu-id="50536-158">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="50536-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="50536-159">description</span><span class="sxs-lookup"><span data-stu-id="50536-159">description</span></span>|<span data-ttu-id="50536-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50536-160">String</span></span>|<span data-ttu-id="50536-161">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="50536-161">The description of the device</span></span>|
|<span data-ttu-id="50536-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="50536-162">enrollmentState</span></span>|[<span data-ttu-id="50536-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="50536-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="50536-164">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="50536-164">The state of the device in Intune.</span></span> <span data-ttu-id="50536-165">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="50536-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="50536-166">Plattform</span><span class="sxs-lookup"><span data-stu-id="50536-166">platform</span></span>|[<span data-ttu-id="50536-167">Plattform</span><span class="sxs-lookup"><span data-stu-id="50536-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="50536-168">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="50536-168">The platform of the Device.</span></span> <span data-ttu-id="50536-169">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="50536-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="50536-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="50536-170">Response</span></span>
<span data-ttu-id="50536-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="50536-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50536-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50536-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="50536-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50536-173">Request</span></span>
<span data-ttu-id="50536-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50536-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 431

{
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

### <a name="response"></a><span data-ttu-id="50536-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="50536-175">Response</span></span>
<span data-ttu-id="50536-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50536-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





