---
title: ActiveDirectoryWindowsAutopilotDeploymentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines activeDirectoryWindowsAutopilotDeploymentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e76fc466195989c82728bf1bba972e876c9ef186
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160060"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="997dd-103">ActiveDirectoryWindowsAutopilotDeploymentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="997dd-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="997dd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="997dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="997dd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="997dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="997dd-106">Aktualisieren der Eigenschaften eines [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="997dd-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="997dd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="997dd-107">Prerequisites</span></span>
<span data-ttu-id="997dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="997dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="997dd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="997dd-110">Permission type</span></span>|<span data-ttu-id="997dd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="997dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="997dd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="997dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="997dd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997dd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="997dd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="997dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="997dd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="997dd-115">Not supported.</span></span>|
|<span data-ttu-id="997dd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="997dd-116">Application</span></span>|<span data-ttu-id="997dd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="997dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="997dd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="997dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="997dd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="997dd-119">Request headers</span></span>
|<span data-ttu-id="997dd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="997dd-120">Header</span></span>|<span data-ttu-id="997dd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="997dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="997dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="997dd-122">Authorization</span></span>|<span data-ttu-id="997dd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="997dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="997dd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="997dd-124">Accept</span></span>|<span data-ttu-id="997dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="997dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="997dd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="997dd-126">Request body</span></span>
<span data-ttu-id="997dd-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="997dd-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="997dd-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="997dd-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="997dd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="997dd-129">Property</span></span>|<span data-ttu-id="997dd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="997dd-130">Type</span></span>|<span data-ttu-id="997dd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="997dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="997dd-132">id</span><span class="sxs-lookup"><span data-stu-id="997dd-132">id</span></span>|<span data-ttu-id="997dd-133">string</span><span class="sxs-lookup"><span data-stu-id="997dd-133">String</span></span>|<span data-ttu-id="997dd-134">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbter Profilschlüssel</span><span class="sxs-lookup"><span data-stu-id="997dd-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="997dd-135">displayName</span></span>|<span data-ttu-id="997dd-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="997dd-136">String</span></span>|<span data-ttu-id="997dd-137">Name des von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="997dd-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-138">description</span><span class="sxs-lookup"><span data-stu-id="997dd-138">description</span></span>|<span data-ttu-id="997dd-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="997dd-139">String</span></span>|<span data-ttu-id="997dd-140">Beschreibung des von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="997dd-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-141">language</span><span class="sxs-lookup"><span data-stu-id="997dd-141">language</span></span>|<span data-ttu-id="997dd-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="997dd-142">String</span></span>|<span data-ttu-id="997dd-143">Sprache, die auf dem von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Gerät konfiguriert ist</span><span class="sxs-lookup"><span data-stu-id="997dd-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="997dd-144">createdDateTime</span></span>|<span data-ttu-id="997dd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="997dd-145">DateTimeOffset</span></span>|<span data-ttu-id="997dd-146">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profil Erstellungszeit</span><span class="sxs-lookup"><span data-stu-id="997dd-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="997dd-147">lastModifiedDateTime</span></span>|<span data-ttu-id="997dd-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="997dd-148">DateTimeOffset</span></span>|<span data-ttu-id="997dd-149">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profile der letzten Änderung</span><span class="sxs-lookup"><span data-stu-id="997dd-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="997dd-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="997dd-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="997dd-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="997dd-152">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Einstellung für die Out-of-Box-Umgebung</span><span class="sxs-lookup"><span data-stu-id="997dd-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="997dd-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="997dd-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="997dd-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="997dd-155">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Einstellung für den Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="997dd-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="997dd-156">extractHardwareHash</span></span>|<span data-ttu-id="997dd-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="997dd-157">Boolean</span></span>|<span data-ttu-id="997dd-158">HardwareHash-Extraktion für das von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profil</span><span class="sxs-lookup"><span data-stu-id="997dd-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="997dd-159">deviceNameTemplate</span></span>|<span data-ttu-id="997dd-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="997dd-160">String</span></span>|<span data-ttu-id="997dd-161">Die Vorlage, die zum Benennen des autoPilot-Geräts verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="997dd-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="997dd-162">Dabei kann es sich um einen benutzerdefinierten Text handeln, der entweder die Seriennummer des Geräts oder eine zufällig generierte Zahl enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="997dd-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="997dd-163">Die Gesamtlänge des von der Vorlage generierten Texts darf nicht mehr als 15 Zeichen betragen.</span><span class="sxs-lookup"><span data-stu-id="997dd-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="997dd-164">Geerbt von [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="997dd-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="997dd-165">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="997dd-165">enableWhiteGlove</span></span>|<span data-ttu-id="997dd-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="997dd-166">Boolean</span></span>|<span data-ttu-id="997dd-167">Aktivieren Sie den weißen Handschuh Autopilot für das Profil.</span><span class="sxs-lookup"><span data-stu-id="997dd-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="997dd-168">Geerbt von [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="997dd-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="997dd-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="997dd-169">Response</span></span>
<span data-ttu-id="997dd-170">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="997dd-170">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="997dd-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="997dd-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="997dd-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="997dd-172">Request</span></span>
<span data-ttu-id="997dd-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="997dd-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1073

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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

### <a name="response"></a><span data-ttu-id="997dd-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="997dd-174">Response</span></span>
<span data-ttu-id="997dd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="997dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
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




