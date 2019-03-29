---
title: DepEnrollmentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines depEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70690403a2c7d2855ce94ac0c58f99d214a7bf7f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969421"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="61466-103">DepEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="61466-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="61466-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61466-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61466-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="61466-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61466-106">Aktualisieren der Eigenschaften eines [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="61466-106">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61466-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="61466-107">Prerequisites</span></span>
<span data-ttu-id="61466-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61466-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61466-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61466-110">Permission type</span></span>|<span data-ttu-id="61466-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61466-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61466-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61466-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61466-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61466-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61466-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61466-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61466-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61466-115">Not supported.</span></span>|
|<span data-ttu-id="61466-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61466-116">Application</span></span>|<span data-ttu-id="61466-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61466-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61466-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61466-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="61466-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61466-119">Request headers</span></span>
|<span data-ttu-id="61466-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="61466-120">Header</span></span>|<span data-ttu-id="61466-121">Wert</span><span class="sxs-lookup"><span data-stu-id="61466-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61466-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61466-122">Authorization</span></span>|<span data-ttu-id="61466-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="61466-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61466-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="61466-124">Accept</span></span>|<span data-ttu-id="61466-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61466-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61466-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61466-126">Request body</span></span>
<span data-ttu-id="61466-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="61466-127">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="61466-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="61466-128">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="61466-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61466-129">Property</span></span>|<span data-ttu-id="61466-130">Typ</span><span class="sxs-lookup"><span data-stu-id="61466-130">Type</span></span>|<span data-ttu-id="61466-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61466-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61466-132">id</span><span class="sxs-lookup"><span data-stu-id="61466-132">id</span></span>|<span data-ttu-id="61466-133">String</span><span class="sxs-lookup"><span data-stu-id="61466-133">String</span></span>|<span data-ttu-id="61466-134">Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.</span><span class="sxs-lookup"><span data-stu-id="61466-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-135">displayName</span><span class="sxs-lookup"><span data-stu-id="61466-135">displayName</span></span>|<span data-ttu-id="61466-136">String</span><span class="sxs-lookup"><span data-stu-id="61466-136">String</span></span>|<span data-ttu-id="61466-137">Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="61466-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-138">description</span><span class="sxs-lookup"><span data-stu-id="61466-138">description</span></span>|<span data-ttu-id="61466-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61466-139">String</span></span>|<span data-ttu-id="61466-140">Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="61466-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="61466-141">requiresUserAuthentication</span></span>|<span data-ttu-id="61466-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-142">Boolean</span></span>|<span data-ttu-id="61466-143">Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="61466-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="61466-144">configurationEndpointUrl</span></span>|<span data-ttu-id="61466-145">String</span><span class="sxs-lookup"><span data-stu-id="61466-145">String</span></span>|<span data-ttu-id="61466-146">Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung</span><span class="sxs-lookup"><span data-stu-id="61466-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="61466-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="61466-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-148">Boolean</span></span>|<span data-ttu-id="61466-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="61466-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="61466-150">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61466-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="61466-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="61466-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-152">Boolean</span></span>|<span data-ttu-id="61466-153">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="61466-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61466-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="61466-154">isDefault</span></span>|<span data-ttu-id="61466-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="61466-155">Boolean</span></span>|<span data-ttu-id="61466-156">Gibt an, ob dies das Standardprofil ist.</span><span class="sxs-lookup"><span data-stu-id="61466-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="61466-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="61466-157">supervisedModeEnabled</span></span>|<span data-ttu-id="61466-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-158">Boolean</span></span>|<span data-ttu-id="61466-159">Überwachter Modus, true, um zu aktivieren, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="61466-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="61466-160">Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="61466-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="61466-161">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="61466-161">supportDepartment</span></span>|<span data-ttu-id="61466-162">String</span><span class="sxs-lookup"><span data-stu-id="61466-162">String</span></span>|<span data-ttu-id="61466-163">Informationen zur Support Abteilung</span><span class="sxs-lookup"><span data-stu-id="61466-163">Support department information</span></span>|
|<span data-ttu-id="61466-164">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-164">passCodeDisabled</span></span>|<span data-ttu-id="61466-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-165">Boolean</span></span>|<span data-ttu-id="61466-166">Gibt an, ob der Bereich "Passcode" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="61466-167">isMandatory</span><span class="sxs-lookup"><span data-stu-id="61466-167">isMandatory</span></span>|<span data-ttu-id="61466-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-168">Boolean</span></span>|<span data-ttu-id="61466-169">Gibt an, ob das Profil obligatorisch ist.</span><span class="sxs-lookup"><span data-stu-id="61466-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="61466-170">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-170">locationDisabled</span></span>|<span data-ttu-id="61466-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-171">Boolean</span></span>|<span data-ttu-id="61466-172">Gibt an, ob der Standortdienst-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="61466-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="61466-173">supportPhoneNumber</span></span>|<span data-ttu-id="61466-174">String</span><span class="sxs-lookup"><span data-stu-id="61466-174">String</span></span>|<span data-ttu-id="61466-175">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="61466-175">Support phone number</span></span>|
|<span data-ttu-id="61466-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="61466-176">iTunesPairingMode</span></span>|[<span data-ttu-id="61466-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="61466-177">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="61466-178">Gibt den iTunes-paarungsmodus an.</span><span class="sxs-lookup"><span data-stu-id="61466-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="61466-179">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="61466-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="61466-180">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-180">profileRemovalDisabled</span></span>|<span data-ttu-id="61466-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-181">Boolean</span></span>|<span data-ttu-id="61466-182">Gibt an, ob die Profil Entfernungs Option deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="61466-183">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="61466-183">managementCertificates</span></span>|<span data-ttu-id="61466-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="61466-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="61466-185">Verwaltungszertifikate für Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="61466-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="61466-186">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="61466-186">restoreBlocked</span></span>|<span data-ttu-id="61466-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-187">Boolean</span></span>|<span data-ttu-id="61466-188">Gibt an, ob der wiederHerstellungs-Setup Bereich blockiert ist</span><span class="sxs-lookup"><span data-stu-id="61466-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="61466-189">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="61466-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-190">Boolean</span></span>|<span data-ttu-id="61466-191">Gibt an, ob die Wiederherstellung von Android deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="61466-192">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-192">appleIdDisabled</span></span>|<span data-ttu-id="61466-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-193">Boolean</span></span>|<span data-ttu-id="61466-194">Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="61466-195">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="61466-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-196">Boolean</span></span>|<span data-ttu-id="61466-197">Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="61466-198">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-198">touchIdDisabled</span></span>|<span data-ttu-id="61466-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-199">Boolean</span></span>|<span data-ttu-id="61466-200">Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="61466-201">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-201">applePayDisabled</span></span>|<span data-ttu-id="61466-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-202">Boolean</span></span>|<span data-ttu-id="61466-203">Gibt an, ob der Apple Pay-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="61466-204">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-204">zoomDisabled</span></span>|<span data-ttu-id="61466-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-205">Boolean</span></span>|<span data-ttu-id="61466-206">Gibt an, ob der Zoom-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="61466-207">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-207">siriDisabled</span></span>|<span data-ttu-id="61466-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-208">Boolean</span></span>|<span data-ttu-id="61466-209">Gibt an, ob der Siri-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="61466-210">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-210">diagnosticsDisabled</span></span>|<span data-ttu-id="61466-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-211">Boolean</span></span>|<span data-ttu-id="61466-212">Gibt an, ob der Diagnose-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="61466-213">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="61466-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-214">Boolean</span></span>|<span data-ttu-id="61466-215">Gibt an, ob die Mac OS-Registrierung deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="61466-216">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="61466-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="61466-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-217">Boolean</span></span>|<span data-ttu-id="61466-218">Gibt an, ob das Mac OS-Dateidepot deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="61466-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="61466-219">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="61466-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="61466-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-220">Boolean</span></span>|<span data-ttu-id="61466-221">Gibt an, ob das Gerät auf die konfigurierte Bestätigung warten muss.</span><span class="sxs-lookup"><span data-stu-id="61466-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="61466-222">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="61466-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="61466-223">Int32</span><span class="sxs-lookup"><span data-stu-id="61466-223">Int32</span></span>|<span data-ttu-id="61466-224">Dies gibt die maximale Anzahl von Benutzern an, die ein freigegebenes iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="61466-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="61466-225">Gilt nur für den freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="61466-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="61466-226">Enablesharedipad wurden</span><span class="sxs-lookup"><span data-stu-id="61466-226">enableSharedIPad</span></span>|<span data-ttu-id="61466-227">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61466-227">Boolean</span></span>|<span data-ttu-id="61466-228">Dieser Wert gibt an, ob das Gerät in einen Modus eingeschrieben werden soll, der mehrere Benutzerszenarien ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="61466-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="61466-229">Gilt nur für freigegebene iPads.</span><span class="sxs-lookup"><span data-stu-id="61466-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="61466-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="61466-230">Response</span></span>
<span data-ttu-id="61466-231">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="61466-231">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61466-232">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61466-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="61466-233">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61466-233">Request</span></span>
<span data-ttu-id="61466-234">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61466-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
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

### <a name="response"></a><span data-ttu-id="61466-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="61466-235">Response</span></span>
<span data-ttu-id="61466-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61466-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




