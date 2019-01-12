---
title: Ressourcentyp depEnrollmentBaseProfile
description: Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e1383048b08a309ea0ecf60eb1ad07c2636e7e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937670"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="522cb-104">Ressourcentyp depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="522cb-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="522cb-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="522cb-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="522cb-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="522cb-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="522cb-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="522cb-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="522cb-108">Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil.</span><span class="sxs-lookup"><span data-stu-id="522cb-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="522cb-109">Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können</span><span class="sxs-lookup"><span data-stu-id="522cb-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="522cb-110">Erbt vom [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="522cb-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="522cb-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="522cb-111">Methods</span></span>
|<span data-ttu-id="522cb-112">Methode</span><span class="sxs-lookup"><span data-stu-id="522cb-112">Method</span></span>|<span data-ttu-id="522cb-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="522cb-113">Return Type</span></span>|<span data-ttu-id="522cb-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="522cb-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="522cb-115">Liste depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="522cb-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="522cb-116">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="522cb-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="522cb-117">Listeneigenschaften und Beziehungen der [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="522cb-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="522cb-118">Abrufen von depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="522cb-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="522cb-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="522cb-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="522cb-120">Lesen Sie Eigenschaften und Beziehungen des [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="522cb-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="522cb-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="522cb-121">Properties</span></span>
|<span data-ttu-id="522cb-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="522cb-122">Property</span></span>|<span data-ttu-id="522cb-123">Typ</span><span class="sxs-lookup"><span data-stu-id="522cb-123">Type</span></span>|<span data-ttu-id="522cb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="522cb-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="522cb-125">id</span><span class="sxs-lookup"><span data-stu-id="522cb-125">id</span></span>|<span data-ttu-id="522cb-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="522cb-126">String</span></span>|<span data-ttu-id="522cb-127">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="522cb-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="522cb-128">displayName</span><span class="sxs-lookup"><span data-stu-id="522cb-128">displayName</span></span>|<span data-ttu-id="522cb-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="522cb-129">String</span></span>|<span data-ttu-id="522cb-130">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="522cb-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="522cb-131">description</span><span class="sxs-lookup"><span data-stu-id="522cb-131">description</span></span>|<span data-ttu-id="522cb-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="522cb-132">String</span></span>|<span data-ttu-id="522cb-133">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="522cb-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="522cb-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="522cb-134">requiresUserAuthentication</span></span>|<span data-ttu-id="522cb-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-135">Boolean</span></span>|<span data-ttu-id="522cb-136">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="522cb-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="522cb-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="522cb-137">configurationEndpointUrl</span></span>|<span data-ttu-id="522cb-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="522cb-138">String</span></span>|<span data-ttu-id="522cb-139">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="522cb-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="522cb-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="522cb-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="522cb-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-141">Boolean</span></span>|<span data-ttu-id="522cb-142">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="522cb-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="522cb-143">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="522cb-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="522cb-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="522cb-144">isDefault</span></span>|<span data-ttu-id="522cb-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-145">Boolean</span></span>|<span data-ttu-id="522cb-146">Gibt an, ob dies das Standardprofil ist</span><span class="sxs-lookup"><span data-stu-id="522cb-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="522cb-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="522cb-147">supervisedModeEnabled</span></span>|<span data-ttu-id="522cb-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-148">Boolean</span></span>|<span data-ttu-id="522cb-149">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="522cb-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="522cb-150">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="522cb-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="522cb-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="522cb-151">supportDepartment</span></span>|<span data-ttu-id="522cb-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="522cb-152">String</span></span>|<span data-ttu-id="522cb-153">Abteilung Supportinformationen</span><span class="sxs-lookup"><span data-stu-id="522cb-153">Support department information</span></span>|
|<span data-ttu-id="522cb-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-154">passCodeDisabled</span></span>|<span data-ttu-id="522cb-155">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-155">Boolean</span></span>|<span data-ttu-id="522cb-156">Gibt an, ob Kennung Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="522cb-157">isMandatory</span></span>|<span data-ttu-id="522cb-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-158">Boolean</span></span>|<span data-ttu-id="522cb-159">Gibt an, ob das Profil zwingend erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="522cb-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="522cb-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-160">locationDisabled</span></span>|<span data-ttu-id="522cb-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-161">Boolean</span></span>|<span data-ttu-id="522cb-162">Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="522cb-163">supportPhoneNumber</span></span>|<span data-ttu-id="522cb-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="522cb-164">String</span></span>|<span data-ttu-id="522cb-165">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="522cb-165">Support phone number</span></span>|
|<span data-ttu-id="522cb-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-166">profileRemovalDisabled</span></span>|<span data-ttu-id="522cb-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-167">Boolean</span></span>|<span data-ttu-id="522cb-168">Gibt an, ob die Option Profil entfernen deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="522cb-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="522cb-169">restoreBlocked</span></span>|<span data-ttu-id="522cb-170">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-170">Boolean</span></span>|<span data-ttu-id="522cb-171">Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="522cb-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="522cb-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-172">appleIdDisabled</span></span>|<span data-ttu-id="522cb-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-173">Boolean</span></span>|<span data-ttu-id="522cb-174">Gibt an, ob Apple Id Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="522cb-176">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-176">Boolean</span></span>|<span data-ttu-id="522cb-177">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-178">touchIdDisabled</span></span>|<span data-ttu-id="522cb-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-179">Boolean</span></span>|<span data-ttu-id="522cb-180">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-181">applePayDisabled</span></span>|<span data-ttu-id="522cb-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-182">Boolean</span></span>|<span data-ttu-id="522cb-183">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-184">zoomDisabled</span></span>|<span data-ttu-id="522cb-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-185">Boolean</span></span>|<span data-ttu-id="522cb-186">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-187">siriDisabled</span></span>|<span data-ttu-id="522cb-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-188">Boolean</span></span>|<span data-ttu-id="522cb-189">Gibt an, ob Siri Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="522cb-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="522cb-190">diagnosticsDisabled</span></span>|<span data-ttu-id="522cb-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="522cb-191">Boolean</span></span>|<span data-ttu-id="522cb-192">Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="522cb-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="522cb-193">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="522cb-193">Relationships</span></span>
<span data-ttu-id="522cb-194">Keine</span><span class="sxs-lookup"><span data-stu-id="522cb-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="522cb-195">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="522cb-195">JSON Representation</span></span>
<span data-ttu-id="522cb-196">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="522cb-196">Here is a JSON representation of the resource.</span></span>
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





