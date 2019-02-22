---
title: depEnrollmentBaseProfile-Ressourcentyp
description: Die DepEnrollmentBaseProfile-Ressource stellt ein Registrierungsprofil für das Apple-Geräte Registrierungsprogramm (DEP) dar. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ad27470bb09313084feadcf468d83e58964532
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143106"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="f9ab8-104">depEnrollmentBaseProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f9ab8-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="f9ab8-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ab8-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ab8-107">Die DepEnrollmentBaseProfile-Ressource stellt ein Registrierungsprofil für das Apple-Geräte Registrierungsprogramm (DEP) dar.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="f9ab8-108">Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="f9ab8-109">Erbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f9ab8-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f9ab8-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="f9ab8-110">Methods</span></span>
|<span data-ttu-id="f9ab8-111">Methode</span><span class="sxs-lookup"><span data-stu-id="f9ab8-111">Method</span></span>|<span data-ttu-id="f9ab8-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f9ab8-112">Return Type</span></span>|<span data-ttu-id="f9ab8-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9ab8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9ab8-114">DepEnrollmentBaseProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="f9ab8-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="f9ab8-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f9ab8-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="f9ab8-116">AufListen von Eigenschaften und Beziehungen der [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="f9ab8-117">DepEnrollmentBaseProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="f9ab8-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="f9ab8-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f9ab8-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="f9ab8-119">Lesen von Eigenschaften und Beziehungen des [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9ab8-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9ab8-120">Properties</span></span>
|<span data-ttu-id="f9ab8-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9ab8-121">Property</span></span>|<span data-ttu-id="f9ab8-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f9ab8-122">Type</span></span>|<span data-ttu-id="f9ab8-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9ab8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ab8-124">id</span><span class="sxs-lookup"><span data-stu-id="f9ab8-124">id</span></span>|<span data-ttu-id="f9ab8-125">string</span><span class="sxs-lookup"><span data-stu-id="f9ab8-125">String</span></span>|<span data-ttu-id="f9ab8-126">Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-127">displayName</span><span class="sxs-lookup"><span data-stu-id="f9ab8-127">displayName</span></span>|<span data-ttu-id="f9ab8-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9ab8-128">String</span></span>|<span data-ttu-id="f9ab8-129">Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="f9ab8-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-130">description</span><span class="sxs-lookup"><span data-stu-id="f9ab8-130">description</span></span>|<span data-ttu-id="f9ab8-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9ab8-131">String</span></span>|<span data-ttu-id="f9ab8-132">Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="f9ab8-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f9ab8-133">requiresUserAuthentication</span></span>|<span data-ttu-id="f9ab8-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-134">Boolean</span></span>|<span data-ttu-id="f9ab8-135">Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-136">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f9ab8-136">configurationEndpointUrl</span></span>|<span data-ttu-id="f9ab8-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9ab8-137">String</span></span>|<span data-ttu-id="f9ab8-138">Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung</span><span class="sxs-lookup"><span data-stu-id="f9ab8-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f9ab8-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f9ab8-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-140">Boolean</span></span>|<span data-ttu-id="f9ab8-141">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f9ab8-142">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f9ab8-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f9ab8-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f9ab8-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-144">Boolean</span></span>|<span data-ttu-id="f9ab8-145">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f9ab8-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="f9ab8-146">isDefault</span></span>|<span data-ttu-id="f9ab8-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-147">Boolean</span></span>|<span data-ttu-id="f9ab8-148">Gibt an, ob dies das Standardprofil ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="f9ab8-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-149">supervisedModeEnabled</span></span>|<span data-ttu-id="f9ab8-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-150">Boolean</span></span>|<span data-ttu-id="f9ab8-151">Überwachter Modus, true, um zu aktivieren, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f9ab8-152">Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="f9ab8-153">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f9ab8-153">supportDepartment</span></span>|<span data-ttu-id="f9ab8-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9ab8-154">String</span></span>|<span data-ttu-id="f9ab8-155">Informationen zur Support Abteilung</span><span class="sxs-lookup"><span data-stu-id="f9ab8-155">Support department information</span></span>|
|<span data-ttu-id="f9ab8-156">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-156">passCodeDisabled</span></span>|<span data-ttu-id="f9ab8-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-157">Boolean</span></span>|<span data-ttu-id="f9ab8-158">Gibt an, ob der Bereich "Passcode" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-159">isMandatory</span><span class="sxs-lookup"><span data-stu-id="f9ab8-159">isMandatory</span></span>|<span data-ttu-id="f9ab8-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-160">Boolean</span></span>|<span data-ttu-id="f9ab8-161">Gibt an, ob das Profil obligatorisch ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="f9ab8-162">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-162">locationDisabled</span></span>|<span data-ttu-id="f9ab8-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-163">Boolean</span></span>|<span data-ttu-id="f9ab8-164">Gibt an, ob der Standortdienst-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f9ab8-165">supportPhoneNumber</span></span>|<span data-ttu-id="f9ab8-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9ab8-166">String</span></span>|<span data-ttu-id="f9ab8-167">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="f9ab8-167">Support phone number</span></span>|
|<span data-ttu-id="f9ab8-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-168">profileRemovalDisabled</span></span>|<span data-ttu-id="f9ab8-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-169">Boolean</span></span>|<span data-ttu-id="f9ab8-170">Gibt an, ob die Profil Entfernungs Option deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="f9ab8-171">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f9ab8-171">restoreBlocked</span></span>|<span data-ttu-id="f9ab8-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-172">Boolean</span></span>|<span data-ttu-id="f9ab8-173">Gibt an, ob der wiederHerstellungs-Setup Bereich blockiert ist</span><span class="sxs-lookup"><span data-stu-id="f9ab8-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="f9ab8-174">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-174">appleIdDisabled</span></span>|<span data-ttu-id="f9ab8-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-175">Boolean</span></span>|<span data-ttu-id="f9ab8-176">Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f9ab8-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-178">Boolean</span></span>|<span data-ttu-id="f9ab8-179">Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-180">touchIdDisabled</span></span>|<span data-ttu-id="f9ab8-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-181">Boolean</span></span>|<span data-ttu-id="f9ab8-182">Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-183">applePayDisabled</span></span>|<span data-ttu-id="f9ab8-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-184">Boolean</span></span>|<span data-ttu-id="f9ab8-185">Gibt an, ob der Apple Pay-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-186">zoomDisabled</span></span>|<span data-ttu-id="f9ab8-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-187">Boolean</span></span>|<span data-ttu-id="f9ab8-188">Gibt an, ob der Zoom-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-189">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-189">siriDisabled</span></span>|<span data-ttu-id="f9ab8-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-190">Boolean</span></span>|<span data-ttu-id="f9ab8-191">Gibt an, ob der Siri-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-192">diagnosticsDisabled</span></span>|<span data-ttu-id="f9ab8-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-193">Boolean</span></span>|<span data-ttu-id="f9ab8-194">Gibt an, ob der Diagnose-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="f9ab8-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="f9ab8-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-196">Boolean</span></span>|<span data-ttu-id="f9ab8-197">Gibt an, ob der displaytone-Setupbildschirm deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="f9ab8-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="f9ab8-198">privacyPaneDisabled</span></span>|<span data-ttu-id="f9ab8-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9ab8-199">Boolean</span></span>|<span data-ttu-id="f9ab8-200">Gibt an, ob der Datenschutz Bildschirm deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-200">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9ab8-201">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f9ab8-201">Relationships</span></span>
<span data-ttu-id="f9ab8-202">Keine</span><span class="sxs-lookup"><span data-stu-id="f9ab8-202">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9ab8-203">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9ab8-203">JSON Representation</span></span>
<span data-ttu-id="f9ab8-204">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9ab8-204">Here is a JSON representation of the resource.</span></span>
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




