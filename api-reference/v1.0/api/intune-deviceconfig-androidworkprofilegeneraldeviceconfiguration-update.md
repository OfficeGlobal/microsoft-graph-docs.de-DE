---
title: AndroidWorkProfileGeneralDeviceConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c9e150fc722842c3d904f2cb06a4127e96fc61c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943956"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="80aae-103">AndroidWorkProfileGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="80aae-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="80aae-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80aae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80aae-105">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="80aae-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80aae-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80aae-106">Prerequisites</span></span>
<span data-ttu-id="80aae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80aae-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80aae-109">Permission type</span></span>|<span data-ttu-id="80aae-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80aae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80aae-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80aae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80aae-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80aae-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80aae-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80aae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80aae-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80aae-114">Not supported.</span></span>|
|<span data-ttu-id="80aae-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80aae-115">Application</span></span>|<span data-ttu-id="80aae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80aae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80aae-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80aae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80aae-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80aae-118">Request headers</span></span>
|<span data-ttu-id="80aae-119">Header</span><span class="sxs-lookup"><span data-stu-id="80aae-119">Header</span></span>|<span data-ttu-id="80aae-120">Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80aae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80aae-121">Authorization</span></span>|<span data-ttu-id="80aae-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80aae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80aae-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80aae-123">Accept</span></span>|<span data-ttu-id="80aae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80aae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80aae-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80aae-125">Request body</span></span>
<span data-ttu-id="80aae-126">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="80aae-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="80aae-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="80aae-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="80aae-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80aae-128">Property</span></span>|<span data-ttu-id="80aae-129">Typ</span><span class="sxs-lookup"><span data-stu-id="80aae-129">Type</span></span>|<span data-ttu-id="80aae-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80aae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80aae-131">id</span><span class="sxs-lookup"><span data-stu-id="80aae-131">id</span></span>|<span data-ttu-id="80aae-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80aae-132">String</span></span>|<span data-ttu-id="80aae-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="80aae-133">Key of the entity.</span></span> <span data-ttu-id="80aae-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80aae-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80aae-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80aae-135">lastModifiedDateTime</span></span>|<span data-ttu-id="80aae-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80aae-136">DateTimeOffset</span></span>|<span data-ttu-id="80aae-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80aae-137">DateTime the object was last modified.</span></span> <span data-ttu-id="80aae-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80aae-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80aae-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80aae-139">createdDateTime</span></span>|<span data-ttu-id="80aae-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80aae-140">DateTimeOffset</span></span>|<span data-ttu-id="80aae-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="80aae-141">DateTime the object was created.</span></span> <span data-ttu-id="80aae-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80aae-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80aae-143">description</span><span class="sxs-lookup"><span data-stu-id="80aae-143">description</span></span>|<span data-ttu-id="80aae-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80aae-144">String</span></span>|<span data-ttu-id="80aae-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80aae-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80aae-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80aae-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80aae-147">displayName</span><span class="sxs-lookup"><span data-stu-id="80aae-147">displayName</span></span>|<span data-ttu-id="80aae-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80aae-148">String</span></span>|<span data-ttu-id="80aae-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="80aae-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80aae-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80aae-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80aae-151">Version</span><span class="sxs-lookup"><span data-stu-id="80aae-151">version</span></span>|<span data-ttu-id="80aae-152">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-152">Int32</span></span>|<span data-ttu-id="80aae-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="80aae-153">Version of the device configuration.</span></span> <span data-ttu-id="80aae-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80aae-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80aae-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="80aae-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="80aae-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-156">Boolean</span></span>|<span data-ttu-id="80aae-157">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="80aae-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="80aae-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="80aae-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="80aae-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-159">Boolean</span></span>|<span data-ttu-id="80aae-160">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="80aae-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="80aae-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="80aae-161">passwordExpirationDays</span></span>|<span data-ttu-id="80aae-162">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-162">Int32</span></span>|<span data-ttu-id="80aae-163">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="80aae-163">Number of days before the password expires.</span></span> <span data-ttu-id="80aae-164">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="80aae-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="80aae-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="80aae-165">passwordMinimumLength</span></span>|<span data-ttu-id="80aae-166">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-166">Int32</span></span>|<span data-ttu-id="80aae-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="80aae-167">Minimum length of passwords.</span></span> <span data-ttu-id="80aae-168">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="80aae-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="80aae-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="80aae-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="80aae-170">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-170">Int32</span></span>|<span data-ttu-id="80aae-171">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="80aae-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="80aae-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="80aae-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="80aae-173">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-173">Int32</span></span>|<span data-ttu-id="80aae-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="80aae-174">Number of previous passwords to block.</span></span> <span data-ttu-id="80aae-175">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="80aae-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="80aae-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="80aae-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="80aae-177">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-177">Int32</span></span>|<span data-ttu-id="80aae-178">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="80aae-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="80aae-179">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="80aae-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="80aae-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="80aae-180">passwordRequiredType</span></span>|[<span data-ttu-id="80aae-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80aae-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="80aae-182">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="80aae-182">Type of password that is required.</span></span> <span data-ttu-id="80aae-183">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="80aae-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="80aae-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="80aae-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="80aae-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="80aae-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="80aae-186">Typ der Daten, die Freigabe ist zulässig.</span><span class="sxs-lookup"><span data-stu-id="80aae-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="80aae-187">Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="80aae-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="80aae-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="80aae-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="80aae-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-189">Boolean</span></span>|<span data-ttu-id="80aae-190">Gibt an, ob beim Gerät gesperrt Benachrichtigungen zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="80aae-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="80aae-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="80aae-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="80aae-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-192">Boolean</span></span>|<span data-ttu-id="80aae-193">Blockieren Sie den Benutzer hinzufügen/entfernen von Konten im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="80aae-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="80aae-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="80aae-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="80aae-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-195">Boolean</span></span>|<span data-ttu-id="80aae-196">Können Sie Bluetooth-Geräte können Kontakte im Unternehmen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="80aae-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="80aae-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="80aae-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="80aae-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-198">Boolean</span></span>|<span data-ttu-id="80aae-199">Blockiert die Bildschirmaufnahme im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="80aae-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="80aae-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="80aae-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="80aae-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-201">Boolean</span></span>|<span data-ttu-id="80aae-202">Block Anzeige Arbeit Profil Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="80aae-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="80aae-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="80aae-203">workProfileBlockCamera</span></span>|<span data-ttu-id="80aae-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-204">Boolean</span></span>|<span data-ttu-id="80aae-205">Blockieren der Profil Kamera.</span><span class="sxs-lookup"><span data-stu-id="80aae-205">Block work profile camera.</span></span>|
|<span data-ttu-id="80aae-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="80aae-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="80aae-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-207">Boolean</span></span>|<span data-ttu-id="80aae-208">Verfügbarkeit der Block Arbeit Profil Kontakte im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="80aae-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="80aae-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="80aae-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="80aae-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-210">Boolean</span></span>|<span data-ttu-id="80aae-211">Boolescher Wert, der angibt, wenn die Einstellung firewallübergreifenden disallow Profil kopieren und einfügen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="80aae-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="80aae-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="80aae-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="80aae-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="80aae-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="80aae-214">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="80aae-214">Type of password that is required.</span></span> <span data-ttu-id="80aae-215">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="80aae-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="80aae-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="80aae-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="80aae-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-217">Boolean</span></span>|<span data-ttu-id="80aae-218">Gibt an, ob blockieren Fingerabdruck Entsperren für Arbeit Profil.</span><span class="sxs-lookup"><span data-stu-id="80aae-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="80aae-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="80aae-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="80aae-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-220">Boolean</span></span>|<span data-ttu-id="80aae-221">Gibt an, ob intelligente sperren und andere Trust-Agenten für Arbeit Profil zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="80aae-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="80aae-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="80aae-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="80aae-223">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-223">Int32</span></span>|<span data-ttu-id="80aae-224">Anzahl von Tagen vor der Arbeit Profilkennwort läuft ab.</span><span class="sxs-lookup"><span data-stu-id="80aae-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="80aae-225">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="80aae-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="80aae-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="80aae-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="80aae-227">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-227">Int32</span></span>|<span data-ttu-id="80aae-228">Minimale Länge der Arbeit Profilkennwort.</span><span class="sxs-lookup"><span data-stu-id="80aae-228">Minimum length of work profile password.</span></span> <span data-ttu-id="80aae-229">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="80aae-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="80aae-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="80aae-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="80aae-231">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-231">Int32</span></span>|<span data-ttu-id="80aae-232">Minimale Anzahl der numerische Zeichen in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80aae-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="80aae-233">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="80aae-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80aae-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="80aae-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="80aae-235">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-235">Int32</span></span>|<span data-ttu-id="80aae-236">Minimale Anzahl der nicht-Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80aae-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="80aae-237">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="80aae-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80aae-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="80aae-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="80aae-239">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-239">Int32</span></span>|<span data-ttu-id="80aae-240">Minimale Anzahl der Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80aae-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="80aae-241">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="80aae-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80aae-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="80aae-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="80aae-243">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-243">Int32</span></span>|<span data-ttu-id="80aae-244">Minimale Anzahl der Kleinbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80aae-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="80aae-245">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="80aae-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80aae-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="80aae-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="80aae-247">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-247">Int32</span></span>|<span data-ttu-id="80aae-248">Minimale Anzahl der Großbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80aae-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="80aae-249">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="80aae-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80aae-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="80aae-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="80aae-251">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-251">Int32</span></span>|<span data-ttu-id="80aae-252">Minimale Anzahl der Symbole in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80aae-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="80aae-253">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="80aae-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80aae-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="80aae-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="80aae-255">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-255">Int32</span></span>|<span data-ttu-id="80aae-256">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="80aae-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="80aae-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="80aae-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="80aae-258">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-258">Int32</span></span>|<span data-ttu-id="80aae-259">Anzahl der vorherigen Arbeit Profil Kennwörter zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="80aae-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="80aae-260">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="80aae-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="80aae-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="80aae-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="80aae-262">Int32</span><span class="sxs-lookup"><span data-stu-id="80aae-262">Int32</span></span>|<span data-ttu-id="80aae-263">Anzahl der Anmeldung Fehler zulässig sind, bevor Arbeit Profil entfernt wird und alle Daten gelöscht.</span><span class="sxs-lookup"><span data-stu-id="80aae-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="80aae-264">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="80aae-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="80aae-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="80aae-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="80aae-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80aae-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="80aae-267">Typ der Arbeit Profilkennwort, das erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="80aae-267">Type of work profile password that is required.</span></span> <span data-ttu-id="80aae-268">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="80aae-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="80aae-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="80aae-269">workProfileRequirePassword</span></span>|<span data-ttu-id="80aae-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-270">Boolean</span></span>|<span data-ttu-id="80aae-271">Kennwort erforderlich ist oder nicht für Arbeit Profil</span><span class="sxs-lookup"><span data-stu-id="80aae-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="80aae-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="80aae-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="80aae-273">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="80aae-273">Boolean</span></span>|<span data-ttu-id="80aae-274">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="80aae-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="80aae-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="80aae-275">Response</span></span>
<span data-ttu-id="80aae-276">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="80aae-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80aae-277">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80aae-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="80aae-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80aae-278">Request</span></span>
<span data-ttu-id="80aae-279">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80aae-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="80aae-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="80aae-280">Response</span></span>
<span data-ttu-id="80aae-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80aae-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



