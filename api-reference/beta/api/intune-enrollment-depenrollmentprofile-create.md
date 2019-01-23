---
title: Erstellen von depEnrollmentProfile
description: Erstellen eines neuen DepEnrollmentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bc6b11a8367ff28b4e4b9957879e251cb939c7e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416314"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="ae228-103">Erstellen von depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ae228-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="ae228-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ae228-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae228-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae228-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae228-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae228-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae228-107">Erstellen eines neuen [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae228-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae228-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae228-108">Prerequisites</span></span>
<span data-ttu-id="ae228-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae228-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae228-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae228-111">Permission type</span></span>|<span data-ttu-id="ae228-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae228-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae228-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae228-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae228-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae228-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae228-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae228-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae228-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae228-116">Not supported.</span></span>|
|<span data-ttu-id="ae228-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae228-117">Application</span></span>|<span data-ttu-id="ae228-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae228-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae228-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae228-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ae228-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae228-120">Request headers</span></span>
|<span data-ttu-id="ae228-121">Header</span><span class="sxs-lookup"><span data-stu-id="ae228-121">Header</span></span>|<span data-ttu-id="ae228-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ae228-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae228-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ae228-123">Authorization</span></span>|<span data-ttu-id="ae228-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae228-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae228-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae228-125">Accept</span></span>|<span data-ttu-id="ae228-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae228-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae228-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae228-127">Request body</span></span>
<span data-ttu-id="ae228-128">Geben Sie im Textkörper Anforderung für das Objekt DepEnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ae228-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="ae228-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepEnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae228-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="ae228-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae228-130">Property</span></span>|<span data-ttu-id="ae228-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ae228-131">Type</span></span>|<span data-ttu-id="ae228-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae228-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae228-133">id</span><span class="sxs-lookup"><span data-stu-id="ae228-133">id</span></span>|<span data-ttu-id="ae228-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae228-134">String</span></span>|<span data-ttu-id="ae228-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ae228-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ae228-136">displayName</span></span>|<span data-ttu-id="ae228-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae228-137">String</span></span>|<span data-ttu-id="ae228-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ae228-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-139">description</span><span class="sxs-lookup"><span data-stu-id="ae228-139">description</span></span>|<span data-ttu-id="ae228-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae228-140">String</span></span>|<span data-ttu-id="ae228-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ae228-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ae228-142">requiresUserAuthentication</span></span>|<span data-ttu-id="ae228-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-143">Boolean</span></span>|<span data-ttu-id="ae228-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="ae228-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ae228-145">configurationEndpointUrl</span></span>|<span data-ttu-id="ae228-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae228-146">String</span></span>|<span data-ttu-id="ae228-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="ae228-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ae228-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ae228-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-149">Boolean</span></span>|<span data-ttu-id="ae228-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="ae228-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ae228-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ae228-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ae228-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ae228-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-153">Boolean</span></span>|<span data-ttu-id="ae228-154">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="ae228-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ae228-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="ae228-155">isDefault</span></span>|<span data-ttu-id="ae228-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-156">Boolean</span></span>|<span data-ttu-id="ae228-157">Gibt an, ob dies das Standardprofil ist</span><span class="sxs-lookup"><span data-stu-id="ae228-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ae228-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ae228-158">supervisedModeEnabled</span></span>|<span data-ttu-id="ae228-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-159">Boolean</span></span>|<span data-ttu-id="ae228-160">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="ae228-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ae228-161">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="ae228-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ae228-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ae228-162">supportDepartment</span></span>|<span data-ttu-id="ae228-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae228-163">String</span></span>|<span data-ttu-id="ae228-164">Abteilung Supportinformationen</span><span class="sxs-lookup"><span data-stu-id="ae228-164">Support department information</span></span>|
|<span data-ttu-id="ae228-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-165">passCodeDisabled</span></span>|<span data-ttu-id="ae228-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-166">Boolean</span></span>|<span data-ttu-id="ae228-167">Gibt an, ob Kennung Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ae228-168">isMandatory</span></span>|<span data-ttu-id="ae228-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-169">Boolean</span></span>|<span data-ttu-id="ae228-170">Gibt an, ob das Profil zwingend erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ae228-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ae228-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-171">locationDisabled</span></span>|<span data-ttu-id="ae228-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-172">Boolean</span></span>|<span data-ttu-id="ae228-173">Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ae228-174">supportPhoneNumber</span></span>|<span data-ttu-id="ae228-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae228-175">String</span></span>|<span data-ttu-id="ae228-176">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="ae228-176">Support phone number</span></span>|
|<span data-ttu-id="ae228-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ae228-177">iTunesPairingMode</span></span>|[<span data-ttu-id="ae228-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ae228-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="ae228-179">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="ae228-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="ae228-180">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="ae228-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="ae228-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-181">profileRemovalDisabled</span></span>|<span data-ttu-id="ae228-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-182">Boolean</span></span>|<span data-ttu-id="ae228-183">Gibt an, ob die Option Profil entfernen deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ae228-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="ae228-184">managementCertificates</span></span>|<span data-ttu-id="ae228-185">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ae228-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="ae228-186">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="ae228-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="ae228-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ae228-187">restoreBlocked</span></span>|<span data-ttu-id="ae228-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-188">Boolean</span></span>|<span data-ttu-id="ae228-189">Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="ae228-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ae228-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="ae228-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-191">Boolean</span></span>|<span data-ttu-id="ae228-192">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="ae228-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-193">appleIdDisabled</span></span>|<span data-ttu-id="ae228-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-194">Boolean</span></span>|<span data-ttu-id="ae228-195">Gibt an, ob Apple Id Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ae228-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-197">Boolean</span></span>|<span data-ttu-id="ae228-198">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-199">touchIdDisabled</span></span>|<span data-ttu-id="ae228-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-200">Boolean</span></span>|<span data-ttu-id="ae228-201">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-202">applePayDisabled</span></span>|<span data-ttu-id="ae228-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-203">Boolean</span></span>|<span data-ttu-id="ae228-204">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-205">zoomDisabled</span></span>|<span data-ttu-id="ae228-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-206">Boolean</span></span>|<span data-ttu-id="ae228-207">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-208">siriDisabled</span></span>|<span data-ttu-id="ae228-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-209">Boolean</span></span>|<span data-ttu-id="ae228-210">Gibt an, ob Siri Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-211">diagnosticsDisabled</span></span>|<span data-ttu-id="ae228-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-212">Boolean</span></span>|<span data-ttu-id="ae228-213">Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="ae228-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="ae228-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-215">Boolean</span></span>|<span data-ttu-id="ae228-216">Gibt an, ob Mac OS-Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="ae228-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="ae228-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="ae228-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-218">Boolean</span></span>|<span data-ttu-id="ae228-219">Gibt an, ob die Datei Vault Mac OS deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ae228-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="ae228-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="ae228-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="ae228-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-221">Boolean</span></span>|<span data-ttu-id="ae228-222">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="ae228-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="ae228-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="ae228-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="ae228-224">Int32</span><span class="sxs-lookup"><span data-stu-id="ae228-224">Int32</span></span>|<span data-ttu-id="ae228-225">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="ae228-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="ae228-226">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="ae228-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="ae228-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="ae228-227">enableSharedIPad</span></span>|<span data-ttu-id="ae228-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae228-228">Boolean</span></span>|<span data-ttu-id="ae228-229">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="ae228-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="ae228-230">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="ae228-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="ae228-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae228-231">Response</span></span>
<span data-ttu-id="ae228-232">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ae228-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae228-233">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae228-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae228-234">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae228-234">Request</span></span>
<span data-ttu-id="ae228-235">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae228-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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

### <a name="response"></a><span data-ttu-id="ae228-236">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae228-236">Response</span></span>
<span data-ttu-id="ae228-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae228-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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




