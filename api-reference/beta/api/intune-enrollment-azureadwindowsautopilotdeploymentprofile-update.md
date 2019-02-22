---
title: AzureADWindowsAutopilotDeploymentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines azureADWindowsAutopilotDeploymentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1c7d8ca7fec97d687bc359bd9137ef368ce585f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144275"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="26ce4-103">AzureADWindowsAutopilotDeploymentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="26ce4-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="26ce4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26ce4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26ce4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="26ce4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ce4-106">Aktualisieren der Eigenschaften eines [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="26ce4-106">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26ce4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="26ce4-107">Prerequisites</span></span>
<span data-ttu-id="26ce4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="26ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="26ce4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26ce4-110">Permission type</span></span>|<span data-ttu-id="26ce4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26ce4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26ce4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26ce4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26ce4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ce4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26ce4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26ce4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26ce4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26ce4-115">Not supported.</span></span>|
|<span data-ttu-id="26ce4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26ce4-116">Application</span></span>|<span data-ttu-id="26ce4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26ce4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26ce4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26ce4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="26ce4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26ce4-119">Request headers</span></span>
|<span data-ttu-id="26ce4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="26ce4-120">Header</span></span>|<span data-ttu-id="26ce4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="26ce4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26ce4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26ce4-122">Authorization</span></span>|<span data-ttu-id="26ce4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="26ce4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26ce4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="26ce4-124">Accept</span></span>|<span data-ttu-id="26ce4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26ce4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26ce4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26ce4-126">Request body</span></span>
<span data-ttu-id="26ce4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="26ce4-127">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="26ce4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="26ce4-128">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="26ce4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26ce4-129">Property</span></span>|<span data-ttu-id="26ce4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="26ce4-130">Type</span></span>|<span data-ttu-id="26ce4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26ce4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ce4-132">id</span><span class="sxs-lookup"><span data-stu-id="26ce4-132">id</span></span>|<span data-ttu-id="26ce4-133">string</span><span class="sxs-lookup"><span data-stu-id="26ce4-133">String</span></span>|<span data-ttu-id="26ce4-134">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbter Profilschlüssel</span><span class="sxs-lookup"><span data-stu-id="26ce4-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="26ce4-135">displayName</span></span>|<span data-ttu-id="26ce4-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26ce4-136">String</span></span>|<span data-ttu-id="26ce4-137">Name des von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="26ce4-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-138">description</span><span class="sxs-lookup"><span data-stu-id="26ce4-138">description</span></span>|<span data-ttu-id="26ce4-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26ce4-139">String</span></span>|<span data-ttu-id="26ce4-140">Beschreibung des von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="26ce4-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-141">language</span><span class="sxs-lookup"><span data-stu-id="26ce4-141">language</span></span>|<span data-ttu-id="26ce4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26ce4-142">String</span></span>|<span data-ttu-id="26ce4-143">Sprache, die auf dem von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Gerät konfiguriert ist</span><span class="sxs-lookup"><span data-stu-id="26ce4-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26ce4-144">createdDateTime</span></span>|<span data-ttu-id="26ce4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26ce4-145">DateTimeOffset</span></span>|<span data-ttu-id="26ce4-146">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profil Erstellungszeit</span><span class="sxs-lookup"><span data-stu-id="26ce4-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26ce4-147">lastModifiedDateTime</span></span>|<span data-ttu-id="26ce4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26ce4-148">DateTimeOffset</span></span>|<span data-ttu-id="26ce4-149">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profile der letzten Änderung</span><span class="sxs-lookup"><span data-stu-id="26ce4-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="26ce4-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="26ce4-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="26ce4-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="26ce4-152">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Einstellung für die Out-of-Box-Umgebung</span><span class="sxs-lookup"><span data-stu-id="26ce4-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="26ce4-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="26ce4-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="26ce4-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="26ce4-155">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Einstellung für den Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="26ce4-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="26ce4-156">extractHardwareHash</span></span>|<span data-ttu-id="26ce4-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="26ce4-157">Boolean</span></span>|<span data-ttu-id="26ce4-158">HardwareHash-Extraktion für das von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profil</span><span class="sxs-lookup"><span data-stu-id="26ce4-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="26ce4-159">deviceNameTemplate</span></span>|<span data-ttu-id="26ce4-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26ce4-160">String</span></span>|<span data-ttu-id="26ce4-161">Die Vorlage, die zum Benennen des autoPilot-Geräts verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="26ce4-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="26ce4-162">Dabei kann es sich um einen benutzerdefinierten Text handeln, der entweder die Seriennummer des Geräts oder eine zufällig generierte Zahl enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="26ce4-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="26ce4-163">Die Gesamtlänge des von der Vorlage generierten Texts darf nicht mehr als 15 Zeichen betragen.</span><span class="sxs-lookup"><span data-stu-id="26ce4-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="26ce4-164">Geerbt von [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="26ce4-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="26ce4-165">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="26ce4-165">enableWhiteGlove</span></span>|<span data-ttu-id="26ce4-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="26ce4-166">Boolean</span></span>|<span data-ttu-id="26ce4-167">Aktivieren Sie den weißen Handschuh Autopilot für das Profil.</span><span class="sxs-lookup"><span data-stu-id="26ce4-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="26ce4-168">Geerbt von [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="26ce4-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="26ce4-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="26ce4-169">Response</span></span>
<span data-ttu-id="26ce4-170">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="26ce4-170">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26ce4-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26ce4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="26ce4-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26ce4-172">Request</span></span>
<span data-ttu-id="26ce4-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26ce4-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1065

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="26ce4-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="26ce4-174">Response</span></span>
<span data-ttu-id="26ce4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26ce4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1237

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "enableWhiteGlove": true
}
```




