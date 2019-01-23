---
title: Erstellen von azureADWindowsAutopilotDeploymentProfile
description: Erstellen eines neuen AzureADWindowsAutopilotDeploymentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62b73c9041477a5aa103e08ce952c5d713bed83b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398828"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="6f74b-103">Erstellen von azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="6f74b-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="6f74b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6f74b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f74b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f74b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f74b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f74b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f74b-107">Erstellen eines neuen [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f74b-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f74b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f74b-108">Prerequisites</span></span>
<span data-ttu-id="6f74b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f74b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f74b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f74b-111">Permission type</span></span>|<span data-ttu-id="6f74b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f74b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f74b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f74b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f74b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f74b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f74b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f74b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f74b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f74b-116">Not supported.</span></span>|
|<span data-ttu-id="6f74b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f74b-117">Application</span></span>|<span data-ttu-id="6f74b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f74b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f74b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f74b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6f74b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f74b-120">Request headers</span></span>
|<span data-ttu-id="6f74b-121">Header</span><span class="sxs-lookup"><span data-stu-id="6f74b-121">Header</span></span>|<span data-ttu-id="6f74b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6f74b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f74b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6f74b-123">Authorization</span></span>|<span data-ttu-id="6f74b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f74b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f74b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f74b-125">Accept</span></span>|<span data-ttu-id="6f74b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f74b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f74b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f74b-127">Request body</span></span>
<span data-ttu-id="6f74b-128">Geben Sie im Textkörper Anforderung für das Objekt AzureADWindowsAutopilotDeploymentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6f74b-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="6f74b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AzureADWindowsAutopilotDeploymentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="6f74b-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="6f74b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f74b-130">Property</span></span>|<span data-ttu-id="6f74b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6f74b-131">Type</span></span>|<span data-ttu-id="6f74b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f74b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f74b-133">id</span><span class="sxs-lookup"><span data-stu-id="6f74b-133">id</span></span>|<span data-ttu-id="6f74b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f74b-134">String</span></span>|<span data-ttu-id="6f74b-135">Profil Schlüssel von [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="6f74b-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6f74b-136">displayName</span></span>|<span data-ttu-id="6f74b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f74b-137">String</span></span>|<span data-ttu-id="6f74b-138">Name des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f74b-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-139">description</span><span class="sxs-lookup"><span data-stu-id="6f74b-139">description</span></span>|<span data-ttu-id="6f74b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f74b-140">String</span></span>|<span data-ttu-id="6f74b-141">Beschreibung des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f74b-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-142">language</span><span class="sxs-lookup"><span data-stu-id="6f74b-142">language</span></span>|<span data-ttu-id="6f74b-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f74b-143">String</span></span>|<span data-ttu-id="6f74b-144">Auf dem Gerät Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) konfigurierten Sprache</span><span class="sxs-lookup"><span data-stu-id="6f74b-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f74b-145">createdDateTime</span></span>|<span data-ttu-id="6f74b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f74b-146">DateTimeOffset</span></span>|<span data-ttu-id="6f74b-147">Profil Erstellungszeit Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f74b-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f74b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6f74b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f74b-149">DateTimeOffset</span></span>|<span data-ttu-id="6f74b-150">Profil Zeitpunkt der letzten Änderung Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f74b-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="6f74b-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="6f74b-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="6f74b-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="6f74b-153">Out of Box experience Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen</span><span class="sxs-lookup"><span data-stu-id="6f74b-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="6f74b-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="6f74b-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="6f74b-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="6f74b-156">Registrierung Statusfenster Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen</span><span class="sxs-lookup"><span data-stu-id="6f74b-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="6f74b-157">extractHardwareHash</span></span>|<span data-ttu-id="6f74b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f74b-158">Boolean</span></span>|<span data-ttu-id="6f74b-159">Extraktion von HardwareHash für das Profil Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f74b-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="6f74b-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="6f74b-160">deviceNameTemplate</span></span>|<span data-ttu-id="6f74b-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f74b-161">String</span></span>|<span data-ttu-id="6f74b-162">Die Vorlage verwendet, um das Gerät AutoPilot nennen.</span><span class="sxs-lookup"><span data-stu-id="6f74b-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="6f74b-163">Dies kann ein benutzerdefinierter Text und kann auch die Seriennummer des Geräts, oder aber eine zufällig erzeugte Zahl enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f74b-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="6f74b-164">Die gesamte Länge des Texts von der Vorlage generierte kann nicht mehr als 15 Zeichen sein.</span><span class="sxs-lookup"><span data-stu-id="6f74b-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="6f74b-165">Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6f74b-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6f74b-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f74b-166">Response</span></span>
<span data-ttu-id="6f74b-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6f74b-167">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f74b-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f74b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f74b-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f74b-169">Request</span></span>
<span data-ttu-id="6f74b-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f74b-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1036

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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="6f74b-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f74b-171">Response</span></span>
<span data-ttu-id="6f74b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f74b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




