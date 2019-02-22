---
title: DepEnrollmentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines depEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e033d5f4601020e677e31a40b1d46c1e7652283
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171449"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="b9703-103">DepEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b9703-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="b9703-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9703-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9703-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b9703-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9703-106">Aktualisieren der Eigenschaften eines [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9703-106">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9703-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9703-107">Prerequisites</span></span>
<span data-ttu-id="b9703-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9703-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9703-110">Permission type</span></span>|<span data-ttu-id="b9703-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9703-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9703-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9703-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9703-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9703-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9703-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9703-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9703-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9703-115">Not supported.</span></span>|
|<span data-ttu-id="b9703-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9703-116">Application</span></span>|<span data-ttu-id="b9703-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9703-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9703-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9703-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="b9703-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9703-119">Request headers</span></span>
|<span data-ttu-id="b9703-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9703-120">Header</span></span>|<span data-ttu-id="b9703-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9703-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9703-122">Authorization</span></span>|<span data-ttu-id="b9703-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9703-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9703-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9703-124">Accept</span></span>|<span data-ttu-id="b9703-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9703-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9703-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9703-126">Request body</span></span>
<span data-ttu-id="b9703-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b9703-127">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="b9703-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b9703-128">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="b9703-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9703-129">Property</span></span>|<span data-ttu-id="b9703-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9703-130">Type</span></span>|<span data-ttu-id="b9703-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9703-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9703-132">id</span><span class="sxs-lookup"><span data-stu-id="b9703-132">id</span></span>|<span data-ttu-id="b9703-133">string</span><span class="sxs-lookup"><span data-stu-id="b9703-133">String</span></span>|<span data-ttu-id="b9703-134">Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.</span><span class="sxs-lookup"><span data-stu-id="b9703-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b9703-135">displayName</span></span>|<span data-ttu-id="b9703-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9703-136">String</span></span>|<span data-ttu-id="b9703-137">Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="b9703-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-138">description</span><span class="sxs-lookup"><span data-stu-id="b9703-138">description</span></span>|<span data-ttu-id="b9703-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9703-139">String</span></span>|<span data-ttu-id="b9703-140">Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="b9703-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b9703-141">requiresUserAuthentication</span></span>|<span data-ttu-id="b9703-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-142">Boolean</span></span>|<span data-ttu-id="b9703-143">Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="b9703-144">configurationEndpointUrl</span></span>|<span data-ttu-id="b9703-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9703-145">String</span></span>|<span data-ttu-id="b9703-146">Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung</span><span class="sxs-lookup"><span data-stu-id="b9703-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b9703-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b9703-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-148">Boolean</span></span>|<span data-ttu-id="b9703-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b9703-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="b9703-150">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b9703-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="b9703-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="b9703-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-152">Boolean</span></span>|<span data-ttu-id="b9703-153">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="b9703-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b9703-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="b9703-154">isDefault</span></span>|<span data-ttu-id="b9703-155">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-155">Boolean</span></span>|<span data-ttu-id="b9703-156">Gibt an, ob dies das Standardprofil ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="b9703-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="b9703-157">supervisedModeEnabled</span></span>|<span data-ttu-id="b9703-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-158">Boolean</span></span>|<span data-ttu-id="b9703-159">Überwachter Modus, true, um zu aktivieren, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="b9703-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="b9703-160">Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="b9703-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="b9703-161">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="b9703-161">supportDepartment</span></span>|<span data-ttu-id="b9703-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9703-162">String</span></span>|<span data-ttu-id="b9703-163">Informationen zur Support Abteilung</span><span class="sxs-lookup"><span data-stu-id="b9703-163">Support department information</span></span>|
|<span data-ttu-id="b9703-164">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-164">passCodeDisabled</span></span>|<span data-ttu-id="b9703-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-165">Boolean</span></span>|<span data-ttu-id="b9703-166">Gibt an, ob der Bereich "Passcode" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-167">isMandatory</span><span class="sxs-lookup"><span data-stu-id="b9703-167">isMandatory</span></span>|<span data-ttu-id="b9703-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-168">Boolean</span></span>|<span data-ttu-id="b9703-169">Gibt an, ob das Profil obligatorisch ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="b9703-170">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-170">locationDisabled</span></span>|<span data-ttu-id="b9703-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-171">Boolean</span></span>|<span data-ttu-id="b9703-172">Gibt an, ob der Standortdienst-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b9703-173">supportPhoneNumber</span></span>|<span data-ttu-id="b9703-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9703-174">String</span></span>|<span data-ttu-id="b9703-175">Support-Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="b9703-175">Support phone number</span></span>|
|<span data-ttu-id="b9703-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="b9703-176">iTunesPairingMode</span></span>|[<span data-ttu-id="b9703-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="b9703-177">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="b9703-178">Gibt den iTunes-paarungsmodus an.</span><span class="sxs-lookup"><span data-stu-id="b9703-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="b9703-179">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="b9703-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="b9703-180">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-180">profileRemovalDisabled</span></span>|<span data-ttu-id="b9703-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-181">Boolean</span></span>|<span data-ttu-id="b9703-182">Gibt an, ob die Profil Entfernungs Option deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="b9703-183">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="b9703-183">managementCertificates</span></span>|<span data-ttu-id="b9703-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9703-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="b9703-185">Verwaltungszertifikate für Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="b9703-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="b9703-186">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b9703-186">restoreBlocked</span></span>|<span data-ttu-id="b9703-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-187">Boolean</span></span>|<span data-ttu-id="b9703-188">Gibt an, ob der wiederHerstellungs-Setup Bereich blockiert ist</span><span class="sxs-lookup"><span data-stu-id="b9703-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="b9703-189">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="b9703-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-190">Boolean</span></span>|<span data-ttu-id="b9703-191">Gibt an, ob die Wiederherstellung von Android deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="b9703-192">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-192">appleIdDisabled</span></span>|<span data-ttu-id="b9703-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-193">Boolean</span></span>|<span data-ttu-id="b9703-194">Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-195">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="b9703-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-196">Boolean</span></span>|<span data-ttu-id="b9703-197">Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-198">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-198">touchIdDisabled</span></span>|<span data-ttu-id="b9703-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-199">Boolean</span></span>|<span data-ttu-id="b9703-200">Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-201">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-201">applePayDisabled</span></span>|<span data-ttu-id="b9703-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-202">Boolean</span></span>|<span data-ttu-id="b9703-203">Gibt an, ob der Apple Pay-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-204">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-204">zoomDisabled</span></span>|<span data-ttu-id="b9703-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-205">Boolean</span></span>|<span data-ttu-id="b9703-206">Gibt an, ob der Zoom-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-207">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-207">siriDisabled</span></span>|<span data-ttu-id="b9703-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-208">Boolean</span></span>|<span data-ttu-id="b9703-209">Gibt an, ob der Siri-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-210">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-210">diagnosticsDisabled</span></span>|<span data-ttu-id="b9703-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-211">Boolean</span></span>|<span data-ttu-id="b9703-212">Gibt an, ob der Diagnose-Setup Bereich deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="b9703-213">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="b9703-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-214">Boolean</span></span>|<span data-ttu-id="b9703-215">Gibt an, ob die Mac OS-Registrierung deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="b9703-216">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="b9703-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="b9703-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-217">Boolean</span></span>|<span data-ttu-id="b9703-218">Gibt an, ob das Mac OS-Dateidepot deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b9703-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="b9703-219">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="b9703-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="b9703-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-220">Boolean</span></span>|<span data-ttu-id="b9703-221">Gibt an, ob das Gerät auf die konfigurierte Bestätigung warten muss.</span><span class="sxs-lookup"><span data-stu-id="b9703-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="b9703-222">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="b9703-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="b9703-223">Int32</span><span class="sxs-lookup"><span data-stu-id="b9703-223">Int32</span></span>|<span data-ttu-id="b9703-224">Dies gibt die maximale Anzahl von Benutzern an, die ein freigegebenes iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="b9703-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="b9703-225">Gilt nur für den freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="b9703-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="b9703-226">Enablesharedipad wurden</span><span class="sxs-lookup"><span data-stu-id="b9703-226">enableSharedIPad</span></span>|<span data-ttu-id="b9703-227">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9703-227">Boolean</span></span>|<span data-ttu-id="b9703-228">Dieser Wert gibt an, ob das Gerät in einen Modus eingeschrieben werden soll, der mehrere Benutzerszenarien ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="b9703-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="b9703-229">Gilt nur für freigegebene iPads.</span><span class="sxs-lookup"><span data-stu-id="b9703-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="b9703-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9703-230">Response</span></span>
<span data-ttu-id="b9703-231">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9703-231">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9703-232">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9703-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9703-233">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9703-233">Request</span></span>
<span data-ttu-id="b9703-234">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9703-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9703-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9703-235">Response</span></span>
<span data-ttu-id="b9703-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9703-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




