---
title: Ressourcentyp depEnrollmentBaseProfile
description: Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423755"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="e60d7-104">Ressourcentyp depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="e60d7-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="e60d7-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e60d7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e60d7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e60d7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e60d7-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e60d7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e60d7-108">Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil.</span><span class="sxs-lookup"><span data-stu-id="e60d7-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="e60d7-109">Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können</span><span class="sxs-lookup"><span data-stu-id="e60d7-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="e60d7-110">Erbt vom [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e60d7-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e60d7-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="e60d7-111">Methods</span></span>
|<span data-ttu-id="e60d7-112">Methode</span><span class="sxs-lookup"><span data-stu-id="e60d7-112">Method</span></span>|<span data-ttu-id="e60d7-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e60d7-113">Return Type</span></span>|<span data-ttu-id="e60d7-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e60d7-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e60d7-115">Liste depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="e60d7-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="e60d7-116">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e60d7-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="e60d7-117">Listeneigenschaften und Beziehungen der [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="e60d7-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="e60d7-118">Abrufen von depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="e60d7-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="e60d7-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="e60d7-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="e60d7-120">Lesen Sie Eigenschaften und Beziehungen des [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e60d7-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e60d7-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e60d7-121">Properties</span></span>
|<span data-ttu-id="e60d7-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e60d7-122">Property</span></span>|<span data-ttu-id="e60d7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e60d7-123">Type</span></span>|<span data-ttu-id="e60d7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e60d7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e60d7-125">id</span><span class="sxs-lookup"><span data-stu-id="e60d7-125">id</span></span>|<span data-ttu-id="e60d7-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e60d7-126">String</span></span>|<span data-ttu-id="e60d7-127">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e60d7-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e60d7-128">displayName</span></span>|<span data-ttu-id="e60d7-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e60d7-129">String</span></span>|<span data-ttu-id="e60d7-130">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e60d7-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-131">description</span><span class="sxs-lookup"><span data-stu-id="e60d7-131">description</span></span>|<span data-ttu-id="e60d7-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e60d7-132">String</span></span>|<span data-ttu-id="e60d7-133">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e60d7-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e60d7-134">requiresUserAuthentication</span></span>|<span data-ttu-id="e60d7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-135">Boolean</span></span>|<span data-ttu-id="e60d7-136">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="e60d7-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e60d7-137">configurationEndpointUrl</span></span>|<span data-ttu-id="e60d7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e60d7-138">String</span></span>|<span data-ttu-id="e60d7-139">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="e60d7-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e60d7-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e60d7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-141">Boolean</span></span>|<span data-ttu-id="e60d7-142">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="e60d7-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="e60d7-143">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e60d7-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="e60d7-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="e60d7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-145">Boolean</span></span>|<span data-ttu-id="e60d7-146">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e60d7-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="e60d7-147">isDefault</span></span>|<span data-ttu-id="e60d7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-148">Boolean</span></span>|<span data-ttu-id="e60d7-149">Gibt an, ob dies das Standardprofil ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="e60d7-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-150">supervisedModeEnabled</span></span>|<span data-ttu-id="e60d7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-151">Boolean</span></span>|<span data-ttu-id="e60d7-152">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="e60d7-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="e60d7-153">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="e60d7-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="e60d7-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="e60d7-154">supportDepartment</span></span>|<span data-ttu-id="e60d7-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e60d7-155">String</span></span>|<span data-ttu-id="e60d7-156">Abteilung Supportinformationen</span><span class="sxs-lookup"><span data-stu-id="e60d7-156">Support department information</span></span>|
|<span data-ttu-id="e60d7-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-157">passCodeDisabled</span></span>|<span data-ttu-id="e60d7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-158">Boolean</span></span>|<span data-ttu-id="e60d7-159">Gibt an, ob Kennung Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-160">isMandatory</span><span class="sxs-lookup"><span data-stu-id="e60d7-160">isMandatory</span></span>|<span data-ttu-id="e60d7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-161">Boolean</span></span>|<span data-ttu-id="e60d7-162">Gibt an, ob das Profil zwingend erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e60d7-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="e60d7-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-163">locationDisabled</span></span>|<span data-ttu-id="e60d7-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-164">Boolean</span></span>|<span data-ttu-id="e60d7-165">Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e60d7-166">supportPhoneNumber</span></span>|<span data-ttu-id="e60d7-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e60d7-167">String</span></span>|<span data-ttu-id="e60d7-168">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="e60d7-168">Support phone number</span></span>|
|<span data-ttu-id="e60d7-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-169">profileRemovalDisabled</span></span>|<span data-ttu-id="e60d7-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-170">Boolean</span></span>|<span data-ttu-id="e60d7-171">Gibt an, ob die Option Profil entfernen deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="e60d7-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e60d7-172">restoreBlocked</span></span>|<span data-ttu-id="e60d7-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-173">Boolean</span></span>|<span data-ttu-id="e60d7-174">Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="e60d7-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-175">appleIdDisabled</span></span>|<span data-ttu-id="e60d7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-176">Boolean</span></span>|<span data-ttu-id="e60d7-177">Gibt an, ob Apple Id Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="e60d7-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-179">Boolean</span></span>|<span data-ttu-id="e60d7-180">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-181">touchIdDisabled</span></span>|<span data-ttu-id="e60d7-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-182">Boolean</span></span>|<span data-ttu-id="e60d7-183">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-184">applePayDisabled</span></span>|<span data-ttu-id="e60d7-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-185">Boolean</span></span>|<span data-ttu-id="e60d7-186">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-187">zoomDisabled</span></span>|<span data-ttu-id="e60d7-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-188">Boolean</span></span>|<span data-ttu-id="e60d7-189">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-190">siriDisabled</span></span>|<span data-ttu-id="e60d7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-191">Boolean</span></span>|<span data-ttu-id="e60d7-192">Gibt an, ob Siri Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-193">diagnosticsDisabled</span></span>|<span data-ttu-id="e60d7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-194">Boolean</span></span>|<span data-ttu-id="e60d7-195">Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="e60d7-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="e60d7-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-197">Boolean</span></span>|<span data-ttu-id="e60d7-198">Gibt an, ob Displaytone Setupbildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="e60d7-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="e60d7-199">privacyPaneDisabled</span></span>|<span data-ttu-id="e60d7-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60d7-200">Boolean</span></span>|<span data-ttu-id="e60d7-201">Gibt an, ob Privacy Bildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="e60d7-201">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="e60d7-202">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e60d7-202">Relationships</span></span>
<span data-ttu-id="e60d7-203">Keine</span><span class="sxs-lookup"><span data-stu-id="e60d7-203">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e60d7-204">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e60d7-204">JSON Representation</span></span>
<span data-ttu-id="e60d7-205">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e60d7-205">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true
}
```




