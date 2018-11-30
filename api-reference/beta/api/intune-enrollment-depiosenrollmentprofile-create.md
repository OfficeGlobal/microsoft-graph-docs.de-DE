---
title: Erstellen von depIOSEnrollmentProfile
description: Erstellen eines neuen DepIOSEnrollmentProfile-Objekts.
ms.openlocfilehash: 33acb1174438b08d3540b904460de5b27e957253
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060761"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="067ca-103">Erstellen von depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="067ca-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="067ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="067ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="067ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="067ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="067ca-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="067ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="067ca-107">Erstellen eines neuen [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="067ca-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="067ca-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="067ca-108">Prerequisites</span></span>
<span data-ttu-id="067ca-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="067ca-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="067ca-111">Permission type</span></span>|<span data-ttu-id="067ca-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="067ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="067ca-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="067ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="067ca-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="067ca-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="067ca-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="067ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="067ca-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="067ca-116">Not supported.</span></span>|
|<span data-ttu-id="067ca-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="067ca-117">Application</span></span>|<span data-ttu-id="067ca-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="067ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="067ca-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="067ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="067ca-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="067ca-120">Request headers</span></span>
|<span data-ttu-id="067ca-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="067ca-121">Header</span></span>|<span data-ttu-id="067ca-122">Wert</span><span class="sxs-lookup"><span data-stu-id="067ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="067ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="067ca-123">Authorization</span></span>|<span data-ttu-id="067ca-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="067ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="067ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="067ca-125">Accept</span></span>|<span data-ttu-id="067ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="067ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="067ca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="067ca-127">Request body</span></span>
<span data-ttu-id="067ca-128">Geben Sie im Textkörper Anforderung für das Objekt DepIOSEnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="067ca-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="067ca-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepIOSEnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="067ca-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="067ca-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="067ca-130">Property</span></span>|<span data-ttu-id="067ca-131">Typ</span><span class="sxs-lookup"><span data-stu-id="067ca-131">Type</span></span>|<span data-ttu-id="067ca-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="067ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="067ca-133">id</span><span class="sxs-lookup"><span data-stu-id="067ca-133">id</span></span>|<span data-ttu-id="067ca-134">String</span><span class="sxs-lookup"><span data-stu-id="067ca-134">String</span></span>|<span data-ttu-id="067ca-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="067ca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="067ca-136">displayName</span></span>|<span data-ttu-id="067ca-137">String</span><span class="sxs-lookup"><span data-stu-id="067ca-137">String</span></span>|<span data-ttu-id="067ca-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="067ca-139">description</span><span class="sxs-lookup"><span data-stu-id="067ca-139">description</span></span>|<span data-ttu-id="067ca-140">String</span><span class="sxs-lookup"><span data-stu-id="067ca-140">String</span></span>|<span data-ttu-id="067ca-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="067ca-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="067ca-142">requiresUserAuthentication</span></span>|<span data-ttu-id="067ca-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-143">Boolean</span></span>|<span data-ttu-id="067ca-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="067ca-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="067ca-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="067ca-145">configurationEndpointUrl</span></span>|<span data-ttu-id="067ca-146">String</span><span class="sxs-lookup"><span data-stu-id="067ca-146">String</span></span>|<span data-ttu-id="067ca-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="067ca-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="067ca-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="067ca-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="067ca-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-149">Boolean</span></span>|<span data-ttu-id="067ca-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="067ca-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="067ca-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="067ca-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="067ca-152">isDefault</span></span>|<span data-ttu-id="067ca-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067ca-153">Boolean</span></span>|<span data-ttu-id="067ca-154">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="067ca-155">supervisedModeEnabled</span></span>|<span data-ttu-id="067ca-156">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-156">Boolean</span></span>|<span data-ttu-id="067ca-157">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="067ca-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="067ca-158">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="067ca-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="067ca-159">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="067ca-160">supportDepartment</span></span>|<span data-ttu-id="067ca-161">String</span><span class="sxs-lookup"><span data-stu-id="067ca-161">String</span></span>|<span data-ttu-id="067ca-162">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-163">passCodeDisabled</span></span>|<span data-ttu-id="067ca-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-164">Boolean</span></span>|<span data-ttu-id="067ca-165">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="067ca-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="067ca-166">isMandatory</span></span>|<span data-ttu-id="067ca-167">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-167">Boolean</span></span>|<span data-ttu-id="067ca-168">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-169">locationDisabled</span></span>|<span data-ttu-id="067ca-170">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-170">Boolean</span></span>|<span data-ttu-id="067ca-171">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="067ca-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="067ca-172">supportPhoneNumber</span></span>|<span data-ttu-id="067ca-173">String</span><span class="sxs-lookup"><span data-stu-id="067ca-173">String</span></span>|<span data-ttu-id="067ca-174">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="067ca-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-175">profileRemovalDisabled</span></span>|<span data-ttu-id="067ca-176">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-176">Boolean</span></span>|<span data-ttu-id="067ca-177">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="067ca-178">restoreBlocked</span></span>|<span data-ttu-id="067ca-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-179">Boolean</span></span>|<span data-ttu-id="067ca-180">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-181">appleIdDisabled</span></span>|<span data-ttu-id="067ca-182">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-182">Boolean</span></span>|<span data-ttu-id="067ca-183">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="067ca-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="067ca-185">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-185">Boolean</span></span>|<span data-ttu-id="067ca-186">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-187">touchIdDisabled</span></span>|<span data-ttu-id="067ca-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-188">Boolean</span></span>|<span data-ttu-id="067ca-189">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-190">applePayDisabled</span></span>|<span data-ttu-id="067ca-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-191">Boolean</span></span>|<span data-ttu-id="067ca-192">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-193">zoomDisabled</span></span>|<span data-ttu-id="067ca-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-194">Boolean</span></span>|<span data-ttu-id="067ca-195">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-196">siriDisabled</span></span>|<span data-ttu-id="067ca-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-197">Boolean</span></span>|<span data-ttu-id="067ca-198">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="067ca-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-199">diagnosticsDisabled</span></span>|<span data-ttu-id="067ca-200">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-200">Boolean</span></span>|<span data-ttu-id="067ca-201">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="067ca-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="067ca-202">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="067ca-202">iTunesPairingMode</span></span>|[<span data-ttu-id="067ca-203">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="067ca-203">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="067ca-204">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="067ca-204">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="067ca-205">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="067ca-205">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="067ca-206">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="067ca-206">managementCertificates</span></span>|<span data-ttu-id="067ca-207">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="067ca-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="067ca-208">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="067ca-208">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="067ca-209">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="067ca-209">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="067ca-210">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-210">Boolean</span></span>|<span data-ttu-id="067ca-211">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="067ca-211">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="067ca-212">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="067ca-212">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="067ca-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-213">Boolean</span></span>|<span data-ttu-id="067ca-214">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="067ca-214">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="067ca-215">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="067ca-215">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="067ca-216">Int32</span><span class="sxs-lookup"><span data-stu-id="067ca-216">Int32</span></span>|<span data-ttu-id="067ca-217">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="067ca-217">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="067ca-218">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="067ca-218">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="067ca-219">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="067ca-219">enableSharedIPad</span></span>|<span data-ttu-id="067ca-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-220">Boolean</span></span>|<span data-ttu-id="067ca-221">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="067ca-221">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="067ca-222">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="067ca-222">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="067ca-223">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="067ca-223">companyPortalVppTokenId</span></span>|<span data-ttu-id="067ca-224">String</span><span class="sxs-lookup"><span data-stu-id="067ca-224">String</span></span>|<span data-ttu-id="067ca-225">Wenn festgelegt ist, gibt an, welche Vpp Token zum Bereitstellen der Unternehmensportal mit Gerät-Lizenzierung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="067ca-225">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="067ca-226">'EnableAuthenticationViaCompanyPortal' muss für diese Eigenschaft festgelegt werden soll festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="067ca-226">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="067ca-227">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="067ca-227">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="067ca-228">Boolesch</span><span class="sxs-lookup"><span data-stu-id="067ca-228">Boolean</span></span>|<span data-ttu-id="067ca-229">Weist das Gerät zum Aktivieren der einzelnen app-Modus und Anwenden von app-Sperre während der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="067ca-229">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="067ca-230">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="067ca-230">Default is false.</span></span> <span data-ttu-id="067ca-231">'EnableAuthenticationViaCompanyPortal' und 'CompanyPortalVppTokenId' müssen für diese Eigenschaft festgelegt werden soll, festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="067ca-231">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|



## <a name="response"></a><span data-ttu-id="067ca-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="067ca-232">Response</span></span>
<span data-ttu-id="067ca-233">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="067ca-233">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="067ca-234">Beispiel</span><span class="sxs-lookup"><span data-stu-id="067ca-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="067ca-235">Anforderung</span><span class="sxs-lookup"><span data-stu-id="067ca-235">Request</span></span>
<span data-ttu-id="067ca-236">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="067ca-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1329

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a><span data-ttu-id="067ca-237">Antwort</span><span class="sxs-lookup"><span data-stu-id="067ca-237">Response</span></span>
<span data-ttu-id="067ca-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="067ca-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true
}
```




