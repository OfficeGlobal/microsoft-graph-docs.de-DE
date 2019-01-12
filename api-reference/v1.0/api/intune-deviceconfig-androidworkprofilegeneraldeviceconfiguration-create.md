---
title: Erstellen von androidWorkProfileGeneralDeviceConfiguration
description: Erstellen eines neuen AndroidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 92cdd51d4bf68aa4607b71ca31c10b35277a06ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912799"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="783ed-103">Erstellen von androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="783ed-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="783ed-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="783ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="783ed-105">Erstellen eines neuen [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="783ed-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="783ed-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="783ed-106">Prerequisites</span></span>
<span data-ttu-id="783ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="783ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="783ed-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="783ed-109">Permission type</span></span>|<span data-ttu-id="783ed-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="783ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="783ed-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="783ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="783ed-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="783ed-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="783ed-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="783ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="783ed-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="783ed-114">Not supported.</span></span>|
|<span data-ttu-id="783ed-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="783ed-115">Application</span></span>|<span data-ttu-id="783ed-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="783ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="783ed-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="783ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="783ed-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="783ed-118">Request headers</span></span>
|<span data-ttu-id="783ed-119">Header</span><span class="sxs-lookup"><span data-stu-id="783ed-119">Header</span></span>|<span data-ttu-id="783ed-120">Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="783ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="783ed-121">Authorization</span></span>|<span data-ttu-id="783ed-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="783ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="783ed-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="783ed-123">Accept</span></span>|<span data-ttu-id="783ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="783ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="783ed-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="783ed-125">Request body</span></span>
<span data-ttu-id="783ed-126">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileGeneralDeviceConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="783ed-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="783ed-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="783ed-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="783ed-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="783ed-128">Property</span></span>|<span data-ttu-id="783ed-129">Typ</span><span class="sxs-lookup"><span data-stu-id="783ed-129">Type</span></span>|<span data-ttu-id="783ed-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="783ed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="783ed-131">id</span><span class="sxs-lookup"><span data-stu-id="783ed-131">id</span></span>|<span data-ttu-id="783ed-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="783ed-132">String</span></span>|<span data-ttu-id="783ed-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="783ed-133">Key of the entity.</span></span> <span data-ttu-id="783ed-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="783ed-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="783ed-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="783ed-135">lastModifiedDateTime</span></span>|<span data-ttu-id="783ed-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="783ed-136">DateTimeOffset</span></span>|<span data-ttu-id="783ed-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="783ed-137">DateTime the object was last modified.</span></span> <span data-ttu-id="783ed-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="783ed-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="783ed-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="783ed-139">createdDateTime</span></span>|<span data-ttu-id="783ed-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="783ed-140">DateTimeOffset</span></span>|<span data-ttu-id="783ed-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="783ed-141">DateTime the object was created.</span></span> <span data-ttu-id="783ed-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="783ed-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="783ed-143">description</span><span class="sxs-lookup"><span data-stu-id="783ed-143">description</span></span>|<span data-ttu-id="783ed-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="783ed-144">String</span></span>|<span data-ttu-id="783ed-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="783ed-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="783ed-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="783ed-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="783ed-147">displayName</span><span class="sxs-lookup"><span data-stu-id="783ed-147">displayName</span></span>|<span data-ttu-id="783ed-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="783ed-148">String</span></span>|<span data-ttu-id="783ed-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="783ed-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="783ed-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="783ed-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="783ed-151">Version</span><span class="sxs-lookup"><span data-stu-id="783ed-151">version</span></span>|<span data-ttu-id="783ed-152">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-152">Int32</span></span>|<span data-ttu-id="783ed-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="783ed-153">Version of the device configuration.</span></span> <span data-ttu-id="783ed-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="783ed-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="783ed-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="783ed-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="783ed-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-156">Boolean</span></span>|<span data-ttu-id="783ed-157">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="783ed-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="783ed-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="783ed-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="783ed-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-159">Boolean</span></span>|<span data-ttu-id="783ed-160">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="783ed-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="783ed-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="783ed-161">passwordExpirationDays</span></span>|<span data-ttu-id="783ed-162">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-162">Int32</span></span>|<span data-ttu-id="783ed-163">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="783ed-163">Number of days before the password expires.</span></span> <span data-ttu-id="783ed-164">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="783ed-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="783ed-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="783ed-165">passwordMinimumLength</span></span>|<span data-ttu-id="783ed-166">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-166">Int32</span></span>|<span data-ttu-id="783ed-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="783ed-167">Minimum length of passwords.</span></span> <span data-ttu-id="783ed-168">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="783ed-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="783ed-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="783ed-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="783ed-170">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-170">Int32</span></span>|<span data-ttu-id="783ed-171">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="783ed-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="783ed-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="783ed-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="783ed-173">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-173">Int32</span></span>|<span data-ttu-id="783ed-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="783ed-174">Number of previous passwords to block.</span></span> <span data-ttu-id="783ed-175">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="783ed-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="783ed-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="783ed-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="783ed-177">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-177">Int32</span></span>|<span data-ttu-id="783ed-178">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="783ed-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="783ed-179">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="783ed-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="783ed-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="783ed-180">passwordRequiredType</span></span>|[<span data-ttu-id="783ed-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="783ed-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="783ed-182">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="783ed-182">Type of password that is required.</span></span> <span data-ttu-id="783ed-183">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="783ed-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="783ed-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="783ed-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="783ed-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="783ed-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="783ed-186">Typ der Daten, die Freigabe ist zulässig.</span><span class="sxs-lookup"><span data-stu-id="783ed-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="783ed-187">Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="783ed-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="783ed-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="783ed-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="783ed-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-189">Boolean</span></span>|<span data-ttu-id="783ed-190">Gibt an, ob beim Gerät gesperrt Benachrichtigungen zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="783ed-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="783ed-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="783ed-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="783ed-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-192">Boolean</span></span>|<span data-ttu-id="783ed-193">Blockieren Sie den Benutzer hinzufügen/entfernen von Konten im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="783ed-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="783ed-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="783ed-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="783ed-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-195">Boolean</span></span>|<span data-ttu-id="783ed-196">Können Sie Bluetooth-Geräte können Kontakte im Unternehmen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="783ed-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="783ed-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="783ed-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="783ed-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-198">Boolean</span></span>|<span data-ttu-id="783ed-199">Blockiert die Bildschirmaufnahme im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="783ed-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="783ed-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="783ed-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="783ed-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-201">Boolean</span></span>|<span data-ttu-id="783ed-202">Block Anzeige Arbeit Profil Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="783ed-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="783ed-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="783ed-203">workProfileBlockCamera</span></span>|<span data-ttu-id="783ed-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-204">Boolean</span></span>|<span data-ttu-id="783ed-205">Blockieren der Profil Kamera.</span><span class="sxs-lookup"><span data-stu-id="783ed-205">Block work profile camera.</span></span>|
|<span data-ttu-id="783ed-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="783ed-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="783ed-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-207">Boolean</span></span>|<span data-ttu-id="783ed-208">Verfügbarkeit der Block Arbeit Profil Kontakte im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="783ed-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="783ed-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="783ed-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="783ed-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-210">Boolean</span></span>|<span data-ttu-id="783ed-211">Boolescher Wert, der angibt, wenn die Einstellung firewallübergreifenden disallow Profil kopieren und einfügen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="783ed-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="783ed-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="783ed-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="783ed-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="783ed-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="783ed-214">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="783ed-214">Type of password that is required.</span></span> <span data-ttu-id="783ed-215">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="783ed-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="783ed-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="783ed-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="783ed-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-217">Boolean</span></span>|<span data-ttu-id="783ed-218">Gibt an, ob blockieren Fingerabdruck Entsperren für Arbeit Profil.</span><span class="sxs-lookup"><span data-stu-id="783ed-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="783ed-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="783ed-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="783ed-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-220">Boolean</span></span>|<span data-ttu-id="783ed-221">Gibt an, ob intelligente sperren und andere Trust-Agenten für Arbeit Profil zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="783ed-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="783ed-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="783ed-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="783ed-223">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-223">Int32</span></span>|<span data-ttu-id="783ed-224">Anzahl von Tagen vor der Arbeit Profilkennwort läuft ab.</span><span class="sxs-lookup"><span data-stu-id="783ed-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="783ed-225">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="783ed-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="783ed-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="783ed-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="783ed-227">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-227">Int32</span></span>|<span data-ttu-id="783ed-228">Minimale Länge der Arbeit Profilkennwort.</span><span class="sxs-lookup"><span data-stu-id="783ed-228">Minimum length of work profile password.</span></span> <span data-ttu-id="783ed-229">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="783ed-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="783ed-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="783ed-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="783ed-231">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-231">Int32</span></span>|<span data-ttu-id="783ed-232">Minimale Anzahl der numerische Zeichen in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="783ed-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="783ed-233">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="783ed-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="783ed-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="783ed-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="783ed-235">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-235">Int32</span></span>|<span data-ttu-id="783ed-236">Minimale Anzahl der nicht-Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="783ed-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="783ed-237">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="783ed-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="783ed-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="783ed-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="783ed-239">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-239">Int32</span></span>|<span data-ttu-id="783ed-240">Minimale Anzahl der Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="783ed-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="783ed-241">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="783ed-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="783ed-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="783ed-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="783ed-243">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-243">Int32</span></span>|<span data-ttu-id="783ed-244">Minimale Anzahl der Kleinbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="783ed-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="783ed-245">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="783ed-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="783ed-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="783ed-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="783ed-247">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-247">Int32</span></span>|<span data-ttu-id="783ed-248">Minimale Anzahl der Großbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="783ed-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="783ed-249">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="783ed-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="783ed-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="783ed-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="783ed-251">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-251">Int32</span></span>|<span data-ttu-id="783ed-252">Minimale Anzahl der Symbole in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="783ed-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="783ed-253">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="783ed-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="783ed-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="783ed-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="783ed-255">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-255">Int32</span></span>|<span data-ttu-id="783ed-256">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="783ed-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="783ed-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="783ed-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="783ed-258">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-258">Int32</span></span>|<span data-ttu-id="783ed-259">Anzahl der vorherigen Arbeit Profil Kennwörter zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="783ed-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="783ed-260">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="783ed-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="783ed-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="783ed-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="783ed-262">Int32</span><span class="sxs-lookup"><span data-stu-id="783ed-262">Int32</span></span>|<span data-ttu-id="783ed-263">Anzahl der Anmeldung Fehler zulässig sind, bevor Arbeit Profil entfernt wird und alle Daten gelöscht.</span><span class="sxs-lookup"><span data-stu-id="783ed-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="783ed-264">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="783ed-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="783ed-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="783ed-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="783ed-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="783ed-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="783ed-267">Typ der Arbeit Profilkennwort, das erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="783ed-267">Type of work profile password that is required.</span></span> <span data-ttu-id="783ed-268">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="783ed-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="783ed-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="783ed-269">workProfileRequirePassword</span></span>|<span data-ttu-id="783ed-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-270">Boolean</span></span>|<span data-ttu-id="783ed-271">Kennwort erforderlich ist oder nicht für Arbeit Profil</span><span class="sxs-lookup"><span data-stu-id="783ed-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="783ed-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="783ed-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="783ed-273">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="783ed-273">Boolean</span></span>|<span data-ttu-id="783ed-274">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="783ed-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="783ed-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="783ed-275">Response</span></span>
<span data-ttu-id="783ed-276">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="783ed-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="783ed-277">Beispiel</span><span class="sxs-lookup"><span data-stu-id="783ed-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="783ed-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="783ed-278">Request</span></span>
<span data-ttu-id="783ed-279">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="783ed-279">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="783ed-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="783ed-280">Response</span></span>
<span data-ttu-id="783ed-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="783ed-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



