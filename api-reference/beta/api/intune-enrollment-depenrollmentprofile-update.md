---
title: DepEnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DepEnrollmentProfile-Objekts.
ms.openlocfilehash: 1026abe11bec1a766b7fda2907612d77af077bd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063556"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="3eb8a-103">DepEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3eb8a-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="3eb8a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eb8a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eb8a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3eb8a-107">Aktualisieren Sie die Eigenschaften eines [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3eb8a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3eb8a-108">Prerequisites</span></span>
<span data-ttu-id="3eb8a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb8a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3eb8a-111">Permission type</span></span>|<span data-ttu-id="3eb8a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb8a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb8a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb8a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb8a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb8a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eb8a-116">Not supported.</span></span>|
|<span data-ttu-id="3eb8a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3eb8a-117">Application</span></span>|<span data-ttu-id="3eb8a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eb8a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb8a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eb8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="3eb8a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3eb8a-120">Request headers</span></span>
|<span data-ttu-id="3eb8a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3eb8a-121">Header</span></span>|<span data-ttu-id="3eb8a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3eb8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb8a-123">Authorization</span></span>|<span data-ttu-id="3eb8a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3eb8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb8a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3eb8a-125">Accept</span></span>|<span data-ttu-id="3eb8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb8a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3eb8a-127">Request body</span></span>
<span data-ttu-id="3eb8a-128">Geben Sie im Textkörper Anforderung für das Objekt [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="3eb8a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="3eb8a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3eb8a-130">Property</span></span>|<span data-ttu-id="3eb8a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3eb8a-131">Type</span></span>|<span data-ttu-id="3eb8a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3eb8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb8a-133">id</span><span class="sxs-lookup"><span data-stu-id="3eb8a-133">id</span></span>|<span data-ttu-id="3eb8a-134">String</span><span class="sxs-lookup"><span data-stu-id="3eb8a-134">String</span></span>|<span data-ttu-id="3eb8a-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3eb8a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3eb8a-136">displayName</span></span>|<span data-ttu-id="3eb8a-137">String</span><span class="sxs-lookup"><span data-stu-id="3eb8a-137">String</span></span>|<span data-ttu-id="3eb8a-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3eb8a-139">description</span><span class="sxs-lookup"><span data-stu-id="3eb8a-139">description</span></span>|<span data-ttu-id="3eb8a-140">String</span><span class="sxs-lookup"><span data-stu-id="3eb8a-140">String</span></span>|<span data-ttu-id="3eb8a-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3eb8a-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="3eb8a-142">requiresUserAuthentication</span></span>|<span data-ttu-id="3eb8a-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-143">Boolean</span></span>|<span data-ttu-id="3eb8a-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="3eb8a-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3eb8a-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="3eb8a-145">configurationEndpointUrl</span></span>|<span data-ttu-id="3eb8a-146">String</span><span class="sxs-lookup"><span data-stu-id="3eb8a-146">String</span></span>|<span data-ttu-id="3eb8a-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="3eb8a-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3eb8a-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="3eb8a-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="3eb8a-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-149">Boolean</span></span>|<span data-ttu-id="3eb8a-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="3eb8a-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3eb8a-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="3eb8a-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="3eb8a-152">isDefault</span></span>|<span data-ttu-id="3eb8a-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3eb8a-153">Boolean</span></span>|<span data-ttu-id="3eb8a-154">Gibt an, ob dies das Standardprofil ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="3eb8a-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-155">supervisedModeEnabled</span></span>|<span data-ttu-id="3eb8a-156">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-156">Boolean</span></span>|<span data-ttu-id="3eb8a-157">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="3eb8a-158">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="3eb8a-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="3eb8a-159">supportDepartment</span></span>|<span data-ttu-id="3eb8a-160">String</span><span class="sxs-lookup"><span data-stu-id="3eb8a-160">String</span></span>|<span data-ttu-id="3eb8a-161">Abteilung Supportinformationen</span><span class="sxs-lookup"><span data-stu-id="3eb8a-161">Support department information</span></span>|
|<span data-ttu-id="3eb8a-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-162">passCodeDisabled</span></span>|<span data-ttu-id="3eb8a-163">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-163">Boolean</span></span>|<span data-ttu-id="3eb8a-164">Gibt an, ob Kennung Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="3eb8a-165">isMandatory</span></span>|<span data-ttu-id="3eb8a-166">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-166">Boolean</span></span>|<span data-ttu-id="3eb8a-167">Gibt an, ob das Profil zwingend erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="3eb8a-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-168">locationDisabled</span></span>|<span data-ttu-id="3eb8a-169">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-169">Boolean</span></span>|<span data-ttu-id="3eb8a-170">Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3eb8a-171">supportPhoneNumber</span></span>|<span data-ttu-id="3eb8a-172">String</span><span class="sxs-lookup"><span data-stu-id="3eb8a-172">String</span></span>|<span data-ttu-id="3eb8a-173">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="3eb8a-173">Support phone number</span></span>|
|<span data-ttu-id="3eb8a-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="3eb8a-174">iTunesPairingMode</span></span>|[<span data-ttu-id="3eb8a-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="3eb8a-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="3eb8a-176">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="3eb8a-177">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="3eb8a-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-178">profileRemovalDisabled</span></span>|<span data-ttu-id="3eb8a-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-179">Boolean</span></span>|<span data-ttu-id="3eb8a-180">Gibt an, ob die Option Profil entfernen deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="3eb8a-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="3eb8a-181">managementCertificates</span></span>|<span data-ttu-id="3eb8a-182">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3eb8a-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="3eb8a-183">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="3eb8a-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="3eb8a-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3eb8a-184">restoreBlocked</span></span>|<span data-ttu-id="3eb8a-185">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-185">Boolean</span></span>|<span data-ttu-id="3eb8a-186">Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="3eb8a-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="3eb8a-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-188">Boolean</span></span>|<span data-ttu-id="3eb8a-189">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="3eb8a-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-190">appleIdDisabled</span></span>|<span data-ttu-id="3eb8a-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-191">Boolean</span></span>|<span data-ttu-id="3eb8a-192">Gibt an, ob Apple Id Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="3eb8a-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-194">Boolean</span></span>|<span data-ttu-id="3eb8a-195">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-196">touchIdDisabled</span></span>|<span data-ttu-id="3eb8a-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-197">Boolean</span></span>|<span data-ttu-id="3eb8a-198">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-199">applePayDisabled</span></span>|<span data-ttu-id="3eb8a-200">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-200">Boolean</span></span>|<span data-ttu-id="3eb8a-201">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-202">zoomDisabled</span></span>|<span data-ttu-id="3eb8a-203">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-203">Boolean</span></span>|<span data-ttu-id="3eb8a-204">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-205">siriDisabled</span></span>|<span data-ttu-id="3eb8a-206">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-206">Boolean</span></span>|<span data-ttu-id="3eb8a-207">Gibt an, ob Siri Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-208">diagnosticsDisabled</span></span>|<span data-ttu-id="3eb8a-209">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-209">Boolean</span></span>|<span data-ttu-id="3eb8a-210">Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="3eb8a-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="3eb8a-212">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-212">Boolean</span></span>|<span data-ttu-id="3eb8a-213">Gibt an, ob Mac OS-Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="3eb8a-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="3eb8a-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="3eb8a-215">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-215">Boolean</span></span>|<span data-ttu-id="3eb8a-216">Gibt an, ob die Datei Vault Mac OS deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="3eb8a-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="3eb8a-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="3eb8a-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="3eb8a-218">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-218">Boolean</span></span>|<span data-ttu-id="3eb8a-219">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="3eb8a-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="3eb8a-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="3eb8a-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="3eb8a-221">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb8a-221">Int32</span></span>|<span data-ttu-id="3eb8a-222">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="3eb8a-223">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="3eb8a-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="3eb8a-224">enableSharedIPad</span></span>|<span data-ttu-id="3eb8a-225">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3eb8a-225">Boolean</span></span>|<span data-ttu-id="3eb8a-226">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="3eb8a-227">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="3eb8a-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eb8a-228">Response</span></span>
<span data-ttu-id="3eb8a-229">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-229">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb8a-230">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3eb8a-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="3eb8a-231">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eb8a-231">Request</span></span>
<span data-ttu-id="3eb8a-232">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1231

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a><span data-ttu-id="3eb8a-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eb8a-233">Response</span></span>
<span data-ttu-id="3eb8a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3eb8a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```




