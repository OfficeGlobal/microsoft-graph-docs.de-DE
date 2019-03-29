---
title: AndroidWorkProfileGeneralDeviceConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7568bd59aa728391779dda6ee24a5e15d5c165ea
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971024"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="7a24b-103">AndroidWorkProfileGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7a24b-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="7a24b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7a24b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a24b-105">Aktualisieren der Eigenschaften eines [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a24b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a24b-106">Prerequisites</span></span>
<span data-ttu-id="7a24b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a24b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a24b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a24b-109">Permission type</span></span>|<span data-ttu-id="7a24b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a24b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a24b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a24b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a24b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a24b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a24b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a24b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a24b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a24b-114">Not supported.</span></span>|
|<span data-ttu-id="7a24b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a24b-115">Application</span></span>|<span data-ttu-id="7a24b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a24b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a24b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a24b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7a24b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a24b-118">Request headers</span></span>
|<span data-ttu-id="7a24b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a24b-119">Header</span></span>|<span data-ttu-id="7a24b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a24b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a24b-121">Authorization</span></span>|<span data-ttu-id="7a24b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a24b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a24b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a24b-123">Accept</span></span>|<span data-ttu-id="7a24b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a24b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a24b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a24b-125">Request body</span></span>
<span data-ttu-id="7a24b-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7a24b-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="7a24b-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="7a24b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a24b-128">Property</span></span>|<span data-ttu-id="7a24b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7a24b-129">Type</span></span>|<span data-ttu-id="7a24b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a24b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a24b-131">id</span><span class="sxs-lookup"><span data-stu-id="7a24b-131">id</span></span>|<span data-ttu-id="7a24b-132">String</span><span class="sxs-lookup"><span data-stu-id="7a24b-132">String</span></span>|<span data-ttu-id="7a24b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7a24b-133">Key of the entity.</span></span> <span data-ttu-id="7a24b-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a24b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a24b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a24b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7a24b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a24b-136">DateTimeOffset</span></span>|<span data-ttu-id="7a24b-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7a24b-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a24b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a24b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a24b-139">createdDateTime</span></span>|<span data-ttu-id="7a24b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a24b-140">DateTimeOffset</span></span>|<span data-ttu-id="7a24b-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-141">DateTime the object was created.</span></span> <span data-ttu-id="7a24b-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a24b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a24b-143">description</span><span class="sxs-lookup"><span data-stu-id="7a24b-143">description</span></span>|<span data-ttu-id="7a24b-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a24b-144">String</span></span>|<span data-ttu-id="7a24b-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7a24b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7a24b-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a24b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a24b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7a24b-147">displayName</span></span>|<span data-ttu-id="7a24b-148">String</span><span class="sxs-lookup"><span data-stu-id="7a24b-148">String</span></span>|<span data-ttu-id="7a24b-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7a24b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7a24b-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a24b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a24b-151">Version</span><span class="sxs-lookup"><span data-stu-id="7a24b-151">version</span></span>|<span data-ttu-id="7a24b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-152">Int32</span></span>|<span data-ttu-id="7a24b-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7a24b-153">Version of the device configuration.</span></span> <span data-ttu-id="7a24b-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a24b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a24b-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="7a24b-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="7a24b-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-156">Boolean</span></span>|<span data-ttu-id="7a24b-157">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="7a24b-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="7a24b-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="7a24b-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="7a24b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a24b-159">Boolean</span></span>|<span data-ttu-id="7a24b-160">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7a24b-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="7a24b-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7a24b-161">passwordExpirationDays</span></span>|<span data-ttu-id="7a24b-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-162">Int32</span></span>|<span data-ttu-id="7a24b-163">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-163">Number of days before the password expires.</span></span> <span data-ttu-id="7a24b-164">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="7a24b-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7a24b-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7a24b-165">passwordMinimumLength</span></span>|<span data-ttu-id="7a24b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-166">Int32</span></span>|<span data-ttu-id="7a24b-167">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="7a24b-167">Minimum length of passwords.</span></span> <span data-ttu-id="7a24b-168">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="7a24b-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7a24b-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7a24b-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7a24b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-170">Int32</span></span>|<span data-ttu-id="7a24b-171">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="7a24b-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7a24b-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7a24b-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7a24b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-173">Int32</span></span>|<span data-ttu-id="7a24b-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="7a24b-174">Number of previous passwords to block.</span></span> <span data-ttu-id="7a24b-175">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="7a24b-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7a24b-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7a24b-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7a24b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-177">Int32</span></span>|<span data-ttu-id="7a24b-178">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="7a24b-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="7a24b-179">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="7a24b-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7a24b-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7a24b-180">passwordRequiredType</span></span>|[<span data-ttu-id="7a24b-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7a24b-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="7a24b-182">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="7a24b-182">Type of password that is required.</span></span> <span data-ttu-id="7a24b-183">Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="7a24b-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="7a24b-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="7a24b-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="7a24b-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="7a24b-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="7a24b-186">Typ der zulässigen Datenfreigabe.</span><span class="sxs-lookup"><span data-stu-id="7a24b-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="7a24b-187">Mögliche Werte sind: `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="7a24b-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="7a24b-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="7a24b-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="7a24b-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-189">Boolean</span></span>|<span data-ttu-id="7a24b-190">Gibt an, ob Benachrichtigungen blockiert werden sollen, während das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="7a24b-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="7a24b-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="7a24b-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="7a24b-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-192">Boolean</span></span>|<span data-ttu-id="7a24b-193">Verhindern, dass Benutzerkonten im Arbeitsprofil hinzufügen/entfernen.</span><span class="sxs-lookup"><span data-stu-id="7a24b-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="7a24b-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="7a24b-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="7a24b-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-195">Boolean</span></span>|<span data-ttu-id="7a24b-196">Bluetooth-Geräte können auf Enterprise-Kontakte zugreifen.</span><span class="sxs-lookup"><span data-stu-id="7a24b-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="7a24b-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="7a24b-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="7a24b-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-198">Boolean</span></span>|<span data-ttu-id="7a24b-199">Blockieren der Bildschirmaufzeichnung im Arbeitsprofil.</span><span class="sxs-lookup"><span data-stu-id="7a24b-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="7a24b-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="7a24b-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="7a24b-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-201">Boolean</span></span>|<span data-ttu-id="7a24b-202">Blockieren der Anzeige von Arbeitsprofil-Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="7a24b-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="7a24b-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="7a24b-203">workProfileBlockCamera</span></span>|<span data-ttu-id="7a24b-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-204">Boolean</span></span>|<span data-ttu-id="7a24b-205">Arbeitsprofil Kamera blockieren.</span><span class="sxs-lookup"><span data-stu-id="7a24b-205">Block work profile camera.</span></span>|
|<span data-ttu-id="7a24b-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="7a24b-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="7a24b-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-207">Boolean</span></span>|<span data-ttu-id="7a24b-208">Blockieren der Verfügbarkeit von Arbeitsprofil Kontakten im persönlichen Profil</span><span class="sxs-lookup"><span data-stu-id="7a24b-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="7a24b-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="7a24b-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="7a24b-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-210">Boolean</span></span>|<span data-ttu-id="7a24b-211">Boolescher Wert, der angibt, ob die Einstellung Cross profile Copy/Paste nicht zulassen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="7a24b-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="7a24b-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="7a24b-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="7a24b-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="7a24b-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="7a24b-214">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="7a24b-214">Type of password that is required.</span></span> <span data-ttu-id="7a24b-215">Mögliche Werte sind: `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="7a24b-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="7a24b-216">Eigenschaften workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="7a24b-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="7a24b-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-217">Boolean</span></span>|<span data-ttu-id="7a24b-218">Gibt an, ob die Fingerabdruck Sperre für das Arbeitsprofil blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="7a24b-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="7a24b-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="7a24b-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="7a24b-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-220">Boolean</span></span>|<span data-ttu-id="7a24b-221">Gibt an, ob die Smart Lock-und andere Trust-Agents für das Arbeitsprofil blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7a24b-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="7a24b-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7a24b-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="7a24b-223">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-223">Int32</span></span>|<span data-ttu-id="7a24b-224">Anzahl der Tage vor Ablauf des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="7a24b-225">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="7a24b-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7a24b-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7a24b-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="7a24b-227">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-227">Int32</span></span>|<span data-ttu-id="7a24b-228">Minimale Länge des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-228">Minimum length of work profile password.</span></span> <span data-ttu-id="7a24b-229">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="7a24b-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7a24b-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="7a24b-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="7a24b-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-231">Int32</span></span>|<span data-ttu-id="7a24b-232">Minimale Anzahl von numerischen Zeichen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="7a24b-233">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="7a24b-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="7a24b-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="7a24b-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="7a24b-235">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-235">Int32</span></span>|<span data-ttu-id="7a24b-236">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="7a24b-237">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="7a24b-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="7a24b-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="7a24b-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="7a24b-239">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-239">Int32</span></span>|<span data-ttu-id="7a24b-240">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="7a24b-241">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="7a24b-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="7a24b-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="7a24b-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="7a24b-243">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-243">Int32</span></span>|<span data-ttu-id="7a24b-244">Minimale Anzahl von Kleinbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="7a24b-245">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="7a24b-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="7a24b-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="7a24b-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="7a24b-247">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-247">Int32</span></span>|<span data-ttu-id="7a24b-248">Minimale Anzahl von Großbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="7a24b-249">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="7a24b-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="7a24b-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="7a24b-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="7a24b-251">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-251">Int32</span></span>|<span data-ttu-id="7a24b-252">Minimale Anzahl von Symbolen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a24b-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="7a24b-253">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="7a24b-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="7a24b-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7a24b-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7a24b-255">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-255">Int32</span></span>|<span data-ttu-id="7a24b-256">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="7a24b-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7a24b-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7a24b-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7a24b-258">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-258">Int32</span></span>|<span data-ttu-id="7a24b-259">Anzahl der vorherigen Arbeitsprofil Kennwörter, die blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7a24b-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="7a24b-260">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="7a24b-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7a24b-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7a24b-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7a24b-262">Int32</span><span class="sxs-lookup"><span data-stu-id="7a24b-262">Int32</span></span>|<span data-ttu-id="7a24b-263">Anzahl der zulässigen Anmeldefehler vor dem Entfernen des Arbeitsprofils und aller gelöschten Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="7a24b-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="7a24b-264">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="7a24b-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7a24b-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7a24b-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="7a24b-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7a24b-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="7a24b-267">Typ des erforderlichen Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7a24b-267">Type of work profile password that is required.</span></span> <span data-ttu-id="7a24b-268">Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="7a24b-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="7a24b-269">Workprofilerequirepassword wurden</span><span class="sxs-lookup"><span data-stu-id="7a24b-269">workProfileRequirePassword</span></span>|<span data-ttu-id="7a24b-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a24b-270">Boolean</span></span>|<span data-ttu-id="7a24b-271">Kennwort ist erforderlich oder nicht für das Arbeitsprofil</span><span class="sxs-lookup"><span data-stu-id="7a24b-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="7a24b-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7a24b-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="7a24b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a24b-273">Boolean</span></span>|<span data-ttu-id="7a24b-274">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="7a24b-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="7a24b-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a24b-275">Response</span></span>
<span data-ttu-id="7a24b-276">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7a24b-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a24b-277">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a24b-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a24b-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a24b-278">Request</span></span>
<span data-ttu-id="7a24b-279">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a24b-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7a24b-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a24b-280">Response</span></span>
<span data-ttu-id="7a24b-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a24b-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



