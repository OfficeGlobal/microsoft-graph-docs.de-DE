---
title: Ressourcentyp depEnrollmentBaseProfile
description: Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
author: tfitzmac
ms.openlocfilehash: 26335fd3d35494b815dd43531ad54b4796dc861c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308372"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="c9e67-104">Ressourcentyp depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c9e67-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="c9e67-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9e67-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9e67-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9e67-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9e67-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9e67-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9e67-108">Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil.</span><span class="sxs-lookup"><span data-stu-id="c9e67-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="c9e67-109">Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können</span><span class="sxs-lookup"><span data-stu-id="c9e67-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="c9e67-110">Erbt vom [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c9e67-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c9e67-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="c9e67-111">Methods</span></span>
|<span data-ttu-id="c9e67-112">Methode</span><span class="sxs-lookup"><span data-stu-id="c9e67-112">Method</span></span>|<span data-ttu-id="c9e67-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c9e67-113">Return Type</span></span>|<span data-ttu-id="c9e67-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9e67-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9e67-115">Liste depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="c9e67-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="c9e67-116">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c9e67-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="c9e67-117">Listeneigenschaften und Beziehungen der [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c9e67-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="c9e67-118">Abrufen von depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c9e67-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="c9e67-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c9e67-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="c9e67-120">Lesen Sie Eigenschaften und Beziehungen des [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9e67-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9e67-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9e67-121">Properties</span></span>
|<span data-ttu-id="c9e67-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9e67-122">Property</span></span>|<span data-ttu-id="c9e67-123">Typ</span><span class="sxs-lookup"><span data-stu-id="c9e67-123">Type</span></span>|<span data-ttu-id="c9e67-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9e67-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9e67-125">id</span><span class="sxs-lookup"><span data-stu-id="c9e67-125">id</span></span>|<span data-ttu-id="c9e67-126">String</span><span class="sxs-lookup"><span data-stu-id="c9e67-126">String</span></span>|<span data-ttu-id="c9e67-127">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c9e67-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c9e67-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c9e67-128">displayName</span></span>|<span data-ttu-id="c9e67-129">String</span><span class="sxs-lookup"><span data-stu-id="c9e67-129">String</span></span>|<span data-ttu-id="c9e67-130">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c9e67-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c9e67-131">description</span><span class="sxs-lookup"><span data-stu-id="c9e67-131">description</span></span>|<span data-ttu-id="c9e67-132">String</span><span class="sxs-lookup"><span data-stu-id="c9e67-132">String</span></span>|<span data-ttu-id="c9e67-133">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c9e67-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c9e67-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="c9e67-134">requiresUserAuthentication</span></span>|<span data-ttu-id="c9e67-135">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-135">Boolean</span></span>|<span data-ttu-id="c9e67-136">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="c9e67-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c9e67-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="c9e67-137">configurationEndpointUrl</span></span>|<span data-ttu-id="c9e67-138">String</span><span class="sxs-lookup"><span data-stu-id="c9e67-138">String</span></span>|<span data-ttu-id="c9e67-139">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="c9e67-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c9e67-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c9e67-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c9e67-141">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-141">Boolean</span></span>|<span data-ttu-id="c9e67-142">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="c9e67-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="c9e67-143">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c9e67-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c9e67-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="c9e67-144">isDefault</span></span>|<span data-ttu-id="c9e67-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c9e67-145">Boolean</span></span>|<span data-ttu-id="c9e67-146">Gibt an, ob dies das Standardprofil ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="c9e67-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-147">supervisedModeEnabled</span></span>|<span data-ttu-id="c9e67-148">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-148">Boolean</span></span>|<span data-ttu-id="c9e67-149">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="c9e67-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="c9e67-150">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="c9e67-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="c9e67-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="c9e67-151">supportDepartment</span></span>|<span data-ttu-id="c9e67-152">String</span><span class="sxs-lookup"><span data-stu-id="c9e67-152">String</span></span>|<span data-ttu-id="c9e67-153">Abteilung Supportinformationen</span><span class="sxs-lookup"><span data-stu-id="c9e67-153">Support department information</span></span>|
|<span data-ttu-id="c9e67-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-154">passCodeDisabled</span></span>|<span data-ttu-id="c9e67-155">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-155">Boolean</span></span>|<span data-ttu-id="c9e67-156">Gibt an, ob Kennung Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="c9e67-157">isMandatory</span></span>|<span data-ttu-id="c9e67-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-158">Boolean</span></span>|<span data-ttu-id="c9e67-159">Gibt an, ob das Profil zwingend erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c9e67-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="c9e67-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-160">locationDisabled</span></span>|<span data-ttu-id="c9e67-161">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-161">Boolean</span></span>|<span data-ttu-id="c9e67-162">Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c9e67-163">supportPhoneNumber</span></span>|<span data-ttu-id="c9e67-164">String</span><span class="sxs-lookup"><span data-stu-id="c9e67-164">String</span></span>|<span data-ttu-id="c9e67-165">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="c9e67-165">Support phone number</span></span>|
|<span data-ttu-id="c9e67-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-166">profileRemovalDisabled</span></span>|<span data-ttu-id="c9e67-167">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-167">Boolean</span></span>|<span data-ttu-id="c9e67-168">Gibt an, ob die Option Profil entfernen deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="c9e67-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c9e67-169">restoreBlocked</span></span>|<span data-ttu-id="c9e67-170">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-170">Boolean</span></span>|<span data-ttu-id="c9e67-171">Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="c9e67-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-172">appleIdDisabled</span></span>|<span data-ttu-id="c9e67-173">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-173">Boolean</span></span>|<span data-ttu-id="c9e67-174">Gibt an, ob Apple Id Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="c9e67-176">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-176">Boolean</span></span>|<span data-ttu-id="c9e67-177">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-178">touchIdDisabled</span></span>|<span data-ttu-id="c9e67-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-179">Boolean</span></span>|<span data-ttu-id="c9e67-180">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-181">applePayDisabled</span></span>|<span data-ttu-id="c9e67-182">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-182">Boolean</span></span>|<span data-ttu-id="c9e67-183">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-184">zoomDisabled</span></span>|<span data-ttu-id="c9e67-185">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-185">Boolean</span></span>|<span data-ttu-id="c9e67-186">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-187">siriDisabled</span></span>|<span data-ttu-id="c9e67-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-188">Boolean</span></span>|<span data-ttu-id="c9e67-189">Gibt an, ob Siri Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="c9e67-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="c9e67-190">diagnosticsDisabled</span></span>|<span data-ttu-id="c9e67-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9e67-191">Boolean</span></span>|<span data-ttu-id="c9e67-192">Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="c9e67-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9e67-193">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9e67-193">Relationships</span></span>
<span data-ttu-id="c9e67-194">Keine</span><span class="sxs-lookup"><span data-stu-id="c9e67-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9e67-195">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9e67-195">JSON Representation</span></span>
<span data-ttu-id="c9e67-196">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9e67-196">Here is a JSON representation of the resource.</span></span>
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
  "diagnosticsDisabled": true
}
```





