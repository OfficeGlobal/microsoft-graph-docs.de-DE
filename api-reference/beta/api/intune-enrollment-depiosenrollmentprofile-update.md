---
title: DepIOSEnrollmentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines depIOSEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea708a5ffe661f8024c027d1ac9ef10877474cd6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986943"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="ba5c3-103">DepIOSEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ba5c3-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="ba5c3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba5c3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba5c3-106">Aktualisieren der Eigenschaften eines [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba5c3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ba5c3-107">Prerequisites</span></span>
<span data-ttu-id="ba5c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba5c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5c3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba5c3-110">Permission type</span></span>|<span data-ttu-id="ba5c3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba5c3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba5c3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5c3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba5c3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba5c3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba5c3-115">Not supported.</span></span>|
|<span data-ttu-id="ba5c3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba5c3-116">Application</span></span>|<span data-ttu-id="ba5c3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba5c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba5c3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba5c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ba5c3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba5c3-119">Request headers</span></span>
|<span data-ttu-id="ba5c3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ba5c3-120">Header</span></span>|<span data-ttu-id="ba5c3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba5c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba5c3-122">Authorization</span></span>|<span data-ttu-id="ba5c3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ba5c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba5c3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ba5c3-124">Accept</span></span>|<span data-ttu-id="ba5c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba5c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba5c3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba5c3-126">Request body</span></span>
<span data-ttu-id="ba5c3-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="ba5c3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="ba5c3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba5c3-129">Property</span></span>|<span data-ttu-id="ba5c3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ba5c3-130">Type</span></span>|<span data-ttu-id="ba5c3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba5c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba5c3-132">id</span><span class="sxs-lookup"><span data-stu-id="ba5c3-132">id</span></span>|<span data-ttu-id="ba5c3-133">String</span><span class="sxs-lookup"><span data-stu-id="ba5c3-133">String</span></span>|<span data-ttu-id="ba5c3-134">Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ba5c3-135">displayName</span></span>|<span data-ttu-id="ba5c3-136">String</span><span class="sxs-lookup"><span data-stu-id="ba5c3-136">String</span></span>|<span data-ttu-id="ba5c3-137">Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="ba5c3-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-138">description</span><span class="sxs-lookup"><span data-stu-id="ba5c3-138">description</span></span>|<span data-ttu-id="ba5c3-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba5c3-139">String</span></span>|<span data-ttu-id="ba5c3-140">Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils</span><span class="sxs-lookup"><span data-stu-id="ba5c3-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ba5c3-141">requiresUserAuthentication</span></span>|<span data-ttu-id="ba5c3-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-142">Boolean</span></span>|<span data-ttu-id="ba5c3-143">Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ba5c3-144">configurationEndpointUrl</span></span>|<span data-ttu-id="ba5c3-145">String</span><span class="sxs-lookup"><span data-stu-id="ba5c3-145">String</span></span>|<span data-ttu-id="ba5c3-146">Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung</span><span class="sxs-lookup"><span data-stu-id="ba5c3-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ba5c3-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ba5c3-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-148">Boolean</span></span>|<span data-ttu-id="ba5c3-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ba5c3-150">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ba5c3-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ba5c3-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-152">Boolean</span></span>|<span data-ttu-id="ba5c3-153">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="ba5c3-154">isDefault</span></span>|<span data-ttu-id="ba5c3-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba5c3-155">Boolean</span></span>|<span data-ttu-id="ba5c3-156">Gibt an, ob dies das Standardprofil ist, das von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-157">supervisedModeEnabled</span></span>|<span data-ttu-id="ba5c3-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-158">Boolean</span></span>|<span data-ttu-id="ba5c3-159">Überwachter Modus, true, um zu aktivieren, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ba5c3-160">Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="ba5c3-161">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ba5c3-162">supportDepartment</span></span>|<span data-ttu-id="ba5c3-163">String</span><span class="sxs-lookup"><span data-stu-id="ba5c3-163">String</span></span>|<span data-ttu-id="ba5c3-164">Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Abteilungsinformationen</span><span class="sxs-lookup"><span data-stu-id="ba5c3-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-165">passCodeDisabled</span></span>|<span data-ttu-id="ba5c3-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-166">Boolean</span></span>|<span data-ttu-id="ba5c3-167">Gibt an, ob der Bereich "Passcode" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ba5c3-168">isMandatory</span></span>|<span data-ttu-id="ba5c3-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-169">Boolean</span></span>|<span data-ttu-id="ba5c3-170">Gibt an, ob das Profil obligatorisch von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-171">locationDisabled</span></span>|<span data-ttu-id="ba5c3-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-172">Boolean</span></span>|<span data-ttu-id="ba5c3-173">Gibt an, ob der speicherortdienst-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ba5c3-174">supportPhoneNumber</span></span>|<span data-ttu-id="ba5c3-175">String</span><span class="sxs-lookup"><span data-stu-id="ba5c3-175">String</span></span>|<span data-ttu-id="ba5c3-176">Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="ba5c3-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-177">profileRemovalDisabled</span></span>|<span data-ttu-id="ba5c3-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-178">Boolean</span></span>|<span data-ttu-id="ba5c3-179">Gibt an, ob die Profil Entfernungs Option deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ba5c3-180">restoreBlocked</span></span>|<span data-ttu-id="ba5c3-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-181">Boolean</span></span>|<span data-ttu-id="ba5c3-182">Gibt an, ob der wiederHerstellungs-Setup Bereich von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-183">appleIdDisabled</span></span>|<span data-ttu-id="ba5c3-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-184">Boolean</span></span>|<span data-ttu-id="ba5c3-185">Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ba5c3-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-187">Boolean</span></span>|<span data-ttu-id="ba5c3-188">Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-189">touchIdDisabled</span></span>|<span data-ttu-id="ba5c3-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-190">Boolean</span></span>|<span data-ttu-id="ba5c3-191">Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-192">applePayDisabled</span></span>|<span data-ttu-id="ba5c3-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-193">Boolean</span></span>|<span data-ttu-id="ba5c3-194">Gibt an, ob der Apple Pay Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-195">zoomDisabled</span></span>|<span data-ttu-id="ba5c3-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-196">Boolean</span></span>|<span data-ttu-id="ba5c3-197">Gibt an, ob der Zoom-Installationsbereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-198">siriDisabled</span></span>|<span data-ttu-id="ba5c3-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-199">Boolean</span></span>|<span data-ttu-id="ba5c3-200">Gibt an, ob Siri-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-201">diagnosticsDisabled</span></span>|<span data-ttu-id="ba5c3-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-202">Boolean</span></span>|<span data-ttu-id="ba5c3-203">Gibt an, ob der Diagnose-Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="ba5c3-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-205">Boolean</span></span>|<span data-ttu-id="ba5c3-206">Gibt an, ob displaytone-Setupbildschirm deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-207">privacyPaneDisabled</span></span>|<span data-ttu-id="ba5c3-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-208">Boolean</span></span>|<span data-ttu-id="ba5c3-209">Gibt an, ob der Datenschutz Bildschirm deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba5c3-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ba5c3-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ba5c3-210">iTunesPairingMode</span></span>|[<span data-ttu-id="ba5c3-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ba5c3-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="ba5c3-212">Gibt den iTunes-paarungsmodus an.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="ba5c3-213">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="ba5c3-214">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="ba5c3-214">managementCertificates</span></span>|<span data-ttu-id="ba5c3-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="ba5c3-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="ba5c3-216">Verwaltungszertifikate für Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="ba5c3-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="ba5c3-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="ba5c3-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-218">Boolean</span></span>|<span data-ttu-id="ba5c3-219">Gibt an, ob die Wiederherstellung von Android deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="ba5c3-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="ba5c3-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="ba5c3-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-221">Boolean</span></span>|<span data-ttu-id="ba5c3-222">Gibt an, ob das Gerät auf die konfigurierte Bestätigung warten muss.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="ba5c3-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="ba5c3-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="ba5c3-224">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5c3-224">Int32</span></span>|<span data-ttu-id="ba5c3-225">Dies gibt die maximale Anzahl von Benutzern an, die ein freigegebenes iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="ba5c3-226">Gilt nur für den freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="ba5c3-227">Enablesharedipad wurden</span><span class="sxs-lookup"><span data-stu-id="ba5c3-227">enableSharedIPad</span></span>|<span data-ttu-id="ba5c3-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-228">Boolean</span></span>|<span data-ttu-id="ba5c3-229">Dieser Wert gibt an, ob das Gerät in einen Modus eingeschrieben werden soll, der mehrere Benutzerszenarien ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="ba5c3-230">Gilt nur für freigegebene iPads.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="ba5c3-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="ba5c3-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="ba5c3-232">String</span><span class="sxs-lookup"><span data-stu-id="ba5c3-232">String</span></span>|<span data-ttu-id="ba5c3-233">Wenn festgelegt, gibt das VSS-Token an, das zum Bereitstellen des Unternehmensportals mit der Geräte Lizenzierung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="ba5c3-234">' enableAuthenticationViaCompanyPortal ' muss festgelegt werden, damit diese Eigenschaft festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="ba5c3-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="ba5c3-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="ba5c3-236">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-236">Boolean</span></span>|<span data-ttu-id="ba5c3-237">Weist das Gerät an, den Einzel APP-Modus zu aktivieren und die APP-Sperre während der Registrierung anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="ba5c3-238">Default is „false“.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-238">Default is false.</span></span> <span data-ttu-id="ba5c3-239">"enableAuthenticationViaCompanyPortal" und "companyPortalVppTokenId" müssen festgelegt werden, damit diese Eigenschaft festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="ba5c3-240">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="ba5c3-241">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-241">Boolean</span></span>|<span data-ttu-id="ba5c3-242">Gibt an, ob der Bildschirm für die Home-Schaltfläche deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="ba5c3-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="ba5c3-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="ba5c3-244">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-244">Boolean</span></span>|<span data-ttu-id="ba5c3-245">Gibt an, ob iMessage-und FaceTime-Bildschirm deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="ba5c3-246">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="ba5c3-247">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-247">Boolean</span></span>|<span data-ttu-id="ba5c3-248">Gibt an, ob der Bildschirm Onboarding Setup deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="ba5c3-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="ba5c3-250">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-250">Boolean</span></span>|<span data-ttu-id="ba5c3-251">Gibt an, ob die Installation des Bildschirm Timeouts deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="ba5c3-252">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="ba5c3-253">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-253">Boolean</span></span>|<span data-ttu-id="ba5c3-254">Gibt an, ob der SIMSetup-Bildschirm deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="ba5c3-255">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="ba5c3-256">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-256">Boolean</span></span>|<span data-ttu-id="ba5c3-257">Gibt an, ob der Bildschirm obligatorische Softwareaktualisierung deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="ba5c3-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ba5c3-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="ba5c3-259">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ba5c3-259">Boolean</span></span>|<span data-ttu-id="ba5c3-260">Gibt an, ob der Bildschirm für die Überwachung der Migration deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="ba5c3-261">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba5c3-261">Response</span></span>
<span data-ttu-id="ba5c3-262">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-262">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba5c3-263">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba5c3-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba5c3-264">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba5c3-264">Request</span></span>
<span data-ttu-id="ba5c3-265">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1736

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="ba5c3-266">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba5c3-266">Response</span></span>
<span data-ttu-id="ba5c3-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba5c3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1785

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




