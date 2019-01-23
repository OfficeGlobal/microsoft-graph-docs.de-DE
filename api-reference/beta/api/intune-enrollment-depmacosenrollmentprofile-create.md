---
title: Erstellen von depMacOSEnrollmentProfile
description: Erstellen eines neuen DepMacOSEnrollmentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7fd29ee598507b982ecd48ea58b6a09ccf90972
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420591"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="b96cb-103">Erstellen von depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b96cb-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="b96cb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b96cb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b96cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b96cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b96cb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b96cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b96cb-107">Erstellen eines neuen [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b96cb-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b96cb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b96cb-108">Prerequisites</span></span>
<span data-ttu-id="b96cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b96cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b96cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b96cb-111">Permission type</span></span>|<span data-ttu-id="b96cb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b96cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b96cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b96cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b96cb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b96cb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b96cb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b96cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b96cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b96cb-116">Not supported.</span></span>|
|<span data-ttu-id="b96cb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b96cb-117">Application</span></span>|<span data-ttu-id="b96cb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b96cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b96cb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b96cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="b96cb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b96cb-120">Request headers</span></span>
|<span data-ttu-id="b96cb-121">Header</span><span class="sxs-lookup"><span data-stu-id="b96cb-121">Header</span></span>|<span data-ttu-id="b96cb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b96cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b96cb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b96cb-123">Authorization</span></span>|<span data-ttu-id="b96cb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b96cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b96cb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b96cb-125">Accept</span></span>|<span data-ttu-id="b96cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b96cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b96cb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b96cb-127">Request body</span></span>
<span data-ttu-id="b96cb-128">Geben Sie im Textkörper Anforderung für das Objekt DepMacOSEnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b96cb-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="b96cb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepMacOSEnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="b96cb-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="b96cb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b96cb-130">Property</span></span>|<span data-ttu-id="b96cb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b96cb-131">Type</span></span>|<span data-ttu-id="b96cb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b96cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b96cb-133">id</span><span class="sxs-lookup"><span data-stu-id="b96cb-133">id</span></span>|<span data-ttu-id="b96cb-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b96cb-134">String</span></span>|<span data-ttu-id="b96cb-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b96cb-136">displayName</span></span>|<span data-ttu-id="b96cb-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b96cb-137">String</span></span>|<span data-ttu-id="b96cb-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-139">description</span><span class="sxs-lookup"><span data-stu-id="b96cb-139">description</span></span>|<span data-ttu-id="b96cb-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b96cb-140">String</span></span>|<span data-ttu-id="b96cb-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b96cb-142">requiresUserAuthentication</span></span>|<span data-ttu-id="b96cb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-143">Boolean</span></span>|<span data-ttu-id="b96cb-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="b96cb-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="b96cb-145">configurationEndpointUrl</span></span>|<span data-ttu-id="b96cb-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b96cb-146">String</span></span>|<span data-ttu-id="b96cb-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="b96cb-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b96cb-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b96cb-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-149">Boolean</span></span>|<span data-ttu-id="b96cb-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="b96cb-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="b96cb-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="b96cb-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="b96cb-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-153">Boolean</span></span>|<span data-ttu-id="b96cb-154">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="b96cb-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b96cb-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="b96cb-155">isDefault</span></span>|<span data-ttu-id="b96cb-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-156">Boolean</span></span>|<span data-ttu-id="b96cb-157">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-158">supervisedModeEnabled</span></span>|<span data-ttu-id="b96cb-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-159">Boolean</span></span>|<span data-ttu-id="b96cb-160">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="b96cb-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="b96cb-161">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="b96cb-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="b96cb-162">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="b96cb-163">supportDepartment</span></span>|<span data-ttu-id="b96cb-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b96cb-164">String</span></span>|<span data-ttu-id="b96cb-165">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-166">passCodeDisabled</span></span>|<span data-ttu-id="b96cb-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-167">Boolean</span></span>|<span data-ttu-id="b96cb-168">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="b96cb-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="b96cb-169">isMandatory</span></span>|<span data-ttu-id="b96cb-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-170">Boolean</span></span>|<span data-ttu-id="b96cb-171">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-172">locationDisabled</span></span>|<span data-ttu-id="b96cb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-173">Boolean</span></span>|<span data-ttu-id="b96cb-174">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="b96cb-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b96cb-175">supportPhoneNumber</span></span>|<span data-ttu-id="b96cb-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b96cb-176">String</span></span>|<span data-ttu-id="b96cb-177">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b96cb-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-178">profileRemovalDisabled</span></span>|<span data-ttu-id="b96cb-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-179">Boolean</span></span>|<span data-ttu-id="b96cb-180">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b96cb-181">restoreBlocked</span></span>|<span data-ttu-id="b96cb-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-182">Boolean</span></span>|<span data-ttu-id="b96cb-183">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-184">appleIdDisabled</span></span>|<span data-ttu-id="b96cb-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-185">Boolean</span></span>|<span data-ttu-id="b96cb-186">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="b96cb-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="b96cb-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-188">Boolean</span></span>|<span data-ttu-id="b96cb-189">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-190">touchIdDisabled</span></span>|<span data-ttu-id="b96cb-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-191">Boolean</span></span>|<span data-ttu-id="b96cb-192">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-193">applePayDisabled</span></span>|<span data-ttu-id="b96cb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-194">Boolean</span></span>|<span data-ttu-id="b96cb-195">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-196">zoomDisabled</span></span>|<span data-ttu-id="b96cb-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-197">Boolean</span></span>|<span data-ttu-id="b96cb-198">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-199">siriDisabled</span></span>|<span data-ttu-id="b96cb-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-200">Boolean</span></span>|<span data-ttu-id="b96cb-201">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-202">diagnosticsDisabled</span></span>|<span data-ttu-id="b96cb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-203">Boolean</span></span>|<span data-ttu-id="b96cb-204">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="b96cb-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="b96cb-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-206">Boolean</span></span>|<span data-ttu-id="b96cb-207">Gibt an, ob Displaytone Setupbildschirm deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-208">privacyPaneDisabled</span></span>|<span data-ttu-id="b96cb-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-209">Boolean</span></span>|<span data-ttu-id="b96cb-210">Gibt an, ob Privacy Bildschirm deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="b96cb-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b96cb-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-211">registrationDisabled</span></span>|<span data-ttu-id="b96cb-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-212">Boolean</span></span>|<span data-ttu-id="b96cb-213">Gibt an, ob die Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="b96cb-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="b96cb-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-214">fileVaultDisabled</span></span>|<span data-ttu-id="b96cb-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-215">Boolean</span></span>|<span data-ttu-id="b96cb-216">Gibt an, ob die Datei Vault deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="b96cb-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="b96cb-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b96cb-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="b96cb-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96cb-218">Boolean</span></span>|<span data-ttu-id="b96cb-219">Gibt an, ob iCloud Analytics Bildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="b96cb-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="b96cb-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="b96cb-220">Response</span></span>
<span data-ttu-id="b96cb-221">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b96cb-221">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b96cb-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b96cb-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="b96cb-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b96cb-223">Request</span></span>
<span data-ttu-id="b96cb-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b96cb-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1061

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="b96cb-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="b96cb-225">Response</span></span>
<span data-ttu-id="b96cb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b96cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```




