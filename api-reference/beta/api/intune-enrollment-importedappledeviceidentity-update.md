---
title: ImportedAppleDeviceIdentity aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedAppleDeviceIdentity-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7970c0c74c7200d6a991a48f986125747589195c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412170"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="1e306-103">ImportedAppleDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1e306-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="1e306-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1e306-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1e306-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e306-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e306-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e306-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e306-107">Aktualisieren Sie die Eigenschaften eines [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1e306-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e306-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e306-108">Prerequisites</span></span>
<span data-ttu-id="1e306-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e306-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1e306-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e306-111">Permission type</span></span>|<span data-ttu-id="1e306-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e306-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e306-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e306-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e306-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e306-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e306-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e306-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e306-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e306-116">Not supported.</span></span>|
|<span data-ttu-id="1e306-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e306-117">Application</span></span>|<span data-ttu-id="1e306-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e306-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e306-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e306-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="1e306-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e306-120">Request headers</span></span>
|<span data-ttu-id="1e306-121">Header</span><span class="sxs-lookup"><span data-stu-id="1e306-121">Header</span></span>|<span data-ttu-id="1e306-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1e306-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e306-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1e306-123">Authorization</span></span>|<span data-ttu-id="1e306-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e306-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e306-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1e306-125">Accept</span></span>|<span data-ttu-id="1e306-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e306-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e306-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e306-127">Request body</span></span>
<span data-ttu-id="1e306-128">Geben Sie im Textkörper Anforderung für das Objekt [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1e306-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="1e306-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1e306-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="1e306-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e306-130">Property</span></span>|<span data-ttu-id="1e306-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1e306-131">Type</span></span>|<span data-ttu-id="1e306-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e306-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e306-133">id</span><span class="sxs-lookup"><span data-stu-id="1e306-133">id</span></span>|<span data-ttu-id="1e306-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e306-134">String</span></span>|<span data-ttu-id="1e306-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1e306-135">Key of the entity.</span></span>|
|<span data-ttu-id="1e306-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1e306-136">serialNumber</span></span>|<span data-ttu-id="1e306-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e306-137">String</span></span>|<span data-ttu-id="1e306-138">Seriennummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="1e306-138">Device serial number</span></span>|
|<span data-ttu-id="1e306-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="1e306-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="1e306-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e306-140">String</span></span>|<span data-ttu-id="1e306-141">Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung anwenden</span><span class="sxs-lookup"><span data-stu-id="1e306-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="1e306-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="1e306-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="1e306-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e306-143">DateTimeOffset</span></span>|<span data-ttu-id="1e306-144">Das Zeit Registrierung Profil zugewiesen wurde das Gerät</span><span class="sxs-lookup"><span data-stu-id="1e306-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="1e306-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1e306-145">isSupervised</span></span>|<span data-ttu-id="1e306-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e306-146">Boolean</span></span>|<span data-ttu-id="1e306-147">Gibt an, ob das Gerät Apple überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="1e306-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="1e306-148">Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="1e306-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="1e306-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1e306-149">discoverySource</span></span>|[<span data-ttu-id="1e306-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1e306-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="1e306-151">Apple Gerät Discovery-Quelle.</span><span class="sxs-lookup"><span data-stu-id="1e306-151">Apple device discovery source.</span></span> <span data-ttu-id="1e306-152">Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="1e306-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="1e306-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e306-153">createdDateTime</span></span>|<span data-ttu-id="1e306-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e306-154">DateTimeOffset</span></span>|<span data-ttu-id="1e306-155">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="1e306-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="1e306-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e306-156">lastContactedDateTime</span></span>|<span data-ttu-id="1e306-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e306-157">DateTimeOffset</span></span>|<span data-ttu-id="1e306-158">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="1e306-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="1e306-159">description</span><span class="sxs-lookup"><span data-stu-id="1e306-159">description</span></span>|<span data-ttu-id="1e306-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e306-160">String</span></span>|<span data-ttu-id="1e306-161">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="1e306-161">The description of the device</span></span>|
|<span data-ttu-id="1e306-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1e306-162">enrollmentState</span></span>|[<span data-ttu-id="1e306-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1e306-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="1e306-164">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="1e306-164">The state of the device in Intune.</span></span> <span data-ttu-id="1e306-165">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1e306-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1e306-166">Plattform</span><span class="sxs-lookup"><span data-stu-id="1e306-166">platform</span></span>|[<span data-ttu-id="1e306-167">Plattform</span><span class="sxs-lookup"><span data-stu-id="1e306-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1e306-168">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="1e306-168">The platform of the Device.</span></span> <span data-ttu-id="1e306-169">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="1e306-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="1e306-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e306-170">Response</span></span>
<span data-ttu-id="1e306-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1e306-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e306-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e306-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e306-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e306-173">Request</span></span>
<span data-ttu-id="1e306-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e306-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e306-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e306-175">Response</span></span>
<span data-ttu-id="1e306-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e306-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




