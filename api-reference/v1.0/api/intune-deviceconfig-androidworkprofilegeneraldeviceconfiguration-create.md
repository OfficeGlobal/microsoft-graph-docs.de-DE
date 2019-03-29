---
title: AndroidWorkProfileGeneralDeviceConfiguration erstellen
description: Erstellen eines neuen androidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0e1ae2e8eed358054163295dc8608a1bbaba68f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960202"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="57781-103">AndroidWorkProfileGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="57781-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="57781-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="57781-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57781-105">Erstellen eines neuen [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="57781-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57781-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57781-106">Prerequisites</span></span>
<span data-ttu-id="57781-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57781-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57781-109">Permission type</span></span>|<span data-ttu-id="57781-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57781-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57781-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57781-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57781-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57781-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57781-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57781-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57781-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57781-114">Not supported.</span></span>|
|<span data-ttu-id="57781-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57781-115">Application</span></span>|<span data-ttu-id="57781-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57781-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57781-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57781-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="57781-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57781-118">Request headers</span></span>
|<span data-ttu-id="57781-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="57781-119">Header</span></span>|<span data-ttu-id="57781-120">Wert</span><span class="sxs-lookup"><span data-stu-id="57781-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57781-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="57781-121">Authorization</span></span>|<span data-ttu-id="57781-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57781-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57781-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="57781-123">Accept</span></span>|<span data-ttu-id="57781-124">application/json</span><span class="sxs-lookup"><span data-stu-id="57781-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57781-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57781-125">Request body</span></span>
<span data-ttu-id="57781-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidWorkProfileGeneralDeviceConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="57781-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="57781-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidWorkProfileGeneralDeviceConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="57781-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57781-128">Property</span></span>|<span data-ttu-id="57781-129">Typ</span><span class="sxs-lookup"><span data-stu-id="57781-129">Type</span></span>|<span data-ttu-id="57781-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57781-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57781-131">id</span><span class="sxs-lookup"><span data-stu-id="57781-131">id</span></span>|<span data-ttu-id="57781-132">String</span><span class="sxs-lookup"><span data-stu-id="57781-132">String</span></span>|<span data-ttu-id="57781-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="57781-133">Key of the entity.</span></span> <span data-ttu-id="57781-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57781-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57781-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57781-135">lastModifiedDateTime</span></span>|<span data-ttu-id="57781-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57781-136">DateTimeOffset</span></span>|<span data-ttu-id="57781-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="57781-137">DateTime the object was last modified.</span></span> <span data-ttu-id="57781-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57781-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57781-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57781-139">createdDateTime</span></span>|<span data-ttu-id="57781-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57781-140">DateTimeOffset</span></span>|<span data-ttu-id="57781-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="57781-141">DateTime the object was created.</span></span> <span data-ttu-id="57781-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57781-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57781-143">description</span><span class="sxs-lookup"><span data-stu-id="57781-143">description</span></span>|<span data-ttu-id="57781-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57781-144">String</span></span>|<span data-ttu-id="57781-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="57781-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57781-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57781-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57781-147">displayName</span><span class="sxs-lookup"><span data-stu-id="57781-147">displayName</span></span>|<span data-ttu-id="57781-148">String</span><span class="sxs-lookup"><span data-stu-id="57781-148">String</span></span>|<span data-ttu-id="57781-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="57781-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57781-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57781-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57781-151">Version</span><span class="sxs-lookup"><span data-stu-id="57781-151">version</span></span>|<span data-ttu-id="57781-152">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-152">Int32</span></span>|<span data-ttu-id="57781-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="57781-153">Version of the device configuration.</span></span> <span data-ttu-id="57781-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57781-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57781-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="57781-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="57781-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-156">Boolean</span></span>|<span data-ttu-id="57781-157">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="57781-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="57781-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="57781-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="57781-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="57781-159">Boolean</span></span>|<span data-ttu-id="57781-160">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="57781-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="57781-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="57781-161">passwordExpirationDays</span></span>|<span data-ttu-id="57781-162">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-162">Int32</span></span>|<span data-ttu-id="57781-163">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57781-163">Number of days before the password expires.</span></span> <span data-ttu-id="57781-164">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="57781-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="57781-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57781-165">passwordMinimumLength</span></span>|<span data-ttu-id="57781-166">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-166">Int32</span></span>|<span data-ttu-id="57781-167">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="57781-167">Minimum length of passwords.</span></span> <span data-ttu-id="57781-168">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="57781-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="57781-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="57781-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="57781-170">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-170">Int32</span></span>|<span data-ttu-id="57781-171">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="57781-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="57781-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="57781-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="57781-173">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-173">Int32</span></span>|<span data-ttu-id="57781-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="57781-174">Number of previous passwords to block.</span></span> <span data-ttu-id="57781-175">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="57781-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="57781-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="57781-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="57781-177">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-177">Int32</span></span>|<span data-ttu-id="57781-178">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="57781-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="57781-179">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="57781-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="57781-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="57781-180">passwordRequiredType</span></span>|[<span data-ttu-id="57781-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="57781-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="57781-182">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="57781-182">Type of password that is required.</span></span> <span data-ttu-id="57781-183">Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="57781-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="57781-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="57781-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="57781-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="57781-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="57781-186">Typ der zulässigen Datenfreigabe.</span><span class="sxs-lookup"><span data-stu-id="57781-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="57781-187">Mögliche Werte sind: `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="57781-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="57781-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="57781-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="57781-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-189">Boolean</span></span>|<span data-ttu-id="57781-190">Gibt an, ob Benachrichtigungen blockiert werden sollen, während das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="57781-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="57781-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="57781-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="57781-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-192">Boolean</span></span>|<span data-ttu-id="57781-193">Verhindern, dass Benutzerkonten im Arbeitsprofil hinzufügen/entfernen.</span><span class="sxs-lookup"><span data-stu-id="57781-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="57781-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="57781-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="57781-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-195">Boolean</span></span>|<span data-ttu-id="57781-196">Bluetooth-Geräte können auf Enterprise-Kontakte zugreifen.</span><span class="sxs-lookup"><span data-stu-id="57781-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="57781-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="57781-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="57781-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-198">Boolean</span></span>|<span data-ttu-id="57781-199">Blockieren der Bildschirmaufzeichnung im Arbeitsprofil.</span><span class="sxs-lookup"><span data-stu-id="57781-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="57781-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="57781-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="57781-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-201">Boolean</span></span>|<span data-ttu-id="57781-202">Blockieren der Anzeige von Arbeitsprofil-Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="57781-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="57781-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="57781-203">workProfileBlockCamera</span></span>|<span data-ttu-id="57781-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-204">Boolean</span></span>|<span data-ttu-id="57781-205">Arbeitsprofil Kamera blockieren.</span><span class="sxs-lookup"><span data-stu-id="57781-205">Block work profile camera.</span></span>|
|<span data-ttu-id="57781-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="57781-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="57781-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-207">Boolean</span></span>|<span data-ttu-id="57781-208">Blockieren der Verfügbarkeit von Arbeitsprofil Kontakten im persönlichen Profil</span><span class="sxs-lookup"><span data-stu-id="57781-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="57781-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="57781-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="57781-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-210">Boolean</span></span>|<span data-ttu-id="57781-211">Boolescher Wert, der angibt, ob die Einstellung Cross profile Copy/Paste nicht zulassen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="57781-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="57781-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="57781-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="57781-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="57781-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="57781-214">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="57781-214">Type of password that is required.</span></span> <span data-ttu-id="57781-215">Mögliche Werte sind: `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="57781-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="57781-216">Eigenschaften workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="57781-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="57781-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-217">Boolean</span></span>|<span data-ttu-id="57781-218">Gibt an, ob die Fingerabdruck Sperre für das Arbeitsprofil blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="57781-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="57781-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="57781-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="57781-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-220">Boolean</span></span>|<span data-ttu-id="57781-221">Gibt an, ob die Smart Lock-und andere Trust-Agents für das Arbeitsprofil blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="57781-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="57781-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="57781-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="57781-223">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-223">Int32</span></span>|<span data-ttu-id="57781-224">Anzahl der Tage vor Ablauf des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57781-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="57781-225">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="57781-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="57781-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57781-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="57781-227">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-227">Int32</span></span>|<span data-ttu-id="57781-228">Minimale Länge des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57781-228">Minimum length of work profile password.</span></span> <span data-ttu-id="57781-229">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="57781-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="57781-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="57781-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="57781-231">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-231">Int32</span></span>|<span data-ttu-id="57781-232">Minimale Anzahl von numerischen Zeichen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="57781-233">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="57781-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="57781-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="57781-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="57781-235">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-235">Int32</span></span>|<span data-ttu-id="57781-236">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="57781-237">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="57781-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="57781-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="57781-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="57781-239">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-239">Int32</span></span>|<span data-ttu-id="57781-240">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="57781-241">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="57781-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="57781-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="57781-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="57781-243">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-243">Int32</span></span>|<span data-ttu-id="57781-244">Minimale Anzahl von Kleinbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="57781-245">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="57781-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="57781-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="57781-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="57781-247">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-247">Int32</span></span>|<span data-ttu-id="57781-248">Minimale Anzahl von Großbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="57781-249">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="57781-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="57781-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="57781-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="57781-251">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-251">Int32</span></span>|<span data-ttu-id="57781-252">Minimale Anzahl von Symbolen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57781-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="57781-253">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="57781-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="57781-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="57781-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="57781-255">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-255">Int32</span></span>|<span data-ttu-id="57781-256">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="57781-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="57781-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="57781-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="57781-258">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-258">Int32</span></span>|<span data-ttu-id="57781-259">Anzahl der vorherigen Arbeitsprofil Kennwörter, die blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="57781-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="57781-260">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="57781-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="57781-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="57781-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="57781-262">Int32</span><span class="sxs-lookup"><span data-stu-id="57781-262">Int32</span></span>|<span data-ttu-id="57781-263">Anzahl der zulässigen Anmeldefehler vor dem Entfernen des Arbeitsprofils und aller gelöschten Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="57781-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="57781-264">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="57781-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="57781-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="57781-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="57781-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="57781-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="57781-267">Typ des erforderlichen Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57781-267">Type of work profile password that is required.</span></span> <span data-ttu-id="57781-268">Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="57781-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="57781-269">Workprofilerequirepassword wurden</span><span class="sxs-lookup"><span data-stu-id="57781-269">workProfileRequirePassword</span></span>|<span data-ttu-id="57781-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57781-270">Boolean</span></span>|<span data-ttu-id="57781-271">Kennwort ist erforderlich oder nicht für das Arbeitsprofil</span><span class="sxs-lookup"><span data-stu-id="57781-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="57781-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="57781-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="57781-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="57781-273">Boolean</span></span>|<span data-ttu-id="57781-274">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57781-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="57781-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="57781-275">Response</span></span>
<span data-ttu-id="57781-276">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="57781-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57781-277">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57781-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="57781-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57781-278">Request</span></span>
<span data-ttu-id="57781-279">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57781-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="57781-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="57781-280">Response</span></span>
<span data-ttu-id="57781-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57781-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



