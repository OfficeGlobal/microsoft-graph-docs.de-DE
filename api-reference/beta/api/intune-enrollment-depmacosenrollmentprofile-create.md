---
title: Erstellen von depMacOSEnrollmentProfile
description: Erstellen eines neuen DepMacOSEnrollmentProfile-Objekts.
ms.openlocfilehash: de789e3b09ba2445240b2cd5adf29fdfde3005d7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065895"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="5e9c8-103">Erstellen von depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5e9c8-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="5e9c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e9c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e9c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e9c8-107">Erstellen eines neuen [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e9c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5e9c8-108">Prerequisites</span></span>
<span data-ttu-id="5e9c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e9c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e9c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e9c8-111">Permission type</span></span>|<span data-ttu-id="5e9c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e9c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e9c8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e9c8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5e9c8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e9c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-116">Not supported.</span></span>|
|<span data-ttu-id="5e9c8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e9c8-117">Application</span></span>|<span data-ttu-id="5e9c8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e9c8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e9c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5e9c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e9c8-120">Request headers</span></span>
|<span data-ttu-id="5e9c8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5e9c8-121">Header</span></span>|<span data-ttu-id="5e9c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e9c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e9c8-123">Authorization</span></span>|<span data-ttu-id="5e9c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5e9c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e9c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e9c8-125">Accept</span></span>|<span data-ttu-id="5e9c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e9c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e9c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e9c8-127">Request body</span></span>
<span data-ttu-id="5e9c8-128">Geben Sie im Textkörper Anforderung für das Objekt DepMacOSEnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="5e9c8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepMacOSEnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="5e9c8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e9c8-130">Property</span></span>|<span data-ttu-id="5e9c8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5e9c8-131">Type</span></span>|<span data-ttu-id="5e9c8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e9c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e9c8-133">id</span><span class="sxs-lookup"><span data-stu-id="5e9c8-133">id</span></span>|<span data-ttu-id="5e9c8-134">String</span><span class="sxs-lookup"><span data-stu-id="5e9c8-134">String</span></span>|<span data-ttu-id="5e9c8-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5e9c8-136">displayName</span></span>|<span data-ttu-id="5e9c8-137">String</span><span class="sxs-lookup"><span data-stu-id="5e9c8-137">String</span></span>|<span data-ttu-id="5e9c8-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-139">description</span><span class="sxs-lookup"><span data-stu-id="5e9c8-139">description</span></span>|<span data-ttu-id="5e9c8-140">String</span><span class="sxs-lookup"><span data-stu-id="5e9c8-140">String</span></span>|<span data-ttu-id="5e9c8-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="5e9c8-142">requiresUserAuthentication</span></span>|<span data-ttu-id="5e9c8-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-143">Boolean</span></span>|<span data-ttu-id="5e9c8-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="5e9c8-145">configurationEndpointUrl</span></span>|<span data-ttu-id="5e9c8-146">String</span><span class="sxs-lookup"><span data-stu-id="5e9c8-146">String</span></span>|<span data-ttu-id="5e9c8-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="5e9c8-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="5e9c8-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="5e9c8-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-149">Boolean</span></span>|<span data-ttu-id="5e9c8-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="5e9c8-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="5e9c8-152">isDefault</span></span>|<span data-ttu-id="5e9c8-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-153">Boolean</span></span>|<span data-ttu-id="5e9c8-154">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-155">supervisedModeEnabled</span></span>|<span data-ttu-id="5e9c8-156">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-156">Boolean</span></span>|<span data-ttu-id="5e9c8-157">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="5e9c8-158">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="5e9c8-159">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="5e9c8-160">supportDepartment</span></span>|<span data-ttu-id="5e9c8-161">String</span><span class="sxs-lookup"><span data-stu-id="5e9c8-161">String</span></span>|<span data-ttu-id="5e9c8-162">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-163">passCodeDisabled</span></span>|<span data-ttu-id="5e9c8-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-164">Boolean</span></span>|<span data-ttu-id="5e9c8-165">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="5e9c8-166">isMandatory</span></span>|<span data-ttu-id="5e9c8-167">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-167">Boolean</span></span>|<span data-ttu-id="5e9c8-168">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-169">locationDisabled</span></span>|<span data-ttu-id="5e9c8-170">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-170">Boolean</span></span>|<span data-ttu-id="5e9c8-171">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5e9c8-172">supportPhoneNumber</span></span>|<span data-ttu-id="5e9c8-173">String</span><span class="sxs-lookup"><span data-stu-id="5e9c8-173">String</span></span>|<span data-ttu-id="5e9c8-174">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5e9c8-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-175">profileRemovalDisabled</span></span>|<span data-ttu-id="5e9c8-176">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-176">Boolean</span></span>|<span data-ttu-id="5e9c8-177">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="5e9c8-178">restoreBlocked</span></span>|<span data-ttu-id="5e9c8-179">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-179">Boolean</span></span>|<span data-ttu-id="5e9c8-180">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-181">appleIdDisabled</span></span>|<span data-ttu-id="5e9c8-182">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-182">Boolean</span></span>|<span data-ttu-id="5e9c8-183">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="5e9c8-185">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-185">Boolean</span></span>|<span data-ttu-id="5e9c8-186">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-187">touchIdDisabled</span></span>|<span data-ttu-id="5e9c8-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-188">Boolean</span></span>|<span data-ttu-id="5e9c8-189">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-190">applePayDisabled</span></span>|<span data-ttu-id="5e9c8-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-191">Boolean</span></span>|<span data-ttu-id="5e9c8-192">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-193">zoomDisabled</span></span>|<span data-ttu-id="5e9c8-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-194">Boolean</span></span>|<span data-ttu-id="5e9c8-195">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-196">siriDisabled</span></span>|<span data-ttu-id="5e9c8-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-197">Boolean</span></span>|<span data-ttu-id="5e9c8-198">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="5e9c8-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-199">diagnosticsDisabled</span></span>|<span data-ttu-id="5e9c8-200">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-200">Boolean</span></span>|<span data-ttu-id="5e9c8-201">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="5e9c8-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5e9c8-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-202">registrationDisabled</span></span>|<span data-ttu-id="5e9c8-203">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-203">Boolean</span></span>|<span data-ttu-id="5e9c8-204">Gibt an, ob die Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="5e9c8-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="5e9c8-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-205">fileVaultDisabled</span></span>|<span data-ttu-id="5e9c8-206">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-206">Boolean</span></span>|<span data-ttu-id="5e9c8-207">Gibt an, ob die Datei Vault deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="5e9c8-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="5e9c8-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="5e9c8-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="5e9c8-209">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5e9c8-209">Boolean</span></span>|<span data-ttu-id="5e9c8-210">Gibt an, ob iCloud Analytics Bildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="5e9c8-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="5e9c8-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e9c8-211">Response</span></span>
<span data-ttu-id="5e9c8-212">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-212">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e9c8-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e9c8-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e9c8-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e9c8-214">Request</span></span>
<span data-ttu-id="5e9c8-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 928

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="5e9c8-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e9c8-216">Response</span></span>
<span data-ttu-id="5e9c8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e9c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```





