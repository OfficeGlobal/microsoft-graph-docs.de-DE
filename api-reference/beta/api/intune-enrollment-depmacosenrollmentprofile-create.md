---
title: Erstellen von depMacOSEnrollmentProfile
description: Erstellen eines neuen DepMacOSEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f61ace61d1ce06be6d448b221924e4ec8a4f7505
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971326"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="66b7d-103">Erstellen von depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="66b7d-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="66b7d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66b7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66b7d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66b7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66b7d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66b7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66b7d-107">Erstellen eines neuen [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="66b7d-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66b7d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66b7d-108">Prerequisites</span></span>
<span data-ttu-id="66b7d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66b7d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66b7d-111">Permission type</span></span>|<span data-ttu-id="66b7d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66b7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66b7d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66b7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66b7d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66b7d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="66b7d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66b7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66b7d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66b7d-116">Not supported.</span></span>|
|<span data-ttu-id="66b7d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66b7d-117">Application</span></span>|<span data-ttu-id="66b7d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66b7d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66b7d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66b7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="66b7d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66b7d-120">Request headers</span></span>
|<span data-ttu-id="66b7d-121">Header</span><span class="sxs-lookup"><span data-stu-id="66b7d-121">Header</span></span>|<span data-ttu-id="66b7d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66b7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66b7d-123">Authorization</span></span>|<span data-ttu-id="66b7d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66b7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66b7d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66b7d-125">Accept</span></span>|<span data-ttu-id="66b7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66b7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66b7d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66b7d-127">Request body</span></span>
<span data-ttu-id="66b7d-128">Geben Sie im Textkörper Anforderung für das Objekt DepMacOSEnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="66b7d-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="66b7d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepMacOSEnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="66b7d-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="66b7d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66b7d-130">Property</span></span>|<span data-ttu-id="66b7d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="66b7d-131">Type</span></span>|<span data-ttu-id="66b7d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66b7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b7d-133">id</span><span class="sxs-lookup"><span data-stu-id="66b7d-133">id</span></span>|<span data-ttu-id="66b7d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b7d-134">String</span></span>|<span data-ttu-id="66b7d-135">Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="66b7d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="66b7d-136">displayName</span></span>|<span data-ttu-id="66b7d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b7d-137">String</span></span>|<span data-ttu-id="66b7d-138">Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="66b7d-139">description</span><span class="sxs-lookup"><span data-stu-id="66b7d-139">description</span></span>|<span data-ttu-id="66b7d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b7d-140">String</span></span>|<span data-ttu-id="66b7d-141">Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="66b7d-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="66b7d-142">requiresUserAuthentication</span></span>|<span data-ttu-id="66b7d-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-143">Boolean</span></span>|<span data-ttu-id="66b7d-144">Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert</span><span class="sxs-lookup"><span data-stu-id="66b7d-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="66b7d-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="66b7d-145">configurationEndpointUrl</span></span>|<span data-ttu-id="66b7d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b7d-146">String</span></span>|<span data-ttu-id="66b7d-147">Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="66b7d-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="66b7d-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="66b7d-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="66b7d-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-149">Boolean</span></span>|<span data-ttu-id="66b7d-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="66b7d-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="66b7d-151">Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="66b7d-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="66b7d-152">isDefault</span></span>|<span data-ttu-id="66b7d-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-153">Boolean</span></span>|<span data-ttu-id="66b7d-154">Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-155">supervisedModeEnabled</span></span>|<span data-ttu-id="66b7d-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-156">Boolean</span></span>|<span data-ttu-id="66b7d-157">Überwachten Modus aktivieren, False andernfalls True.</span><span class="sxs-lookup"><span data-stu-id="66b7d-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="66b7d-158">Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="66b7d-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="66b7d-159">Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="66b7d-160">supportDepartment</span></span>|<span data-ttu-id="66b7d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b7d-161">String</span></span>|<span data-ttu-id="66b7d-162">Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-163">passCodeDisabled</span></span>|<span data-ttu-id="66b7d-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-164">Boolean</span></span>|<span data-ttu-id="66b7d-165">Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="66b7d-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="66b7d-166">isMandatory</span></span>|<span data-ttu-id="66b7d-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-167">Boolean</span></span>|<span data-ttu-id="66b7d-168">Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-169">locationDisabled</span></span>|<span data-ttu-id="66b7d-170">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-170">Boolean</span></span>|<span data-ttu-id="66b7d-171">Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="66b7d-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="66b7d-172">supportPhoneNumber</span></span>|<span data-ttu-id="66b7d-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b7d-173">String</span></span>|<span data-ttu-id="66b7d-174">Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b7d-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-175">profileRemovalDisabled</span></span>|<span data-ttu-id="66b7d-176">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-176">Boolean</span></span>|<span data-ttu-id="66b7d-177">Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="66b7d-178">restoreBlocked</span></span>|<span data-ttu-id="66b7d-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-179">Boolean</span></span>|<span data-ttu-id="66b7d-180">Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-181">appleIdDisabled</span></span>|<span data-ttu-id="66b7d-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-182">Boolean</span></span>|<span data-ttu-id="66b7d-183">Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="66b7d-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="66b7d-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-185">Boolean</span></span>|<span data-ttu-id="66b7d-186">Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-187">touchIdDisabled</span></span>|<span data-ttu-id="66b7d-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-188">Boolean</span></span>|<span data-ttu-id="66b7d-189">Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-190">applePayDisabled</span></span>|<span data-ttu-id="66b7d-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-191">Boolean</span></span>|<span data-ttu-id="66b7d-192">Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-193">zoomDisabled</span></span>|<span data-ttu-id="66b7d-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-194">Boolean</span></span>|<span data-ttu-id="66b7d-195">Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-196">siriDisabled</span></span>|<span data-ttu-id="66b7d-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-197">Boolean</span></span>|<span data-ttu-id="66b7d-198">Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="66b7d-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-199">diagnosticsDisabled</span></span>|<span data-ttu-id="66b7d-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-200">Boolean</span></span>|<span data-ttu-id="66b7d-201">Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert</span><span class="sxs-lookup"><span data-stu-id="66b7d-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="66b7d-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-202">registrationDisabled</span></span>|<span data-ttu-id="66b7d-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-203">Boolean</span></span>|<span data-ttu-id="66b7d-204">Gibt an, ob die Registrierung deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="66b7d-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="66b7d-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-205">fileVaultDisabled</span></span>|<span data-ttu-id="66b7d-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-206">Boolean</span></span>|<span data-ttu-id="66b7d-207">Gibt an, ob die Datei Vault deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="66b7d-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="66b7d-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="66b7d-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="66b7d-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="66b7d-209">Boolean</span></span>|<span data-ttu-id="66b7d-210">Gibt an, ob iCloud Analytics Bildschirm deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="66b7d-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="66b7d-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="66b7d-211">Response</span></span>
<span data-ttu-id="66b7d-212">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="66b7d-212">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66b7d-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66b7d-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="66b7d-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66b7d-214">Request</span></span>
<span data-ttu-id="66b7d-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66b7d-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66b7d-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="66b7d-216">Response</span></span>
<span data-ttu-id="66b7d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66b7d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





