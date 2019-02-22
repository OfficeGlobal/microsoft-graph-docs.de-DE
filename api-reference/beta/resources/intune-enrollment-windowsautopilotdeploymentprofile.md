---
title: Windowsautopilotdeploymentprofile hinzugefügt-Ressourcentyp
description: Windows Autopilot-BereitstellungsProfil
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3b815e0184ab9969af348338c07c3fabf0b0597
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168873"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="350ac-103">Windowsautopilotdeploymentprofile hinzugefügt-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="350ac-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="350ac-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="350ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="350ac-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="350ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="350ac-106">Windows Autopilot-BereitstellungsProfil</span><span class="sxs-lookup"><span data-stu-id="350ac-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="350ac-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="350ac-107">Methods</span></span>
|<span data-ttu-id="350ac-108">Methode</span><span class="sxs-lookup"><span data-stu-id="350ac-108">Method</span></span>|<span data-ttu-id="350ac-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="350ac-109">Return Type</span></span>|<span data-ttu-id="350ac-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="350ac-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="350ac-111">Windowsautopilotdeploymentprofile hinzugefügt abrufen</span><span class="sxs-lookup"><span data-stu-id="350ac-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="350ac-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="350ac-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="350ac-113">Lesen von Eigenschaften und Beziehungen des [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="350ac-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="350ac-114">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="350ac-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="350ac-115">Keine</span><span class="sxs-lookup"><span data-stu-id="350ac-115">None</span></span>|<span data-ttu-id="350ac-116">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="350ac-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="350ac-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="350ac-117">Properties</span></span>
|<span data-ttu-id="350ac-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="350ac-118">Property</span></span>|<span data-ttu-id="350ac-119">Typ</span><span class="sxs-lookup"><span data-stu-id="350ac-119">Type</span></span>|<span data-ttu-id="350ac-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="350ac-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="350ac-121">id</span><span class="sxs-lookup"><span data-stu-id="350ac-121">id</span></span>|<span data-ttu-id="350ac-122">string</span><span class="sxs-lookup"><span data-stu-id="350ac-122">String</span></span>|<span data-ttu-id="350ac-123">Profilschlüssel</span><span class="sxs-lookup"><span data-stu-id="350ac-123">Profile Key</span></span>|
|<span data-ttu-id="350ac-124">displayName</span><span class="sxs-lookup"><span data-stu-id="350ac-124">displayName</span></span>|<span data-ttu-id="350ac-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="350ac-125">String</span></span>|<span data-ttu-id="350ac-126">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="350ac-126">Name of the profile</span></span>|
|<span data-ttu-id="350ac-127">description</span><span class="sxs-lookup"><span data-stu-id="350ac-127">description</span></span>|<span data-ttu-id="350ac-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="350ac-128">String</span></span>|<span data-ttu-id="350ac-129">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="350ac-129">Description of the profile</span></span>|
|<span data-ttu-id="350ac-130">language</span><span class="sxs-lookup"><span data-stu-id="350ac-130">language</span></span>|<span data-ttu-id="350ac-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="350ac-131">String</span></span>|<span data-ttu-id="350ac-132">Auf dem Gerät konfigurierte Sprache</span><span class="sxs-lookup"><span data-stu-id="350ac-132">Language configured on the device</span></span>|
|<span data-ttu-id="350ac-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="350ac-133">createdDateTime</span></span>|<span data-ttu-id="350ac-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350ac-134">DateTimeOffset</span></span>|<span data-ttu-id="350ac-135">Erstellungszeit für profile</span><span class="sxs-lookup"><span data-stu-id="350ac-135">Profile creation time</span></span>|
|<span data-ttu-id="350ac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="350ac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="350ac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350ac-137">DateTimeOffset</span></span>|<span data-ttu-id="350ac-138">Zeitpunkt der letzten Änderung des Profils</span><span class="sxs-lookup"><span data-stu-id="350ac-138">Profile last modified time</span></span>|
|<span data-ttu-id="350ac-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="350ac-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="350ac-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="350ac-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="350ac-141">Einstellung für die Out-of-Box-Erfahrung</span><span class="sxs-lookup"><span data-stu-id="350ac-141">Out of box experience setting</span></span>|
|<span data-ttu-id="350ac-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="350ac-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="350ac-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="350ac-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="350ac-144">Einstellung für den Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="350ac-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="350ac-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="350ac-145">extractHardwareHash</span></span>|<span data-ttu-id="350ac-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350ac-146">Boolean</span></span>|<span data-ttu-id="350ac-147">HardwareHash-Extraktion für das Profil</span><span class="sxs-lookup"><span data-stu-id="350ac-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="350ac-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="350ac-148">deviceNameTemplate</span></span>|<span data-ttu-id="350ac-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="350ac-149">String</span></span>|<span data-ttu-id="350ac-150">Die Vorlage, die zum Benennen des autoPilot-Geräts verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="350ac-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="350ac-151">Dabei kann es sich um einen benutzerdefinierten Text handeln, der entweder die Seriennummer des Geräts oder eine zufällig generierte Zahl enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="350ac-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="350ac-152">Die Gesamtlänge des von der Vorlage generierten Texts darf nicht mehr als 15 Zeichen betragen.</span><span class="sxs-lookup"><span data-stu-id="350ac-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="350ac-153">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="350ac-153">enableWhiteGlove</span></span>|<span data-ttu-id="350ac-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350ac-154">Boolean</span></span>|<span data-ttu-id="350ac-155">Aktivieren Sie den weißen Handschuh Autopilot für das Profil.</span><span class="sxs-lookup"><span data-stu-id="350ac-155">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="350ac-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="350ac-156">Relationships</span></span>
|<span data-ttu-id="350ac-157">Beziehung</span><span class="sxs-lookup"><span data-stu-id="350ac-157">Relationship</span></span>|<span data-ttu-id="350ac-158">Typ</span><span class="sxs-lookup"><span data-stu-id="350ac-158">Type</span></span>|<span data-ttu-id="350ac-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="350ac-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="350ac-160">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="350ac-160">assignedDevices</span></span>|<span data-ttu-id="350ac-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="350ac-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="350ac-162">Die Liste der zugewiesenen Geräte für das Profil.</span><span class="sxs-lookup"><span data-stu-id="350ac-162">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="350ac-163">assignments</span><span class="sxs-lookup"><span data-stu-id="350ac-163">assignments</span></span>|<span data-ttu-id="350ac-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="350ac-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="350ac-165">Die Liste der Gruppenzuweisungen für das Profil.</span><span class="sxs-lookup"><span data-stu-id="350ac-165">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="350ac-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="350ac-166">JSON Representation</span></span>
<span data-ttu-id="350ac-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="350ac-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "enableWhiteGlove": true
}
```




