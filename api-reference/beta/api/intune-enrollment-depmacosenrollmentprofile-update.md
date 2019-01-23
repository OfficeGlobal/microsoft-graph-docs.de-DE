---
title: DepMacOSEnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DepMacOSEnrollmentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f86e520160e988e72aaa2473b256613a997cae0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420115"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="15857-103">DepMacOSEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15857-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="15857-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="15857-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15857-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15857-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15857-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15857-107">Aktualisieren Sie die Eigenschaften eines [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="15857-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15857-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15857-108">Prerequisites</span></span>
<span data-ttu-id="15857-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15857-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15857-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15857-111">Permission type</span></span>|<span data-ttu-id="15857-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15857-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15857-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15857-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15857-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15857-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15857-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15857-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15857-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15857-116">Not supported.</span></span>|
|<span data-ttu-id="15857-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15857-117">Application</span></span>|<span data-ttu-id="15857-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15857-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15857-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15857-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="15857-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15857-120">Request headers</span></span>
|<span data-ttu-id="15857-121">Header</span><span class="sxs-lookup"><span data-stu-id="15857-121">Header</span></span>|<span data-ttu-id="15857-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15857-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15857-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="15857-123">Authorization</span></span>|<span data-ttu-id="15857-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15857-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15857-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15857-125">Accept</span></span>|<span data-ttu-id="15857-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15857-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15857-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15857-127">Request body</span></span>
<span data-ttu-id="15857-128">Geben Sie im Textkörper Anforderung für das Objekt [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="15857-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="15857-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="15857-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="15857-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15857-130">Property</span></span>|<span data-ttu-id="15857-131">Typ</span><span class="sxs-lookup"><span data-stu-id="15857-131">Type</span></span>|<span data-ttu-id="15857-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15857-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15857-133">id</span><span class="sxs-lookup"><span data-stu-id="15857-133">id</span></span>|<span data-ttu-id="15857-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15857-134">String</span></span>|<span data-ttu-id="15857-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15857-136">displayName</span></span>|<span data-ttu-id="15857-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15857-137">String</span></span>|<span data-ttu-id="15857-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-139">description</span><span class="sxs-lookup"><span data-stu-id="15857-139">description</span></span>|<span data-ttu-id="15857-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15857-140">String</span></span>|<span data-ttu-id="15857-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="15857-142">requiresUserAuthentication</span></span>|<span data-ttu-id="15857-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-143">Boolean</span></span>|<span data-ttu-id="15857-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="15857-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="15857-145">configurationEndpointUrl</span></span>|<span data-ttu-id="15857-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15857-146">String</span></span>|<span data-ttu-id="15857-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="15857-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="15857-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="15857-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-149">Boolean</span></span>|<span data-ttu-id="15857-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="15857-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="15857-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="15857-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="15857-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-153">Boolean</span></span>|<span data-ttu-id="15857-154">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="15857-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15857-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="15857-155">isDefault</span></span>|<span data-ttu-id="15857-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-156">Boolean</span></span>|<span data-ttu-id="15857-157">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="15857-158">supervisedModeEnabled</span></span>|<span data-ttu-id="15857-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-159">Boolean</span></span>|<span data-ttu-id="15857-160">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="15857-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="15857-161">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="15857-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="15857-162">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="15857-163">supportDepartment</span></span>|<span data-ttu-id="15857-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15857-164">String</span></span>|<span data-ttu-id="15857-165">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-166">passCodeDisabled</span></span>|<span data-ttu-id="15857-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-167">Boolean</span></span>|<span data-ttu-id="15857-168">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="15857-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="15857-169">isMandatory</span></span>|<span data-ttu-id="15857-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-170">Boolean</span></span>|<span data-ttu-id="15857-171">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-172">locationDisabled</span></span>|<span data-ttu-id="15857-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-173">Boolean</span></span>|<span data-ttu-id="15857-174">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="15857-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="15857-175">supportPhoneNumber</span></span>|<span data-ttu-id="15857-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15857-176">String</span></span>|<span data-ttu-id="15857-177">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15857-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-178">profileRemovalDisabled</span></span>|<span data-ttu-id="15857-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-179">Boolean</span></span>|<span data-ttu-id="15857-180">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="15857-181">restoreBlocked</span></span>|<span data-ttu-id="15857-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-182">Boolean</span></span>|<span data-ttu-id="15857-183">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-184">appleIdDisabled</span></span>|<span data-ttu-id="15857-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-185">Boolean</span></span>|<span data-ttu-id="15857-186">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="15857-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="15857-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-188">Boolean</span></span>|<span data-ttu-id="15857-189">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-190">touchIdDisabled</span></span>|<span data-ttu-id="15857-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-191">Boolean</span></span>|<span data-ttu-id="15857-192">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-193">applePayDisabled</span></span>|<span data-ttu-id="15857-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-194">Boolean</span></span>|<span data-ttu-id="15857-195">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-196">zoomDisabled</span></span>|<span data-ttu-id="15857-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-197">Boolean</span></span>|<span data-ttu-id="15857-198">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-199">siriDisabled</span></span>|<span data-ttu-id="15857-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-200">Boolean</span></span>|<span data-ttu-id="15857-201">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-202">diagnosticsDisabled</span></span>|<span data-ttu-id="15857-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-203">Boolean</span></span>|<span data-ttu-id="15857-204">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="15857-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="15857-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-206">Boolean</span></span>|<span data-ttu-id="15857-207">Gibt an, ob Displaytone Setupbildschirm deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-208">privacyPaneDisabled</span></span>|<span data-ttu-id="15857-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-209">Boolean</span></span>|<span data-ttu-id="15857-210">Gibt an, ob Privacy Bildschirm deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="15857-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="15857-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-211">registrationDisabled</span></span>|<span data-ttu-id="15857-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-212">Boolean</span></span>|<span data-ttu-id="15857-213">Gibt an, ob die Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="15857-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="15857-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-214">fileVaultDisabled</span></span>|<span data-ttu-id="15857-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-215">Boolean</span></span>|<span data-ttu-id="15857-216">Gibt an, ob die Datei Vault deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="15857-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="15857-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="15857-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="15857-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="15857-218">Boolean</span></span>|<span data-ttu-id="15857-219">Gibt an, ob iCloud Analytics Bildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="15857-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="15857-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="15857-220">Response</span></span>
<span data-ttu-id="15857-221">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="15857-221">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15857-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15857-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="15857-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15857-223">Request</span></span>
<span data-ttu-id="15857-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15857-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="15857-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="15857-225">Response</span></span>
<span data-ttu-id="15857-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15857-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




