---
title: DepMacOSEnrollmentProfile erstellen
description: Erstellen eines neuen depMacOSEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9968e03c62f2b377e8644f3f5ac84531f16f15d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571725"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="19363-103">DepMacOSEnrollmentProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="19363-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="19363-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19363-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19363-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="19363-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19363-106">Erstellen eines neuen [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19363-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19363-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="19363-107">Prerequisites</span></span>
<span data-ttu-id="19363-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19363-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19363-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19363-110">Permission type</span></span>|<span data-ttu-id="19363-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19363-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19363-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19363-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19363-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19363-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="19363-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19363-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19363-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19363-115">Not supported.</span></span>|
|<span data-ttu-id="19363-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19363-116">Application</span></span>|<span data-ttu-id="19363-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19363-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19363-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19363-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="19363-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19363-119">Request headers</span></span>
|<span data-ttu-id="19363-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="19363-120">Header</span></span>|<span data-ttu-id="19363-121">Wert</span><span class="sxs-lookup"><span data-stu-id="19363-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19363-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19363-122">Authorization</span></span>|<span data-ttu-id="19363-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="19363-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19363-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="19363-124">Accept</span></span>|<span data-ttu-id="19363-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19363-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19363-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19363-126">Request body</span></span>
<span data-ttu-id="19363-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das depMacOSEnrollmentProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="19363-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="19363-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der depMacOSEnrollmentProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="19363-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="19363-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19363-129">Property</span></span>|<span data-ttu-id="19363-130">Typ</span><span class="sxs-lookup"><span data-stu-id="19363-130">Type</span></span>|<span data-ttu-id="19363-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19363-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19363-132">id</span><span class="sxs-lookup"><span data-stu-id="19363-132">id</span></span>|<span data-ttu-id="19363-133">String</span><span class="sxs-lookup"><span data-stu-id="19363-133">String</span></span>|<span data-ttu-id="19363-134">Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.</span><span class="sxs-lookup"><span data-stu-id="19363-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-135">displayName</span><span class="sxs-lookup"><span data-stu-id="19363-135">displayName</span></span>|<span data-ttu-id="19363-136">String</span><span class="sxs-lookup"><span data-stu-id="19363-136">String</span></span>|<span data-ttu-id="19363-137">Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="19363-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-138">description</span><span class="sxs-lookup"><span data-stu-id="19363-138">description</span></span>|<span data-ttu-id="19363-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19363-139">String</span></span>|<span data-ttu-id="19363-140">Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="19363-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="19363-141">requiresUserAuthentication</span></span>|<span data-ttu-id="19363-142">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-142">Boolean</span></span>|<span data-ttu-id="19363-143">Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="19363-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="19363-144">configurationEndpointUrl</span></span>|<span data-ttu-id="19363-145">String</span><span class="sxs-lookup"><span data-stu-id="19363-145">String</span></span>|<span data-ttu-id="19363-146">Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung</span><span class="sxs-lookup"><span data-stu-id="19363-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="19363-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="19363-148">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-148">Boolean</span></span>|<span data-ttu-id="19363-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="19363-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="19363-150">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="19363-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="19363-152">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-152">Boolean</span></span>|<span data-ttu-id="19363-153">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="19363-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="19363-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="19363-154">isDefault</span></span>|<span data-ttu-id="19363-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="19363-155">Boolean</span></span>|<span data-ttu-id="19363-156">Gibt an, ob dies das Standardprofil ist, das von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="19363-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="19363-157">supervisedModeEnabled</span></span>|<span data-ttu-id="19363-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-158">Boolean</span></span>|<span data-ttu-id="19363-159">Überwachter Modus, true, um zu aktivieren, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="19363-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="19363-160">Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="19363-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="19363-161">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="19363-162">supportDepartment</span></span>|<span data-ttu-id="19363-163">String</span><span class="sxs-lookup"><span data-stu-id="19363-163">String</span></span>|<span data-ttu-id="19363-164">Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Abteilungsinformationen</span><span class="sxs-lookup"><span data-stu-id="19363-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-165">passCodeDisabled</span></span>|<span data-ttu-id="19363-166">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-166">Boolean</span></span>|<span data-ttu-id="19363-167">Gibt an, ob der Bereich "Passcode" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="19363-168">isMandatory</span></span>|<span data-ttu-id="19363-169">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-169">Boolean</span></span>|<span data-ttu-id="19363-170">Gibt an, ob das Profil obligatorisch von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="19363-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-171">locationDisabled</span></span>|<span data-ttu-id="19363-172">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-172">Boolean</span></span>|<span data-ttu-id="19363-173">Gibt an, ob der speicherortdienst-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="19363-174">supportPhoneNumber</span></span>|<span data-ttu-id="19363-175">String</span><span class="sxs-lookup"><span data-stu-id="19363-175">String</span></span>|<span data-ttu-id="19363-176">Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="19363-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-177">profileRemovalDisabled</span></span>|<span data-ttu-id="19363-178">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-178">Boolean</span></span>|<span data-ttu-id="19363-179">Gibt an, ob die Profil Entfernungs Option deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="19363-180">restoreBlocked</span></span>|<span data-ttu-id="19363-181">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-181">Boolean</span></span>|<span data-ttu-id="19363-182">Gibt an, ob der wiederHerstellungs-Setup Bereich von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="19363-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-183">appleIdDisabled</span></span>|<span data-ttu-id="19363-184">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-184">Boolean</span></span>|<span data-ttu-id="19363-185">Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="19363-187">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-187">Boolean</span></span>|<span data-ttu-id="19363-188">Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-189">touchIdDisabled</span></span>|<span data-ttu-id="19363-190">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-190">Boolean</span></span>|<span data-ttu-id="19363-191">Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-192">applePayDisabled</span></span>|<span data-ttu-id="19363-193">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-193">Boolean</span></span>|<span data-ttu-id="19363-194">Gibt an, ob der Apple Pay Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-195">zoomDisabled</span></span>|<span data-ttu-id="19363-196">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-196">Boolean</span></span>|<span data-ttu-id="19363-197">Gibt an, ob der Zoom-Installationsbereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-198">siriDisabled</span></span>|<span data-ttu-id="19363-199">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-199">Boolean</span></span>|<span data-ttu-id="19363-200">Gibt an, ob Siri-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-201">diagnosticsDisabled</span></span>|<span data-ttu-id="19363-202">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-202">Boolean</span></span>|<span data-ttu-id="19363-203">Gibt an, ob der Diagnose-Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="19363-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-205">Boolean</span></span>|<span data-ttu-id="19363-206">Gibt an, ob displaytone-Setupbildschirm deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-207">privacyPaneDisabled</span></span>|<span data-ttu-id="19363-208">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-208">Boolean</span></span>|<span data-ttu-id="19363-209">Gibt an, ob der Datenschutz Bildschirm deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="19363-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="19363-210">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-210">registrationDisabled</span></span>|<span data-ttu-id="19363-211">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-211">Boolean</span></span>|<span data-ttu-id="19363-212">Gibt an, ob die Registrierung deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="19363-212">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="19363-213">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-213">fileVaultDisabled</span></span>|<span data-ttu-id="19363-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-214">Boolean</span></span>|<span data-ttu-id="19363-215">Gibt an, ob das Dateidepot deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="19363-215">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="19363-216">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-216">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="19363-217">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-217">Boolean</span></span>|<span data-ttu-id="19363-218">Gibt an, ob der iCloud-Analysebildschirm deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="19363-218">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="19363-219">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-219">iCloudStorageDisabled</span></span>|<span data-ttu-id="19363-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-220">Boolean</span></span>|<span data-ttu-id="19363-221">Gibt an, ob iCloud-Dokumente und Desktop-Bildschirm deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="19363-221">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="19363-222">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="19363-222">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="19363-223">Boolesch</span><span class="sxs-lookup"><span data-stu-id="19363-223">Boolean</span></span>|<span data-ttu-id="19363-224">Gibt an, ob iCloud-Dokumente und Desktop-Bildschirm deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="19363-224">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="19363-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="19363-225">Response</span></span>
<span data-ttu-id="19363-226">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="19363-226">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19363-227">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19363-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="19363-228">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19363-228">Request</span></span>
<span data-ttu-id="19363-229">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19363-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1136

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
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="19363-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="19363-230">Response</span></span>
<span data-ttu-id="19363-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19363-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1185

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
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




