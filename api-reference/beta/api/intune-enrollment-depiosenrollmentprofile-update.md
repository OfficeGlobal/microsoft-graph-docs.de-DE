---
title: DepIOSEnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DepIOSEnrollmentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e36951d69f3047c69ccfc0d1e0a72247a0715db9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400592"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="21ee6-103">DepIOSEnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="21ee6-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="21ee6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="21ee6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21ee6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21ee6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21ee6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ee6-107">Aktualisieren Sie die Eigenschaften eines [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="21ee6-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21ee6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21ee6-108">Prerequisites</span></span>
<span data-ttu-id="21ee6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21ee6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21ee6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21ee6-111">Permission type</span></span>|<span data-ttu-id="21ee6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21ee6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21ee6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21ee6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21ee6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21ee6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21ee6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21ee6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21ee6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21ee6-116">Not supported.</span></span>|
|<span data-ttu-id="21ee6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21ee6-117">Application</span></span>|<span data-ttu-id="21ee6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21ee6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21ee6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21ee6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="21ee6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21ee6-120">Request headers</span></span>
|<span data-ttu-id="21ee6-121">Header</span><span class="sxs-lookup"><span data-stu-id="21ee6-121">Header</span></span>|<span data-ttu-id="21ee6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="21ee6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21ee6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="21ee6-123">Authorization</span></span>|<span data-ttu-id="21ee6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21ee6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21ee6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21ee6-125">Accept</span></span>|<span data-ttu-id="21ee6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21ee6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21ee6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21ee6-127">Request body</span></span>
<span data-ttu-id="21ee6-128">Geben Sie im Textkörper Anforderung für das Objekt [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="21ee6-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="21ee6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="21ee6-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="21ee6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21ee6-130">Property</span></span>|<span data-ttu-id="21ee6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="21ee6-131">Type</span></span>|<span data-ttu-id="21ee6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21ee6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ee6-133">id</span><span class="sxs-lookup"><span data-stu-id="21ee6-133">id</span></span>|<span data-ttu-id="21ee6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-134">String</span></span>|<span data-ttu-id="21ee6-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="21ee6-136">displayName</span></span>|<span data-ttu-id="21ee6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-137">String</span></span>|<span data-ttu-id="21ee6-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-139">description</span><span class="sxs-lookup"><span data-stu-id="21ee6-139">description</span></span>|<span data-ttu-id="21ee6-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-140">String</span></span>|<span data-ttu-id="21ee6-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="21ee6-142">requiresUserAuthentication</span></span>|<span data-ttu-id="21ee6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-143">Boolean</span></span>|<span data-ttu-id="21ee6-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="21ee6-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="21ee6-145">configurationEndpointUrl</span></span>|<span data-ttu-id="21ee6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-146">String</span></span>|<span data-ttu-id="21ee6-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="21ee6-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="21ee6-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="21ee6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-149">Boolean</span></span>|<span data-ttu-id="21ee6-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="21ee6-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="21ee6-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="21ee6-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="21ee6-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-153">Boolean</span></span>|<span data-ttu-id="21ee6-154">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="21ee6-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="21ee6-155">isDefault</span></span>|<span data-ttu-id="21ee6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-156">Boolean</span></span>|<span data-ttu-id="21ee6-157">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-158">supervisedModeEnabled</span></span>|<span data-ttu-id="21ee6-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-159">Boolean</span></span>|<span data-ttu-id="21ee6-160">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="21ee6-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="21ee6-161">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="21ee6-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="21ee6-162">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="21ee6-163">supportDepartment</span></span>|<span data-ttu-id="21ee6-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-164">String</span></span>|<span data-ttu-id="21ee6-165">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-166">passCodeDisabled</span></span>|<span data-ttu-id="21ee6-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-167">Boolean</span></span>|<span data-ttu-id="21ee6-168">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="21ee6-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="21ee6-169">isMandatory</span></span>|<span data-ttu-id="21ee6-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-170">Boolean</span></span>|<span data-ttu-id="21ee6-171">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-172">locationDisabled</span></span>|<span data-ttu-id="21ee6-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-173">Boolean</span></span>|<span data-ttu-id="21ee6-174">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="21ee6-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="21ee6-175">supportPhoneNumber</span></span>|<span data-ttu-id="21ee6-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-176">String</span></span>|<span data-ttu-id="21ee6-177">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="21ee6-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-178">profileRemovalDisabled</span></span>|<span data-ttu-id="21ee6-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-179">Boolean</span></span>|<span data-ttu-id="21ee6-180">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="21ee6-181">restoreBlocked</span></span>|<span data-ttu-id="21ee6-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-182">Boolean</span></span>|<span data-ttu-id="21ee6-183">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-184">appleIdDisabled</span></span>|<span data-ttu-id="21ee6-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-185">Boolean</span></span>|<span data-ttu-id="21ee6-186">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="21ee6-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="21ee6-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-188">Boolean</span></span>|<span data-ttu-id="21ee6-189">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-190">touchIdDisabled</span></span>|<span data-ttu-id="21ee6-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-191">Boolean</span></span>|<span data-ttu-id="21ee6-192">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-193">applePayDisabled</span></span>|<span data-ttu-id="21ee6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-194">Boolean</span></span>|<span data-ttu-id="21ee6-195">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-196">zoomDisabled</span></span>|<span data-ttu-id="21ee6-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-197">Boolean</span></span>|<span data-ttu-id="21ee6-198">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-199">siriDisabled</span></span>|<span data-ttu-id="21ee6-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-200">Boolean</span></span>|<span data-ttu-id="21ee6-201">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-202">diagnosticsDisabled</span></span>|<span data-ttu-id="21ee6-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-203">Boolean</span></span>|<span data-ttu-id="21ee6-204">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="21ee6-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="21ee6-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-206">Boolean</span></span>|<span data-ttu-id="21ee6-207">Gibt an, ob Displaytone Setupbildschirm deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-208">privacyPaneDisabled</span></span>|<span data-ttu-id="21ee6-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-209">Boolean</span></span>|<span data-ttu-id="21ee6-210">Gibt an, ob Privacy Bildschirm deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="21ee6-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="21ee6-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="21ee6-211">iTunesPairingMode</span></span>|[<span data-ttu-id="21ee6-212">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="21ee6-212">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="21ee6-213">Gibt den Modus Paarung iTunes an.</span><span class="sxs-lookup"><span data-stu-id="21ee6-213">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="21ee6-214">Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="21ee6-214">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="21ee6-215">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="21ee6-215">managementCertificates</span></span>|<span data-ttu-id="21ee6-216">[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="21ee6-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="21ee6-217">Verwaltung von Zertifikaten für Apple-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="21ee6-217">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="21ee6-218">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-218">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="21ee6-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-219">Boolean</span></span>|<span data-ttu-id="21ee6-220">Gibt an, ob die Wiederherstellung von Android deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-220">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="21ee6-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="21ee6-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="21ee6-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-222">Boolean</span></span>|<span data-ttu-id="21ee6-223">Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen</span><span class="sxs-lookup"><span data-stu-id="21ee6-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="21ee6-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="21ee6-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="21ee6-225">Int32</span><span class="sxs-lookup"><span data-stu-id="21ee6-225">Int32</span></span>|<span data-ttu-id="21ee6-226">Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können.</span><span class="sxs-lookup"><span data-stu-id="21ee6-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="21ee6-227">Gilt nur im freigegebenen iPad-Modus.</span><span class="sxs-lookup"><span data-stu-id="21ee6-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="21ee6-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="21ee6-228">enableSharedIPad</span></span>|<span data-ttu-id="21ee6-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-229">Boolean</span></span>|<span data-ttu-id="21ee6-230">Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien.</span><span class="sxs-lookup"><span data-stu-id="21ee6-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="21ee6-231">Nur im freigegebenen iPads anwendbar.</span><span class="sxs-lookup"><span data-stu-id="21ee6-231">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="21ee6-232">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="21ee6-232">companyPortalVppTokenId</span></span>|<span data-ttu-id="21ee6-233">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21ee6-233">String</span></span>|<span data-ttu-id="21ee6-234">Wenn festgelegt ist, gibt an, welche Vpp Token zum Bereitstellen der Unternehmensportal mit Gerät-Lizenzierung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="21ee6-234">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="21ee6-235">'EnableAuthenticationViaCompanyPortal' muss für diese Eigenschaft festgelegt werden soll festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="21ee6-235">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="21ee6-236">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="21ee6-236">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="21ee6-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-237">Boolean</span></span>|<span data-ttu-id="21ee6-238">Weist das Gerät zum Aktivieren der einzelnen app-Modus und Anwenden von app-Sperre während der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="21ee6-238">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="21ee6-239">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="21ee6-239">Default is false.</span></span> <span data-ttu-id="21ee6-240">'EnableAuthenticationViaCompanyPortal' und 'CompanyPortalVppTokenId' müssen für diese Eigenschaft festgelegt werden soll, festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="21ee6-240">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="21ee6-241">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-241">homeButtonScreenDisabled</span></span>|<span data-ttu-id="21ee6-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-242">Boolean</span></span>|<span data-ttu-id="21ee6-243">Gibt an, ob die Vertraulichkeit Bildschirm home-Schaltfläche deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-243">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="21ee6-244">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-244">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="21ee6-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-245">Boolean</span></span>|<span data-ttu-id="21ee6-246">Gibt an, ob iMessage und FaceTime Bildschirm ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="21ee6-246">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="21ee6-247">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-247">onBoardingScreenDisabled</span></span>|<span data-ttu-id="21ee6-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-248">Boolean</span></span>|<span data-ttu-id="21ee6-249">Gibt an, ob Onboarding Setupbildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-249">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="21ee6-250">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-250">screenTimeScreenDisabled</span></span>|<span data-ttu-id="21ee6-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-251">Boolean</span></span>|<span data-ttu-id="21ee6-252">Gibt an, ob der Bildschirm Timeout-Setup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-252">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="21ee6-253">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-253">simSetupScreenDisabled</span></span>|<span data-ttu-id="21ee6-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-254">Boolean</span></span>|<span data-ttu-id="21ee6-255">Gibt an, ob der Bildschirm SIMSetup deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-255">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="21ee6-256">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-256">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="21ee6-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-257">Boolean</span></span>|<span data-ttu-id="21ee6-258">Gibt an, ob der obligatorische Software Update Bildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-258">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="21ee6-259">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="21ee6-259">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="21ee6-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ee6-260">Boolean</span></span>|<span data-ttu-id="21ee6-261">Gibt an, ob auf dem Bildschirm Watch Migration deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="21ee6-261">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="21ee6-262">Antwort</span><span class="sxs-lookup"><span data-stu-id="21ee6-262">Response</span></span>
<span data-ttu-id="21ee6-263">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="21ee6-263">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21ee6-264">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21ee6-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="21ee6-265">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21ee6-265">Request</span></span>
<span data-ttu-id="21ee6-266">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21ee6-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21ee6-267">Antwort</span><span class="sxs-lookup"><span data-stu-id="21ee6-267">Response</span></span>
<span data-ttu-id="21ee6-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21ee6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




