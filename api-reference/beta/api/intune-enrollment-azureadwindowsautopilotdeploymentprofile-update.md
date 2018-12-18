---
title: AzureADWindowsAutopilotDeploymentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AzureADWindowsAutopilotDeploymentProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: e47ef4aa80254ca7f08ef40c9bda9d43006f0d49
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315211"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="fd876-103">AzureADWindowsAutopilotDeploymentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fd876-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="fd876-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd876-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd876-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd876-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd876-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd876-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd876-107">Aktualisieren Sie die Eigenschaften eines [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fd876-107">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd876-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fd876-108">Prerequisites</span></span>
<span data-ttu-id="fd876-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd876-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd876-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd876-111">Permission type</span></span>|<span data-ttu-id="fd876-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd876-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd876-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd876-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd876-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd876-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd876-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd876-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd876-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd876-116">Not supported.</span></span>|
|<span data-ttu-id="fd876-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd876-117">Application</span></span>|<span data-ttu-id="fd876-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd876-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd876-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd876-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="fd876-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd876-120">Request headers</span></span>
|<span data-ttu-id="fd876-121">Header</span><span class="sxs-lookup"><span data-stu-id="fd876-121">Header</span></span>|<span data-ttu-id="fd876-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fd876-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd876-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fd876-123">Authorization</span></span>|<span data-ttu-id="fd876-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fd876-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd876-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd876-125">Accept</span></span>|<span data-ttu-id="fd876-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd876-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd876-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd876-127">Request body</span></span>
<span data-ttu-id="fd876-128">Geben Sie im Textkörper Anforderung für das Objekt [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fd876-128">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="fd876-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="fd876-129">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="fd876-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd876-130">Property</span></span>|<span data-ttu-id="fd876-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fd876-131">Type</span></span>|<span data-ttu-id="fd876-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd876-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd876-133">id</span><span class="sxs-lookup"><span data-stu-id="fd876-133">id</span></span>|<span data-ttu-id="fd876-134">String</span><span class="sxs-lookup"><span data-stu-id="fd876-134">String</span></span>|<span data-ttu-id="fd876-135">Profil Schlüssel von [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="fd876-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fd876-136">displayName</span></span>|<span data-ttu-id="fd876-137">String</span><span class="sxs-lookup"><span data-stu-id="fd876-137">String</span></span>|<span data-ttu-id="fd876-138">Name des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fd876-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-139">description</span><span class="sxs-lookup"><span data-stu-id="fd876-139">description</span></span>|<span data-ttu-id="fd876-140">String</span><span class="sxs-lookup"><span data-stu-id="fd876-140">String</span></span>|<span data-ttu-id="fd876-141">Beschreibung des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fd876-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-142">language</span><span class="sxs-lookup"><span data-stu-id="fd876-142">language</span></span>|<span data-ttu-id="fd876-143">String</span><span class="sxs-lookup"><span data-stu-id="fd876-143">String</span></span>|<span data-ttu-id="fd876-144">Auf dem Gerät Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) konfigurierten Sprache</span><span class="sxs-lookup"><span data-stu-id="fd876-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd876-145">createdDateTime</span></span>|<span data-ttu-id="fd876-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd876-146">DateTimeOffset</span></span>|<span data-ttu-id="fd876-147">Profil Erstellungszeit Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fd876-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd876-148">lastModifiedDateTime</span></span>|<span data-ttu-id="fd876-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd876-149">DateTimeOffset</span></span>|<span data-ttu-id="fd876-150">Profil Zeitpunkt der letzten Änderung Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fd876-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="fd876-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="fd876-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="fd876-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="fd876-153">Out of Box experience Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen</span><span class="sxs-lookup"><span data-stu-id="fd876-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="fd876-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="fd876-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="fd876-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="fd876-156">Registrierung Statusfenster Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen</span><span class="sxs-lookup"><span data-stu-id="fd876-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="fd876-157">extractHardwareHash</span></span>|<span data-ttu-id="fd876-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="fd876-158">Boolean</span></span>|<span data-ttu-id="fd876-159">Extraktion von HardwareHash für das Profil Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fd876-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="fd876-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="fd876-160">deviceNameTemplate</span></span>|<span data-ttu-id="fd876-161">String</span><span class="sxs-lookup"><span data-stu-id="fd876-161">String</span></span>|<span data-ttu-id="fd876-162">Die Vorlage verwendet, um das Gerät AutoPilot nennen.</span><span class="sxs-lookup"><span data-stu-id="fd876-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="fd876-163">Dies kann ein benutzerdefinierter Text und kann auch die Seriennummer des Geräts, oder aber eine zufällig erzeugte Zahl enthalten.</span><span class="sxs-lookup"><span data-stu-id="fd876-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="fd876-164">Die gesamte Länge des Texts von der Vorlage generierte kann nicht mehr als 15 Zeichen sein.</span><span class="sxs-lookup"><span data-stu-id="fd876-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="fd876-165">Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fd876-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fd876-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd876-166">Response</span></span>
<span data-ttu-id="fd876-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fd876-167">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd876-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd876-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd876-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd876-169">Request</span></span>
<span data-ttu-id="fd876-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd876-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1021

{
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

### <a name="response"></a><span data-ttu-id="fd876-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd876-171">Response</span></span>
<span data-ttu-id="fd876-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd876-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1208

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
  "deviceNameTemplate": "Device Name Template value"
}
```





