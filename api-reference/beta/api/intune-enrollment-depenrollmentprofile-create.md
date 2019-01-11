---
title: Erstellen von depEnrollmentProfile
description: Erstellen eines neuen DepEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c7936af86b25fbf0c4e022adef0bc387c56b196
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828147"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="d2806-103">Erstellen von depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2806-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="d2806-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d2806-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2806-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2806-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2806-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2806-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2806-107">Erstellen eines neuen [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d2806-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2806-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d2806-108">Prerequisites</span></span>
<span data-ttu-id="d2806-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2806-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2806-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2806-111">Permission type</span></span>|<span data-ttu-id="d2806-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2806-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2806-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2806-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2806-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2806-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d2806-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2806-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2806-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2806-116">Not supported.</span></span>|
|<span data-ttu-id="d2806-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2806-117">Application</span></span>|<span data-ttu-id="d2806-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2806-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2806-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2806-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d2806-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2806-120">Request headers</span></span>
|<span data-ttu-id="d2806-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2806-121">Header</span></span>|<span data-ttu-id="d2806-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d2806-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2806-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2806-123">Authorization</span></span>|<span data-ttu-id="d2806-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d2806-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2806-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d2806-125">Accept</span></span>|<span data-ttu-id="d2806-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2806-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2806-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2806-127">Request body</span></span>
<span data-ttu-id="d2806-128">Geben Sie im Textkörper Anforderung für das Objekt DepEnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d2806-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="d2806-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepEnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="d2806-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="d2806-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2806-130">Property</span></span>|<span data-ttu-id="d2806-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d2806-131">Type</span></span>|<span data-ttu-id="d2806-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2806-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2806-133">id</span><span class="sxs-lookup"><span data-stu-id="d2806-133">id</span></span>|<span data-ttu-id="d2806-134">String</span><span class="sxs-lookup"><span data-stu-id="d2806-134">String</span></span>|<span data-ttu-id="d2806-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d2806-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d2806-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d2806-136">displayName</span></span>|<span data-ttu-id="d2806-137">String</span><span class="sxs-lookup"><span data-stu-id="d2806-137">String</span></span>|<span data-ttu-id="d2806-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d2806-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d2806-139">description</span><span class="sxs-lookup"><span data-stu-id="d2806-139">description</span></span>|<span data-ttu-id="d2806-140">String</span><span class="sxs-lookup"><span data-stu-id="d2806-140">String</span></span>|<span data-ttu-id="d2806-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d2806-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d2806-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d2806-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d2806-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-143">Boolean</span></span>|<span data-ttu-id="d2806-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="d2806-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d2806-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d2806-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d2806-146">String</span><span class="sxs-lookup"><span data-stu-id="d2806-146">String</span></span>|<span data-ttu-id="d2806-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d2806-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d2806-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d2806-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d2806-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-149">Boolean</span></span>|<span data-ttu-id="d2806-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="d2806-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d2806-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d2806-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d2806-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="d2806-152">isDefault</span></span>|<span data-ttu-id="d2806-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-153">Boolean</span></span>|<span data-ttu-id="d2806-154">Gibt an, ob dies das Standardprofil ist</span><span class="sxs-lookup"><span data-stu-id="d2806-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="d2806-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d2806-155">supervisedModeEnabled</span></span>|<span data-ttu-id="d2806-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-156">Boolean</span></span>|<span data-ttu-id="d2806-157">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="d2806-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d2806-158">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="d2806-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="d2806-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="d2806-159">supportDepartment</span></span>|<span data-ttu-id="d2806-160">String</span><span class="sxs-lookup"><span data-stu-id="d2806-160">String</span></span>|<span data-ttu-id="d2806-161">Abteilung Supportinformationen</span><span class="sxs-lookup"><span data-stu-id="d2806-161">Support department information</span></span>|
|<span data-ttu-id="d2806-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-162">passCodeDisabled</span></span>|<span data-ttu-id="d2806-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-163">Boolean</span></span>|<span data-ttu-id="d2806-164">Gibt an, ob Kennung Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="d2806-165">isMandatory</span></span>|<span data-ttu-id="d2806-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-166">Boolean</span></span>|<span data-ttu-id="d2806-167">Gibt an, ob das Profil zwingend erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d2806-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="d2806-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-168">locationDisabled</span></span>|<span data-ttu-id="d2806-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-169">Boolean</span></span>|<span data-ttu-id="d2806-170">Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d2806-171">supportPhoneNumber</span></span>|<span data-ttu-id="d2806-172">String</span><span class="sxs-lookup"><span data-stu-id="d2806-172">String</span></span>|<span data-ttu-id="d2806-173">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="d2806-173">Support phone number</span></span>|
|<span data-ttu-id="d2806-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d2806-174">iTunesPairingMode</span></span>|[<span data-ttu-id="d2806-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d2806-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="d2806-176">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="d2806-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d2806-177">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="d2806-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d2806-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-178">profileRemovalDisabled</span></span>|<span data-ttu-id="d2806-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-179">Boolean</span></span>|<span data-ttu-id="d2806-180">Gibt an, ob die Option Profil entfernen deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="d2806-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="d2806-181">managementCertificates</span></span>|<span data-ttu-id="d2806-182">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d2806-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d2806-183">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="d2806-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d2806-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d2806-184">restoreBlocked</span></span>|<span data-ttu-id="d2806-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-185">Boolean</span></span>|<span data-ttu-id="d2806-186">Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="d2806-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="d2806-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d2806-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-188">Boolean</span></span>|<span data-ttu-id="d2806-189">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d2806-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-190">appleIdDisabled</span></span>|<span data-ttu-id="d2806-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-191">Boolean</span></span>|<span data-ttu-id="d2806-192">Gibt an, ob Apple Id Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d2806-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-194">Boolean</span></span>|<span data-ttu-id="d2806-195">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-196">touchIdDisabled</span></span>|<span data-ttu-id="d2806-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-197">Boolean</span></span>|<span data-ttu-id="d2806-198">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-199">applePayDisabled</span></span>|<span data-ttu-id="d2806-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-200">Boolean</span></span>|<span data-ttu-id="d2806-201">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-202">zoomDisabled</span></span>|<span data-ttu-id="d2806-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-203">Boolean</span></span>|<span data-ttu-id="d2806-204">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-205">siriDisabled</span></span>|<span data-ttu-id="d2806-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-206">Boolean</span></span>|<span data-ttu-id="d2806-207">Gibt an, ob Siri Setup Bereich deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-208">diagnosticsDisabled</span></span>|<span data-ttu-id="d2806-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-209">Boolean</span></span>|<span data-ttu-id="d2806-210">Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="d2806-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="d2806-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-212">Boolean</span></span>|<span data-ttu-id="d2806-213">Gibt an, ob Mac OS-Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="d2806-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="d2806-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="d2806-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-215">Boolean</span></span>|<span data-ttu-id="d2806-216">Gibt an, ob die Datei Vault Mac OS deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d2806-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="d2806-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="d2806-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d2806-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-218">Boolean</span></span>|<span data-ttu-id="d2806-219">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="d2806-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d2806-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="d2806-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d2806-221">Int32</span><span class="sxs-lookup"><span data-stu-id="d2806-221">Int32</span></span>|<span data-ttu-id="d2806-222">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="d2806-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d2806-223">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="d2806-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d2806-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="d2806-224">enableSharedIPad</span></span>|<span data-ttu-id="d2806-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2806-225">Boolean</span></span>|<span data-ttu-id="d2806-226">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="d2806-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d2806-227">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="d2806-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="d2806-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2806-228">Response</span></span>
<span data-ttu-id="d2806-229">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d2806-229">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2806-230">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2806-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2806-231">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2806-231">Request</span></span>
<span data-ttu-id="d2806-232">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2806-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1290

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="d2806-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2806-233">Response</span></span>
<span data-ttu-id="d2806-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2806-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





