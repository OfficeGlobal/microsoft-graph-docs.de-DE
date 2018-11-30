---
title: Ressourcentyp depIOSEnrollmentProfile
description: Die Ressource DepIOSEnrollmentProfile stellt eine bestimmte Apple Gerät Registrierung Programm (DEP) Registrierung Profil iOS-Konfiguration. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
ms.openlocfilehash: f8ddb907d7dfc3fa43704b162a12c0607d607dd4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063024"
---
# <a name="depiosenrollmentprofile-resource-type"></a><span data-ttu-id="06d3c-104">Ressourcentyp depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="06d3c-104">depIOSEnrollmentProfile resource type</span></span>

> <span data-ttu-id="06d3c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06d3c-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06d3c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06d3c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06d3c-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06d3c-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06d3c-108">Die Ressource DepIOSEnrollmentProfile stellt eine bestimmte Apple Gerät Registrierung Programm (DEP) Registrierung Profil iOS-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="06d3c-108">The DepIOSEnrollmentProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile specific to iOS configuration.</span></span> <span data-ttu-id="06d3c-109">Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können</span><span class="sxs-lookup"><span data-stu-id="06d3c-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="06d3c-110">Erbt vom [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-110">Inherits from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="06d3c-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="06d3c-111">Methods</span></span>
|<span data-ttu-id="06d3c-112">Methode</span><span class="sxs-lookup"><span data-stu-id="06d3c-112">Method</span></span>|<span data-ttu-id="06d3c-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="06d3c-113">Return Type</span></span>|<span data-ttu-id="06d3c-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06d3c-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06d3c-115">Liste depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="06d3c-115">List depIOSEnrollmentProfiles</span></span>](../api/intune-enrollment-depiosenrollmentprofile-list.md)|<span data-ttu-id="06d3c-116">[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="06d3c-116">[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) collection</span></span>|<span data-ttu-id="06d3c-117">Listeneigenschaften und Beziehungen der [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="06d3c-117">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="06d3c-118">Abrufen von depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="06d3c-118">Get depIOSEnrollmentProfile</span></span>](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[<span data-ttu-id="06d3c-119">depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="06d3c-119">depIOSEnrollmentProfile</span></span>](../resources/intune-enrollment-depiosenrollmentprofile.md)|<span data-ttu-id="06d3c-120">Lesen Sie Eigenschaften und Beziehungen des [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06d3c-120">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="06d3c-121">Erstellen von depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="06d3c-121">Create depIOSEnrollmentProfile</span></span>](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[<span data-ttu-id="06d3c-122">depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="06d3c-122">depIOSEnrollmentProfile</span></span>](../resources/intune-enrollment-depiosenrollmentprofile.md)|<span data-ttu-id="06d3c-123">Erstellen eines neuen [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06d3c-123">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="06d3c-124">DepIOSEnrollmentProfile löschen</span><span class="sxs-lookup"><span data-stu-id="06d3c-124">Delete depIOSEnrollmentProfile</span></span>](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|<span data-ttu-id="06d3c-125">Keines</span><span class="sxs-lookup"><span data-stu-id="06d3c-125">None</span></span>|<span data-ttu-id="06d3c-126">Löscht eine [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="06d3c-126">Deletes a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="06d3c-127">DepIOSEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="06d3c-127">Update depIOSEnrollmentProfile</span></span>](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[<span data-ttu-id="06d3c-128">depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="06d3c-128">depIOSEnrollmentProfile</span></span>](../resources/intune-enrollment-depiosenrollmentprofile.md)|<span data-ttu-id="06d3c-129">Aktualisieren Sie die Eigenschaften eines [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06d3c-129">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06d3c-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06d3c-130">Properties</span></span>
|<span data-ttu-id="06d3c-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06d3c-131">Property</span></span>|<span data-ttu-id="06d3c-132">Typ</span><span class="sxs-lookup"><span data-stu-id="06d3c-132">Type</span></span>|<span data-ttu-id="06d3c-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06d3c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06d3c-134">id</span><span class="sxs-lookup"><span data-stu-id="06d3c-134">id</span></span>|<span data-ttu-id="06d3c-135">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-135">String</span></span>|<span data-ttu-id="06d3c-136">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-136">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06d3c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06d3c-137">displayName</span></span>|<span data-ttu-id="06d3c-138">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-138">String</span></span>|<span data-ttu-id="06d3c-139">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-139">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06d3c-140">description</span><span class="sxs-lookup"><span data-stu-id="06d3c-140">description</span></span>|<span data-ttu-id="06d3c-141">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-141">String</span></span>|<span data-ttu-id="06d3c-142">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-142">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06d3c-143">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="06d3c-143">requiresUserAuthentication</span></span>|<span data-ttu-id="06d3c-144">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-144">Boolean</span></span>|<span data-ttu-id="06d3c-145">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="06d3c-145">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06d3c-146">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="06d3c-146">configurationEndpointUrl</span></span>|<span data-ttu-id="06d3c-147">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-147">String</span></span>|<span data-ttu-id="06d3c-148">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="06d3c-148">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06d3c-149">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="06d3c-149">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="06d3c-150">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-150">Boolean</span></span>|<span data-ttu-id="06d3c-151">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="06d3c-151">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="06d3c-152">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-152">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06d3c-153">isDefault</span><span class="sxs-lookup"><span data-stu-id="06d3c-153">isDefault</span></span>|<span data-ttu-id="06d3c-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06d3c-154">Boolean</span></span>|<span data-ttu-id="06d3c-155">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-155">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-156">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-156">supervisedModeEnabled</span></span>|<span data-ttu-id="06d3c-157">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-157">Boolean</span></span>|<span data-ttu-id="06d3c-158">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="06d3c-158">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="06d3c-159">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="06d3c-159">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="06d3c-160">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-160">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-161">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="06d3c-161">supportDepartment</span></span>|<span data-ttu-id="06d3c-162">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-162">String</span></span>|<span data-ttu-id="06d3c-163">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-163">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-164">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-164">passCodeDisabled</span></span>|<span data-ttu-id="06d3c-165">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-165">Boolean</span></span>|<span data-ttu-id="06d3c-166">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="06d3c-166">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-167">isMandatory</span><span class="sxs-lookup"><span data-stu-id="06d3c-167">isMandatory</span></span>|<span data-ttu-id="06d3c-168">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-168">Boolean</span></span>|<span data-ttu-id="06d3c-169">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-169">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-170">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-170">locationDisabled</span></span>|<span data-ttu-id="06d3c-171">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-171">Boolean</span></span>|<span data-ttu-id="06d3c-172">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="06d3c-172">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="06d3c-173">supportPhoneNumber</span></span>|<span data-ttu-id="06d3c-174">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-174">String</span></span>|<span data-ttu-id="06d3c-175">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06d3c-175">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-176">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-176">profileRemovalDisabled</span></span>|<span data-ttu-id="06d3c-177">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-177">Boolean</span></span>|<span data-ttu-id="06d3c-178">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-178">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-179">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="06d3c-179">restoreBlocked</span></span>|<span data-ttu-id="06d3c-180">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-180">Boolean</span></span>|<span data-ttu-id="06d3c-181">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-181">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-182">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-182">appleIdDisabled</span></span>|<span data-ttu-id="06d3c-183">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-183">Boolean</span></span>|<span data-ttu-id="06d3c-184">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="06d3c-184">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-185">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-185">termsAndConditionsDisabled</span></span>|<span data-ttu-id="06d3c-186">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-186">Boolean</span></span>|<span data-ttu-id="06d3c-187">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-187">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-188">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-188">touchIdDisabled</span></span>|<span data-ttu-id="06d3c-189">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-189">Boolean</span></span>|<span data-ttu-id="06d3c-190">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-190">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-191">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-191">applePayDisabled</span></span>|<span data-ttu-id="06d3c-192">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-192">Boolean</span></span>|<span data-ttu-id="06d3c-193">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-193">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-194">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-194">zoomDisabled</span></span>|<span data-ttu-id="06d3c-195">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-195">Boolean</span></span>|<span data-ttu-id="06d3c-196">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-196">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-197">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-197">siriDisabled</span></span>|<span data-ttu-id="06d3c-198">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-198">Boolean</span></span>|<span data-ttu-id="06d3c-199">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="06d3c-199">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-200">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-200">diagnosticsDisabled</span></span>|<span data-ttu-id="06d3c-201">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-201">Boolean</span></span>|<span data-ttu-id="06d3c-202">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="06d3c-202">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06d3c-203">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="06d3c-203">iTunesPairingMode</span></span>|[<span data-ttu-id="06d3c-204">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="06d3c-204">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="06d3c-205">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="06d3c-205">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="06d3c-206">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="06d3c-206">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="06d3c-207">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="06d3c-207">managementCertificates</span></span>|<span data-ttu-id="06d3c-208">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="06d3c-208">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="06d3c-209">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="06d3c-209">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="06d3c-210">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="06d3c-210">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="06d3c-211">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-211">Boolean</span></span>|<span data-ttu-id="06d3c-212">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="06d3c-212">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="06d3c-213">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="06d3c-213">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="06d3c-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-214">Boolean</span></span>|<span data-ttu-id="06d3c-215">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="06d3c-215">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="06d3c-216">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="06d3c-216">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="06d3c-217">Int32</span><span class="sxs-lookup"><span data-stu-id="06d3c-217">Int32</span></span>|<span data-ttu-id="06d3c-218">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="06d3c-218">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="06d3c-219">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="06d3c-219">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="06d3c-220">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="06d3c-220">enableSharedIPad</span></span>|<span data-ttu-id="06d3c-221">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-221">Boolean</span></span>|<span data-ttu-id="06d3c-222">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="06d3c-222">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="06d3c-223">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="06d3c-223">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="06d3c-224">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="06d3c-224">companyPortalVppTokenId</span></span>|<span data-ttu-id="06d3c-225">String</span><span class="sxs-lookup"><span data-stu-id="06d3c-225">String</span></span>|<span data-ttu-id="06d3c-226">Wenn festgelegt ist, gibt an, welche Vpp Token zum Bereitstellen der Unternehmensportal mit Gerät-Lizenzierung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="06d3c-226">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="06d3c-227">'EnableAuthenticationViaCompanyPortal' muss für diese Eigenschaft festgelegt werden soll festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="06d3c-227">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="06d3c-228">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="06d3c-228">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="06d3c-229">Boolesch</span><span class="sxs-lookup"><span data-stu-id="06d3c-229">Boolean</span></span>|<span data-ttu-id="06d3c-230">Weist das Gerät zum Aktivieren der einzelnen app-Modus und Anwenden von app-Sperre während der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="06d3c-230">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="06d3c-231">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="06d3c-231">Default is false.</span></span> <span data-ttu-id="06d3c-232">'EnableAuthenticationViaCompanyPortal' und 'CompanyPortalVppTokenId' müssen für diese Eigenschaft festgelegt werden soll, festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="06d3c-232">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06d3c-233">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06d3c-233">Relationships</span></span>
<span data-ttu-id="06d3c-234">Keine</span><span class="sxs-lookup"><span data-stu-id="06d3c-234">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06d3c-235">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06d3c-235">JSON Representation</span></span>
<span data-ttu-id="06d3c-236">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06d3c-236">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "diagnosticsDisabled": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
  "enableSingleAppEnrollmentMode": true
}
```




