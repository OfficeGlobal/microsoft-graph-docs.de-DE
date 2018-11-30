---
title: Erstellen von activeDirectoryWindowsAutopilotDeploymentProfile
description: Erstellen eines neuen ActiveDirectoryWindowsAutopilotDeploymentProfile-Objekts.
ms.openlocfilehash: f5f0bca53cd45d060c8a2619ffd4b851a106e59b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060747"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="3a724-103">Erstellen von activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="3a724-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="3a724-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3a724-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a724-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a724-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a724-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3a724-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a724-107">Erstellen eines neuen [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3a724-107">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a724-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3a724-108">Prerequisites</span></span>
<span data-ttu-id="3a724-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a724-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a724-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a724-111">Permission type</span></span>|<span data-ttu-id="3a724-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a724-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a724-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a724-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a724-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a724-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a724-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a724-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a724-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a724-116">Not supported.</span></span>|
|<span data-ttu-id="3a724-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a724-117">Application</span></span>|<span data-ttu-id="3a724-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a724-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a724-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a724-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3a724-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a724-120">Request headers</span></span>
|<span data-ttu-id="3a724-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3a724-121">Header</span></span>|<span data-ttu-id="3a724-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3a724-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a724-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a724-123">Authorization</span></span>|<span data-ttu-id="3a724-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3a724-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a724-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a724-125">Accept</span></span>|<span data-ttu-id="3a724-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a724-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a724-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a724-127">Request body</span></span>
<span data-ttu-id="3a724-128">Geben Sie im Textkörper Anforderung für das Objekt ActiveDirectoryWindowsAutopilotDeploymentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3a724-128">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="3a724-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ActiveDirectoryWindowsAutopilotDeploymentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="3a724-129">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="3a724-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a724-130">Property</span></span>|<span data-ttu-id="3a724-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3a724-131">Type</span></span>|<span data-ttu-id="3a724-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a724-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a724-133">id</span><span class="sxs-lookup"><span data-stu-id="3a724-133">id</span></span>|<span data-ttu-id="3a724-134">String</span><span class="sxs-lookup"><span data-stu-id="3a724-134">String</span></span>|<span data-ttu-id="3a724-135">Profil Schlüssel von [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="3a724-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3a724-136">displayName</span></span>|<span data-ttu-id="3a724-137">String</span><span class="sxs-lookup"><span data-stu-id="3a724-137">String</span></span>|<span data-ttu-id="3a724-138">Name des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3a724-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-139">description</span><span class="sxs-lookup"><span data-stu-id="3a724-139">description</span></span>|<span data-ttu-id="3a724-140">String</span><span class="sxs-lookup"><span data-stu-id="3a724-140">String</span></span>|<span data-ttu-id="3a724-141">Beschreibung des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3a724-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-142">language</span><span class="sxs-lookup"><span data-stu-id="3a724-142">language</span></span>|<span data-ttu-id="3a724-143">String</span><span class="sxs-lookup"><span data-stu-id="3a724-143">String</span></span>|<span data-ttu-id="3a724-144">Auf dem Gerät Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) konfigurierten Sprache</span><span class="sxs-lookup"><span data-stu-id="3a724-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a724-145">createdDateTime</span></span>|<span data-ttu-id="3a724-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a724-146">DateTimeOffset</span></span>|<span data-ttu-id="3a724-147">Profil Erstellungszeit Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3a724-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a724-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3a724-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a724-149">DateTimeOffset</span></span>|<span data-ttu-id="3a724-150">Profil Zeitpunkt der letzten Änderung Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3a724-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3a724-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="3a724-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3a724-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="3a724-153">Out of Box experience Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen</span><span class="sxs-lookup"><span data-stu-id="3a724-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="3a724-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="3a724-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="3a724-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="3a724-156">Registrierung Statusfenster Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen</span><span class="sxs-lookup"><span data-stu-id="3a724-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="3a724-157">extractHardwareHash</span></span>|<span data-ttu-id="3a724-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3a724-158">Boolean</span></span>|<span data-ttu-id="3a724-159">Extraktion von HardwareHash für das Profil Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3a724-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="3a724-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="3a724-160">deviceNameTemplate</span></span>|<span data-ttu-id="3a724-161">String</span><span class="sxs-lookup"><span data-stu-id="3a724-161">String</span></span>|<span data-ttu-id="3a724-162">Die Vorlage verwendet, um das Gerät AutoPilot nennen.</span><span class="sxs-lookup"><span data-stu-id="3a724-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="3a724-163">Dies kann ein benutzerdefinierter Text und kann auch die Seriennummer des Geräts, oder aber eine zufällig erzeugte Zahl enthalten.</span><span class="sxs-lookup"><span data-stu-id="3a724-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="3a724-164">Die gesamte Länge des Texts von der Vorlage generierte kann nicht mehr als 15 Zeichen sein.</span><span class="sxs-lookup"><span data-stu-id="3a724-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="3a724-165">Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3a724-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3a724-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a724-166">Response</span></span>
<span data-ttu-id="3a724-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3a724-167">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a724-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a724-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a724-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a724-169">Request</span></span>
<span data-ttu-id="3a724-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a724-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1108

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="3a724-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a724-171">Response</span></span>
<span data-ttu-id="3a724-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a724-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1216

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
  "deviceNameTemplate": "Device Name Template value"
}
```





