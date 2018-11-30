---
title: DepIOSEnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DepIOSEnrollmentProfile-Objekts.
ms.openlocfilehash: 75fbf56532a4145537b714a73626dd01554179a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063816"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="1c438-103">DepIOSEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1c438-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="1c438-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c438-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c438-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c438-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c438-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c438-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c438-107">Aktualisieren Sie die Eigenschaften eines [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c438-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c438-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c438-108">Prerequisites</span></span>
<span data-ttu-id="1c438-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c438-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c438-111">Permission type</span></span>|<span data-ttu-id="1c438-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c438-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c438-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c438-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c438-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c438-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1c438-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c438-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c438-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c438-116">Not supported.</span></span>|
|<span data-ttu-id="1c438-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c438-117">Application</span></span>|<span data-ttu-id="1c438-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c438-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c438-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c438-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="1c438-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c438-120">Request headers</span></span>
|<span data-ttu-id="1c438-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c438-121">Header</span></span>|<span data-ttu-id="1c438-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1c438-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c438-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c438-123">Authorization</span></span>|<span data-ttu-id="1c438-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c438-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c438-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c438-125">Accept</span></span>|<span data-ttu-id="1c438-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c438-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c438-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c438-127">Request body</span></span>
<span data-ttu-id="1c438-128">Geben Sie im Textkörper Anforderung für das Objekt [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1c438-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="1c438-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1c438-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="1c438-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c438-130">Property</span></span>|<span data-ttu-id="1c438-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1c438-131">Type</span></span>|<span data-ttu-id="1c438-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c438-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c438-133">id</span><span class="sxs-lookup"><span data-stu-id="1c438-133">id</span></span>|<span data-ttu-id="1c438-134">String</span><span class="sxs-lookup"><span data-stu-id="1c438-134">String</span></span>|<span data-ttu-id="1c438-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1c438-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1c438-136">displayName</span></span>|<span data-ttu-id="1c438-137">String</span><span class="sxs-lookup"><span data-stu-id="1c438-137">String</span></span>|<span data-ttu-id="1c438-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1c438-139">description</span><span class="sxs-lookup"><span data-stu-id="1c438-139">description</span></span>|<span data-ttu-id="1c438-140">String</span><span class="sxs-lookup"><span data-stu-id="1c438-140">String</span></span>|<span data-ttu-id="1c438-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1c438-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="1c438-142">requiresUserAuthentication</span></span>|<span data-ttu-id="1c438-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-143">Boolean</span></span>|<span data-ttu-id="1c438-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="1c438-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1c438-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="1c438-145">configurationEndpointUrl</span></span>|<span data-ttu-id="1c438-146">String</span><span class="sxs-lookup"><span data-stu-id="1c438-146">String</span></span>|<span data-ttu-id="1c438-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="1c438-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1c438-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="1c438-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="1c438-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-149">Boolean</span></span>|<span data-ttu-id="1c438-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="1c438-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="1c438-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1c438-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="1c438-152">isDefault</span></span>|<span data-ttu-id="1c438-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1c438-153">Boolean</span></span>|<span data-ttu-id="1c438-154">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="1c438-155">supervisedModeEnabled</span></span>|<span data-ttu-id="1c438-156">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-156">Boolean</span></span>|<span data-ttu-id="1c438-157">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="1c438-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="1c438-158">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="1c438-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="1c438-159">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="1c438-160">supportDepartment</span></span>|<span data-ttu-id="1c438-161">String</span><span class="sxs-lookup"><span data-stu-id="1c438-161">String</span></span>|<span data-ttu-id="1c438-162">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-163">passCodeDisabled</span></span>|<span data-ttu-id="1c438-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-164">Boolean</span></span>|<span data-ttu-id="1c438-165">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="1c438-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="1c438-166">isMandatory</span></span>|<span data-ttu-id="1c438-167">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-167">Boolean</span></span>|<span data-ttu-id="1c438-168">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-169">locationDisabled</span></span>|<span data-ttu-id="1c438-170">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-170">Boolean</span></span>|<span data-ttu-id="1c438-171">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="1c438-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1c438-172">supportPhoneNumber</span></span>|<span data-ttu-id="1c438-173">String</span><span class="sxs-lookup"><span data-stu-id="1c438-173">String</span></span>|<span data-ttu-id="1c438-174">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1c438-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-175">profileRemovalDisabled</span></span>|<span data-ttu-id="1c438-176">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-176">Boolean</span></span>|<span data-ttu-id="1c438-177">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1c438-178">restoreBlocked</span></span>|<span data-ttu-id="1c438-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-179">Boolean</span></span>|<span data-ttu-id="1c438-180">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-181">appleIdDisabled</span></span>|<span data-ttu-id="1c438-182">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-182">Boolean</span></span>|<span data-ttu-id="1c438-183">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="1c438-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="1c438-185">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-185">Boolean</span></span>|<span data-ttu-id="1c438-186">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-187">touchIdDisabled</span></span>|<span data-ttu-id="1c438-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-188">Boolean</span></span>|<span data-ttu-id="1c438-189">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-190">applePayDisabled</span></span>|<span data-ttu-id="1c438-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-191">Boolean</span></span>|<span data-ttu-id="1c438-192">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-193">zoomDisabled</span></span>|<span data-ttu-id="1c438-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-194">Boolean</span></span>|<span data-ttu-id="1c438-195">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-196">siriDisabled</span></span>|<span data-ttu-id="1c438-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-197">Boolean</span></span>|<span data-ttu-id="1c438-198">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="1c438-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-199">diagnosticsDisabled</span></span>|<span data-ttu-id="1c438-200">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-200">Boolean</span></span>|<span data-ttu-id="1c438-201">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="1c438-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1c438-202">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="1c438-202">iTunesPairingMode</span></span>|[<span data-ttu-id="1c438-203">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="1c438-203">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="1c438-204">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="1c438-204">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="1c438-205">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="1c438-205">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="1c438-206">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="1c438-206">managementCertificates</span></span>|<span data-ttu-id="1c438-207">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1c438-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="1c438-208">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="1c438-208">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="1c438-209">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="1c438-209">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="1c438-210">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-210">Boolean</span></span>|<span data-ttu-id="1c438-211">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="1c438-211">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="1c438-212">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="1c438-212">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="1c438-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-213">Boolean</span></span>|<span data-ttu-id="1c438-214">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="1c438-214">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="1c438-215">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="1c438-215">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="1c438-216">Int32</span><span class="sxs-lookup"><span data-stu-id="1c438-216">Int32</span></span>|<span data-ttu-id="1c438-217">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="1c438-217">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="1c438-218">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="1c438-218">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="1c438-219">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="1c438-219">enableSharedIPad</span></span>|<span data-ttu-id="1c438-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-220">Boolean</span></span>|<span data-ttu-id="1c438-221">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="1c438-221">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="1c438-222">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="1c438-222">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="1c438-223">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="1c438-223">companyPortalVppTokenId</span></span>|<span data-ttu-id="1c438-224">String</span><span class="sxs-lookup"><span data-stu-id="1c438-224">String</span></span>|<span data-ttu-id="1c438-225">Wenn festgelegt ist, gibt an, welche Vpp Token zum Bereitstellen der Unternehmensportal mit Gerät-Lizenzierung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1c438-225">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="1c438-226">'EnableAuthenticationViaCompanyPortal' muss für diese Eigenschaft festgelegt werden soll festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="1c438-226">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="1c438-227">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="1c438-227">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="1c438-228">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1c438-228">Boolean</span></span>|<span data-ttu-id="1c438-229">Weist das Gerät zum Aktivieren der einzelnen app-Modus und Anwenden von app-Sperre während der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="1c438-229">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="1c438-230">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="1c438-230">Default is false.</span></span> <span data-ttu-id="1c438-231">'EnableAuthenticationViaCompanyPortal' und 'CompanyPortalVppTokenId' müssen für diese Eigenschaft festgelegt werden soll, festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="1c438-231">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|



## <a name="response"></a><span data-ttu-id="1c438-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c438-232">Response</span></span>
<span data-ttu-id="1c438-233">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1c438-233">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c438-234">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c438-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c438-235">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c438-235">Request</span></span>
<span data-ttu-id="1c438-236">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c438-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1267

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

### <a name="response"></a><span data-ttu-id="1c438-237">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c438-237">Response</span></span>
<span data-ttu-id="1c438-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c438-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





