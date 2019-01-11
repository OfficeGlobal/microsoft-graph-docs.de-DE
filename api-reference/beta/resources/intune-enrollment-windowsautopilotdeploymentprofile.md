---
title: Ressourcentyp windowsAutopilotDeploymentProfile
description: Windows Autopilot Bereitstellung Benutzerprofil
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1538497dc5105dcd2e7f0c9ff7fdf83c3ddec56e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892197"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="862aa-103">Ressourcentyp windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="862aa-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="862aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="862aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="862aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="862aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="862aa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="862aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="862aa-107">Windows Autopilot Bereitstellung Benutzerprofil</span><span class="sxs-lookup"><span data-stu-id="862aa-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="862aa-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="862aa-108">Methods</span></span>
|<span data-ttu-id="862aa-109">Methode</span><span class="sxs-lookup"><span data-stu-id="862aa-109">Method</span></span>|<span data-ttu-id="862aa-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="862aa-110">Return Type</span></span>|<span data-ttu-id="862aa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="862aa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="862aa-112">Abrufen von windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="862aa-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="862aa-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="862aa-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="862aa-114">Lesen Sie Eigenschaften und Beziehungen des [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="862aa-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="862aa-115">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="862aa-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="862aa-116">Keine</span><span class="sxs-lookup"><span data-stu-id="862aa-116">None</span></span>|<span data-ttu-id="862aa-117">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="862aa-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="862aa-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="862aa-118">Properties</span></span>
|<span data-ttu-id="862aa-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="862aa-119">Property</span></span>|<span data-ttu-id="862aa-120">Typ</span><span class="sxs-lookup"><span data-stu-id="862aa-120">Type</span></span>|<span data-ttu-id="862aa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="862aa-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="862aa-122">id</span><span class="sxs-lookup"><span data-stu-id="862aa-122">id</span></span>|<span data-ttu-id="862aa-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="862aa-123">String</span></span>|<span data-ttu-id="862aa-124">Profil-Taste</span><span class="sxs-lookup"><span data-stu-id="862aa-124">Profile Key</span></span>|
|<span data-ttu-id="862aa-125">displayName</span><span class="sxs-lookup"><span data-stu-id="862aa-125">displayName</span></span>|<span data-ttu-id="862aa-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="862aa-126">String</span></span>|<span data-ttu-id="862aa-127">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="862aa-127">Name of the profile</span></span>|
|<span data-ttu-id="862aa-128">description</span><span class="sxs-lookup"><span data-stu-id="862aa-128">description</span></span>|<span data-ttu-id="862aa-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="862aa-129">String</span></span>|<span data-ttu-id="862aa-130">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="862aa-130">Description of the profile</span></span>|
|<span data-ttu-id="862aa-131">language</span><span class="sxs-lookup"><span data-stu-id="862aa-131">language</span></span>|<span data-ttu-id="862aa-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="862aa-132">String</span></span>|<span data-ttu-id="862aa-133">Auf dem Gerät konfigurierten Sprache</span><span class="sxs-lookup"><span data-stu-id="862aa-133">Language configured on the device</span></span>|
|<span data-ttu-id="862aa-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="862aa-134">createdDateTime</span></span>|<span data-ttu-id="862aa-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862aa-135">DateTimeOffset</span></span>|<span data-ttu-id="862aa-136">Erstellungszeit Profil</span><span class="sxs-lookup"><span data-stu-id="862aa-136">Profile creation time</span></span>|
|<span data-ttu-id="862aa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="862aa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="862aa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862aa-138">DateTimeOffset</span></span>|<span data-ttu-id="862aa-139">Profil Zeitpunkt der letzten Änderung</span><span class="sxs-lookup"><span data-stu-id="862aa-139">Profile last modified time</span></span>|
|<span data-ttu-id="862aa-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="862aa-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="862aa-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="862aa-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="862aa-142">Erleben Sie die Einstellung im Lieferzustand</span><span class="sxs-lookup"><span data-stu-id="862aa-142">Out of box experience setting</span></span>|
|<span data-ttu-id="862aa-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="862aa-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="862aa-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="862aa-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="862aa-145">Registrierung Status Bildschirm Einstellung</span><span class="sxs-lookup"><span data-stu-id="862aa-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="862aa-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="862aa-146">extractHardwareHash</span></span>|<span data-ttu-id="862aa-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="862aa-147">Boolean</span></span>|<span data-ttu-id="862aa-148">Extraktion von HardwareHash für das Profil</span><span class="sxs-lookup"><span data-stu-id="862aa-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="862aa-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="862aa-149">deviceNameTemplate</span></span>|<span data-ttu-id="862aa-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="862aa-150">String</span></span>|<span data-ttu-id="862aa-151">Die Vorlage verwendet, um das Gerät AutoPilot nennen.</span><span class="sxs-lookup"><span data-stu-id="862aa-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="862aa-152">Dies kann ein benutzerdefinierter Text und kann auch die Seriennummer des Geräts, oder aber eine zufällig erzeugte Zahl enthalten.</span><span class="sxs-lookup"><span data-stu-id="862aa-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="862aa-153">Die gesamte Länge des Texts von der Vorlage generierte kann nicht mehr als 15 Zeichen sein.</span><span class="sxs-lookup"><span data-stu-id="862aa-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="862aa-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="862aa-154">Relationships</span></span>
|<span data-ttu-id="862aa-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="862aa-155">Relationship</span></span>|<span data-ttu-id="862aa-156">Typ</span><span class="sxs-lookup"><span data-stu-id="862aa-156">Type</span></span>|<span data-ttu-id="862aa-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="862aa-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="862aa-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="862aa-158">assignedDevices</span></span>|<span data-ttu-id="862aa-159">[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="862aa-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="862aa-160">Die Liste der Geräte für das Profil.</span><span class="sxs-lookup"><span data-stu-id="862aa-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="862aa-161">assignments</span><span class="sxs-lookup"><span data-stu-id="862aa-161">assignments</span></span>|<span data-ttu-id="862aa-162">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="862aa-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="862aa-163">Die Liste der Gruppe Zuordnungen für das Profil.</span><span class="sxs-lookup"><span data-stu-id="862aa-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="862aa-164">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="862aa-164">JSON Representation</span></span>
<span data-ttu-id="862aa-165">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="862aa-165">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```





