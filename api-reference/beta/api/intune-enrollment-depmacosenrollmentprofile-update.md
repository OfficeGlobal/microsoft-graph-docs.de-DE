---
title: DepMacOSEnrollmentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines depMacOSEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2efa7c1791bb8a7c9ed86e13439903e8458f038a
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572341"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="52e6a-103">DepMacOSEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="52e6a-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="52e6a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52e6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52e6a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="52e6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e6a-106">Aktualisieren der Eigenschaften eines [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="52e6a-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52e6a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="52e6a-107">Prerequisites</span></span>
<span data-ttu-id="52e6a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="52e6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="52e6a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52e6a-110">Permission type</span></span>|<span data-ttu-id="52e6a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52e6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52e6a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52e6a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52e6a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e6a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="52e6a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52e6a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52e6a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52e6a-115">Not supported.</span></span>|
|<span data-ttu-id="52e6a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52e6a-116">Application</span></span>|<span data-ttu-id="52e6a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52e6a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52e6a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52e6a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="52e6a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52e6a-119">Request headers</span></span>
|<span data-ttu-id="52e6a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="52e6a-120">Header</span></span>|<span data-ttu-id="52e6a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="52e6a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52e6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e6a-122">Authorization</span></span>|<span data-ttu-id="52e6a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="52e6a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52e6a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="52e6a-124">Accept</span></span>|<span data-ttu-id="52e6a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52e6a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52e6a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52e6a-126">Request body</span></span>
<span data-ttu-id="52e6a-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="52e6a-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="52e6a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="52e6a-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="52e6a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52e6a-129">Property</span></span>|<span data-ttu-id="52e6a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="52e6a-130">Type</span></span>|<span data-ttu-id="52e6a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52e6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e6a-132">id</span><span class="sxs-lookup"><span data-stu-id="52e6a-132">id</span></span>|<span data-ttu-id="52e6a-133">String</span><span class="sxs-lookup"><span data-stu-id="52e6a-133">String</span></span>|<span data-ttu-id="52e6a-134">Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.</span><span class="sxs-lookup"><span data-stu-id="52e6a-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="52e6a-135">displayName</span></span>|<span data-ttu-id="52e6a-136">String</span><span class="sxs-lookup"><span data-stu-id="52e6a-136">String</span></span>|<span data-ttu-id="52e6a-137">Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="52e6a-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-138">description</span><span class="sxs-lookup"><span data-stu-id="52e6a-138">description</span></span>|<span data-ttu-id="52e6a-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52e6a-139">String</span></span>|<span data-ttu-id="52e6a-140">Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="52e6a-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="52e6a-141">requiresUserAuthentication</span></span>|<span data-ttu-id="52e6a-142">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-142">Boolean</span></span>|<span data-ttu-id="52e6a-143">Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="52e6a-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="52e6a-144">configurationEndpointUrl</span></span>|<span data-ttu-id="52e6a-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52e6a-145">String</span></span>|<span data-ttu-id="52e6a-146">Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung</span><span class="sxs-lookup"><span data-stu-id="52e6a-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="52e6a-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="52e6a-148">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-148">Boolean</span></span>|<span data-ttu-id="52e6a-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="52e6a-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="52e6a-150">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="52e6a-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="52e6a-152">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-152">Boolean</span></span>|<span data-ttu-id="52e6a-153">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="52e6a-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e6a-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="52e6a-154">isDefault</span></span>|<span data-ttu-id="52e6a-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e6a-155">Boolean</span></span>|<span data-ttu-id="52e6a-156">Gibt an, ob dies das Standardprofil ist, das von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="52e6a-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-157">supervisedModeEnabled</span></span>|<span data-ttu-id="52e6a-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-158">Boolean</span></span>|<span data-ttu-id="52e6a-159">Überwachter Modus, true, um zu aktivieren, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="52e6a-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="52e6a-160">Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="52e6a-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="52e6a-161">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="52e6a-162">supportDepartment</span></span>|<span data-ttu-id="52e6a-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52e6a-163">String</span></span>|<span data-ttu-id="52e6a-164">Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Abteilungsinformationen</span><span class="sxs-lookup"><span data-stu-id="52e6a-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-165">passCodeDisabled</span></span>|<span data-ttu-id="52e6a-166">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-166">Boolean</span></span>|<span data-ttu-id="52e6a-167">Gibt an, ob der Bereich "Passcode" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="52e6a-168">isMandatory</span></span>|<span data-ttu-id="52e6a-169">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-169">Boolean</span></span>|<span data-ttu-id="52e6a-170">Gibt an, ob das Profil obligatorisch von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="52e6a-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-171">locationDisabled</span></span>|<span data-ttu-id="52e6a-172">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-172">Boolean</span></span>|<span data-ttu-id="52e6a-173">Gibt an, ob der speicherortdienst-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="52e6a-174">supportPhoneNumber</span></span>|<span data-ttu-id="52e6a-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52e6a-175">String</span></span>|<span data-ttu-id="52e6a-176">Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="52e6a-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-177">profileRemovalDisabled</span></span>|<span data-ttu-id="52e6a-178">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-178">Boolean</span></span>|<span data-ttu-id="52e6a-179">Gibt an, ob die Profil Entfernungs Option deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="52e6a-180">restoreBlocked</span></span>|<span data-ttu-id="52e6a-181">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-181">Boolean</span></span>|<span data-ttu-id="52e6a-182">Gibt an, ob der wiederHerstellungs-Setup Bereich von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="52e6a-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-183">appleIdDisabled</span></span>|<span data-ttu-id="52e6a-184">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-184">Boolean</span></span>|<span data-ttu-id="52e6a-185">Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="52e6a-187">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-187">Boolean</span></span>|<span data-ttu-id="52e6a-188">Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-189">touchIdDisabled</span></span>|<span data-ttu-id="52e6a-190">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-190">Boolean</span></span>|<span data-ttu-id="52e6a-191">Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-192">applePayDisabled</span></span>|<span data-ttu-id="52e6a-193">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-193">Boolean</span></span>|<span data-ttu-id="52e6a-194">Gibt an, ob der Apple Pay Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-195">zoomDisabled</span></span>|<span data-ttu-id="52e6a-196">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-196">Boolean</span></span>|<span data-ttu-id="52e6a-197">Gibt an, ob der Zoom-Installationsbereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-198">siriDisabled</span></span>|<span data-ttu-id="52e6a-199">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-199">Boolean</span></span>|<span data-ttu-id="52e6a-200">Gibt an, ob Siri-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-201">diagnosticsDisabled</span></span>|<span data-ttu-id="52e6a-202">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-202">Boolean</span></span>|<span data-ttu-id="52e6a-203">Gibt an, ob der Diagnose-Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="52e6a-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-205">Boolean</span></span>|<span data-ttu-id="52e6a-206">Gibt an, ob displaytone-Setupbildschirm deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-207">privacyPaneDisabled</span></span>|<span data-ttu-id="52e6a-208">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-208">Boolean</span></span>|<span data-ttu-id="52e6a-209">Gibt an, ob der Datenschutz Bildschirm deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e6a-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e6a-210">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-210">registrationDisabled</span></span>|<span data-ttu-id="52e6a-211">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-211">Boolean</span></span>|<span data-ttu-id="52e6a-212">Gibt an, ob die Registrierung deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="52e6a-212">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="52e6a-213">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-213">fileVaultDisabled</span></span>|<span data-ttu-id="52e6a-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-214">Boolean</span></span>|<span data-ttu-id="52e6a-215">Gibt an, ob das Dateidepot deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="52e6a-215">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="52e6a-216">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-216">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="52e6a-217">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-217">Boolean</span></span>|<span data-ttu-id="52e6a-218">Gibt an, ob der iCloud-Analysebildschirm deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="52e6a-218">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="52e6a-219">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-219">iCloudStorageDisabled</span></span>|<span data-ttu-id="52e6a-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-220">Boolean</span></span>|<span data-ttu-id="52e6a-221">Gibt an, ob iCloud-Dokumente und Desktop-Bildschirm deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="52e6a-221">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="52e6a-222">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e6a-222">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="52e6a-223">Boolesch</span><span class="sxs-lookup"><span data-stu-id="52e6a-223">Boolean</span></span>|<span data-ttu-id="52e6a-224">Gibt an, ob iCloud-Dokumente und Desktop-Bildschirm deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="52e6a-224">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="52e6a-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="52e6a-225">Response</span></span>
<span data-ttu-id="52e6a-226">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="52e6a-226">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e6a-227">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52e6a-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="52e6a-228">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52e6a-228">Request</span></span>
<span data-ttu-id="52e6a-229">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52e6a-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="52e6a-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="52e6a-230">Response</span></span>
<span data-ttu-id="52e6a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52e6a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




