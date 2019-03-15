---
title: ActiveDirectoryWindowsAutopilotDeploymentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines activeDirectoryWindowsAutopilotDeploymentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 440c47438867fd178c2c0d08df50eeb0ca500e8a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571795"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="53b79-103">ActiveDirectoryWindowsAutopilotDeploymentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="53b79-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="53b79-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53b79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53b79-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53b79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53b79-106">Aktualisieren der Eigenschaften eines [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="53b79-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53b79-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53b79-107">Prerequisites</span></span>
<span data-ttu-id="53b79-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53b79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53b79-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53b79-110">Permission type</span></span>|<span data-ttu-id="53b79-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53b79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b79-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53b79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53b79-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b79-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53b79-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53b79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b79-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53b79-115">Not supported.</span></span>|
|<span data-ttu-id="53b79-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53b79-116">Application</span></span>|<span data-ttu-id="53b79-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53b79-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b79-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53b79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="53b79-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53b79-119">Request headers</span></span>
|<span data-ttu-id="53b79-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53b79-120">Header</span></span>|<span data-ttu-id="53b79-121">Wert</span><span class="sxs-lookup"><span data-stu-id="53b79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53b79-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53b79-122">Authorization</span></span>|<span data-ttu-id="53b79-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53b79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53b79-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53b79-124">Accept</span></span>|<span data-ttu-id="53b79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53b79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b79-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53b79-126">Request body</span></span>
<span data-ttu-id="53b79-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="53b79-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="53b79-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="53b79-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="53b79-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53b79-129">Property</span></span>|<span data-ttu-id="53b79-130">Typ</span><span class="sxs-lookup"><span data-stu-id="53b79-130">Type</span></span>|<span data-ttu-id="53b79-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53b79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b79-132">id</span><span class="sxs-lookup"><span data-stu-id="53b79-132">id</span></span>|<span data-ttu-id="53b79-133">String</span><span class="sxs-lookup"><span data-stu-id="53b79-133">String</span></span>|<span data-ttu-id="53b79-134">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbter Profilschlüssel</span><span class="sxs-lookup"><span data-stu-id="53b79-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-135">displayName</span><span class="sxs-lookup"><span data-stu-id="53b79-135">displayName</span></span>|<span data-ttu-id="53b79-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53b79-136">String</span></span>|<span data-ttu-id="53b79-137">Name des von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="53b79-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-138">description</span><span class="sxs-lookup"><span data-stu-id="53b79-138">description</span></span>|<span data-ttu-id="53b79-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53b79-139">String</span></span>|<span data-ttu-id="53b79-140">Beschreibung des von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="53b79-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-141">language</span><span class="sxs-lookup"><span data-stu-id="53b79-141">language</span></span>|<span data-ttu-id="53b79-142">String</span><span class="sxs-lookup"><span data-stu-id="53b79-142">String</span></span>|<span data-ttu-id="53b79-143">Sprache, die auf dem von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbten Gerät konfiguriert ist</span><span class="sxs-lookup"><span data-stu-id="53b79-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53b79-144">createdDateTime</span></span>|<span data-ttu-id="53b79-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b79-145">DateTimeOffset</span></span>|<span data-ttu-id="53b79-146">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profil Erstellungszeit</span><span class="sxs-lookup"><span data-stu-id="53b79-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53b79-147">lastModifiedDateTime</span></span>|<span data-ttu-id="53b79-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b79-148">DateTimeOffset</span></span>|<span data-ttu-id="53b79-149">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profile der letzten Änderung</span><span class="sxs-lookup"><span data-stu-id="53b79-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="53b79-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="53b79-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="53b79-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="53b79-152">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Einstellung für die Out-of-Box-Umgebung</span><span class="sxs-lookup"><span data-stu-id="53b79-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="53b79-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="53b79-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="53b79-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="53b79-155">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Einstellung für den Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="53b79-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="53b79-156">extractHardwareHash</span></span>|<span data-ttu-id="53b79-157">Boolesch</span><span class="sxs-lookup"><span data-stu-id="53b79-157">Boolean</span></span>|<span data-ttu-id="53b79-158">HardwareHash-Extraktion für das von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbte Profil</span><span class="sxs-lookup"><span data-stu-id="53b79-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="53b79-159">deviceNameTemplate</span></span>|<span data-ttu-id="53b79-160">String</span><span class="sxs-lookup"><span data-stu-id="53b79-160">String</span></span>|<span data-ttu-id="53b79-161">Die Vorlage, die zum Benennen des autoPilot-Geräts verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="53b79-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="53b79-162">Dabei kann es sich um einen benutzerdefinierten Text handeln, der entweder die Seriennummer des Geräts oder eine zufällig generierte Zahl enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="53b79-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="53b79-163">Die Gesamtlänge des von der Vorlage generierten Texts darf nicht mehr als 15 Zeichen betragen.</span><span class="sxs-lookup"><span data-stu-id="53b79-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="53b79-164">Geerbt von [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="53b79-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="53b79-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="53b79-165">deviceType</span></span>|[<span data-ttu-id="53b79-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="53b79-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="53b79-167">Der autoPilot-Gerätetyp, auf den dieses Profil angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="53b79-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="53b79-168">Von [Windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="53b79-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="53b79-169">Mögliche Werte sind: `windowsPc` und `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="53b79-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="53b79-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="53b79-170">enableWhiteGlove</span></span>|<span data-ttu-id="53b79-171">Boolesch</span><span class="sxs-lookup"><span data-stu-id="53b79-171">Boolean</span></span>|<span data-ttu-id="53b79-172">Aktivieren Sie den weißen Handschuh Autopilot für das Profil.</span><span class="sxs-lookup"><span data-stu-id="53b79-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="53b79-173">Geerbt von [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="53b79-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="53b79-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="53b79-174">Response</span></span>
<span data-ttu-id="53b79-175">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="53b79-175">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b79-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53b79-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="53b79-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53b79-177">Request</span></span>
<span data-ttu-id="53b79-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53b79-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1105

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
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="53b79-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="53b79-179">Response</span></span>
<span data-ttu-id="53b79-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53b79-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

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
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true
}
```




