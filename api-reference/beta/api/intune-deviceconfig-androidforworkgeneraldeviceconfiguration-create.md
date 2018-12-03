---
title: Erstellen von androidForWorkGeneralDeviceConfiguration
description: Erstellen eines neuen AndroidForWorkGeneralDeviceConfiguration-Objekts.
ms.openlocfilehash: e04f2071fff39e8030d38203d3c2fc8bb550ac48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064400"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="031cd-103">Erstellen von androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="031cd-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="031cd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="031cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="031cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="031cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="031cd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="031cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="031cd-107">Erstellen eines neuen [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="031cd-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="031cd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="031cd-108">Prerequisites</span></span>
<span data-ttu-id="031cd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="031cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="031cd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="031cd-111">Permission type</span></span>|<span data-ttu-id="031cd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="031cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="031cd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="031cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="031cd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031cd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="031cd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="031cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="031cd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="031cd-116">Not supported.</span></span>|
|<span data-ttu-id="031cd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="031cd-117">Application</span></span>|<span data-ttu-id="031cd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="031cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="031cd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="031cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="031cd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="031cd-120">Request headers</span></span>
|<span data-ttu-id="031cd-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="031cd-121">Header</span></span>|<span data-ttu-id="031cd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="031cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="031cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="031cd-123">Authorization</span></span>|<span data-ttu-id="031cd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="031cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="031cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="031cd-125">Accept</span></span>|<span data-ttu-id="031cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="031cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="031cd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="031cd-127">Request body</span></span>
<span data-ttu-id="031cd-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkGeneralDeviceConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="031cd-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="031cd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="031cd-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="031cd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="031cd-130">Property</span></span>|<span data-ttu-id="031cd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="031cd-131">Type</span></span>|<span data-ttu-id="031cd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="031cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="031cd-133">id</span><span class="sxs-lookup"><span data-stu-id="031cd-133">id</span></span>|<span data-ttu-id="031cd-134">String</span><span class="sxs-lookup"><span data-stu-id="031cd-134">String</span></span>|<span data-ttu-id="031cd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="031cd-135">Key of the entity.</span></span> <span data-ttu-id="031cd-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="031cd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="031cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="031cd-138">DateTimeOffset</span></span>|<span data-ttu-id="031cd-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="031cd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="031cd-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="031cd-141">roleScopeTagIds</span></span>|<span data-ttu-id="031cd-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="031cd-142">String collection</span></span>|<span data-ttu-id="031cd-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="031cd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="031cd-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="031cd-145">supportsScopeTags</span></span>|<span data-ttu-id="031cd-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-146">Boolean</span></span>|<span data-ttu-id="031cd-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="031cd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="031cd-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="031cd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="031cd-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="031cd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="031cd-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="031cd-150">This property is read-only.</span></span> <span data-ttu-id="031cd-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="031cd-152">createdDateTime</span></span>|<span data-ttu-id="031cd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="031cd-153">DateTimeOffset</span></span>|<span data-ttu-id="031cd-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="031cd-154">DateTime the object was created.</span></span> <span data-ttu-id="031cd-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-156">description</span><span class="sxs-lookup"><span data-stu-id="031cd-156">description</span></span>|<span data-ttu-id="031cd-157">String</span><span class="sxs-lookup"><span data-stu-id="031cd-157">String</span></span>|<span data-ttu-id="031cd-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="031cd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="031cd-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="031cd-160">displayName</span></span>|<span data-ttu-id="031cd-161">String</span><span class="sxs-lookup"><span data-stu-id="031cd-161">String</span></span>|<span data-ttu-id="031cd-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="031cd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="031cd-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-164">Version</span><span class="sxs-lookup"><span data-stu-id="031cd-164">version</span></span>|<span data-ttu-id="031cd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-165">Int32</span></span>|<span data-ttu-id="031cd-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="031cd-166">Version of the device configuration.</span></span> <span data-ttu-id="031cd-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="031cd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="031cd-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="031cd-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="031cd-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="031cd-169">Boolean</span></span>|<span data-ttu-id="031cd-170">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="031cd-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="031cd-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="031cd-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="031cd-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="031cd-172">Boolean</span></span>|<span data-ttu-id="031cd-173">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="031cd-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="031cd-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="031cd-174">passwordExpirationDays</span></span>|<span data-ttu-id="031cd-175">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-175">Int32</span></span>|<span data-ttu-id="031cd-176">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="031cd-176">Number of days before the password expires.</span></span> <span data-ttu-id="031cd-177">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="031cd-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="031cd-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="031cd-178">passwordMinimumLength</span></span>|<span data-ttu-id="031cd-179">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-179">Int32</span></span>|<span data-ttu-id="031cd-180">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="031cd-180">Minimum length of passwords.</span></span> <span data-ttu-id="031cd-181">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="031cd-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="031cd-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="031cd-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="031cd-183">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-183">Int32</span></span>|<span data-ttu-id="031cd-184">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="031cd-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="031cd-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="031cd-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="031cd-186">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-186">Int32</span></span>|<span data-ttu-id="031cd-187">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="031cd-187">Number of previous passwords to block.</span></span> <span data-ttu-id="031cd-188">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="031cd-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="031cd-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="031cd-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="031cd-190">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-190">Int32</span></span>|<span data-ttu-id="031cd-191">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="031cd-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="031cd-192">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="031cd-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="031cd-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="031cd-193">passwordRequiredType</span></span>|[<span data-ttu-id="031cd-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="031cd-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="031cd-195">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="031cd-195">Type of password that is required.</span></span> <span data-ttu-id="031cd-196">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="031cd-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="031cd-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="031cd-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="031cd-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="031cd-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="031cd-199">Typ der Daten, die Freigabe ist zulässig.</span><span class="sxs-lookup"><span data-stu-id="031cd-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="031cd-200">Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="031cd-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="031cd-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="031cd-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="031cd-202">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-202">Boolean</span></span>|<span data-ttu-id="031cd-203">Gibt an, ob beim Gerät gesperrt Benachrichtigungen zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="031cd-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="031cd-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="031cd-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="031cd-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-205">Boolean</span></span>|<span data-ttu-id="031cd-206">Blockieren Sie den Benutzer hinzufügen/entfernen von Konten im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="031cd-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="031cd-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="031cd-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="031cd-208">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-208">Boolean</span></span>|<span data-ttu-id="031cd-209">Können Sie Bluetooth-Geräte können Kontakte im Unternehmen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="031cd-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="031cd-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="031cd-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="031cd-211">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-211">Boolean</span></span>|<span data-ttu-id="031cd-212">Blockiert die Bildschirmaufnahme im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="031cd-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="031cd-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="031cd-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="031cd-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-214">Boolean</span></span>|<span data-ttu-id="031cd-215">Block Anzeige Arbeit Profil Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="031cd-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="031cd-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="031cd-216">workProfileBlockCamera</span></span>|<span data-ttu-id="031cd-217">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-217">Boolean</span></span>|<span data-ttu-id="031cd-218">Blockieren der Profil Kamera.</span><span class="sxs-lookup"><span data-stu-id="031cd-218">Block work profile camera.</span></span>|
|<span data-ttu-id="031cd-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="031cd-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="031cd-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-220">Boolean</span></span>|<span data-ttu-id="031cd-221">Verfügbarkeit der Block Arbeit Profil Kontakte im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="031cd-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="031cd-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="031cd-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="031cd-223">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-223">Boolean</span></span>|<span data-ttu-id="031cd-224">Boolescher Wert, der angibt, wenn die Einstellung firewallübergreifenden disallow Profil kopieren und einfügen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="031cd-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="031cd-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="031cd-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="031cd-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="031cd-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="031cd-227">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="031cd-227">Type of password that is required.</span></span> <span data-ttu-id="031cd-228">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="031cd-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="031cd-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="031cd-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="031cd-230">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-230">Boolean</span></span>|<span data-ttu-id="031cd-231">Gibt an, ob blockieren Fingerabdruck Entsperren für Arbeit Profil.</span><span class="sxs-lookup"><span data-stu-id="031cd-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="031cd-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="031cd-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="031cd-233">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-233">Boolean</span></span>|<span data-ttu-id="031cd-234">Gibt an, ob intelligente sperren und andere Trust-Agenten für Arbeit Profil zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="031cd-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="031cd-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="031cd-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="031cd-236">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-236">Int32</span></span>|<span data-ttu-id="031cd-237">Anzahl von Tagen vor der Arbeit Profilkennwort läuft ab.</span><span class="sxs-lookup"><span data-stu-id="031cd-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="031cd-238">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="031cd-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="031cd-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="031cd-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="031cd-240">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-240">Int32</span></span>|<span data-ttu-id="031cd-241">Minimale Länge der Arbeit Profilkennwort.</span><span class="sxs-lookup"><span data-stu-id="031cd-241">Minimum length of work profile password.</span></span> <span data-ttu-id="031cd-242">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="031cd-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="031cd-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="031cd-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="031cd-244">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-244">Int32</span></span>|<span data-ttu-id="031cd-245">Minimale Anzahl der numerische Zeichen in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="031cd-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="031cd-246">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="031cd-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="031cd-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="031cd-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="031cd-248">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-248">Int32</span></span>|<span data-ttu-id="031cd-249">Minimale Anzahl der nicht-Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="031cd-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="031cd-250">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="031cd-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="031cd-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="031cd-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="031cd-252">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-252">Int32</span></span>|<span data-ttu-id="031cd-253">Minimale Anzahl der Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="031cd-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="031cd-254">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="031cd-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="031cd-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="031cd-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="031cd-256">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-256">Int32</span></span>|<span data-ttu-id="031cd-257">Minimale Anzahl der Kleinbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="031cd-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="031cd-258">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="031cd-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="031cd-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="031cd-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="031cd-260">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-260">Int32</span></span>|<span data-ttu-id="031cd-261">Minimale Anzahl der Großbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="031cd-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="031cd-262">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="031cd-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="031cd-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="031cd-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="031cd-264">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-264">Int32</span></span>|<span data-ttu-id="031cd-265">Minimale Anzahl der Symbole in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="031cd-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="031cd-266">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="031cd-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="031cd-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="031cd-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="031cd-268">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-268">Int32</span></span>|<span data-ttu-id="031cd-269">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="031cd-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="031cd-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="031cd-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="031cd-271">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-271">Int32</span></span>|<span data-ttu-id="031cd-272">Anzahl der vorherigen Arbeit Profil Kennwörter zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="031cd-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="031cd-273">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="031cd-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="031cd-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="031cd-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="031cd-275">Int32</span><span class="sxs-lookup"><span data-stu-id="031cd-275">Int32</span></span>|<span data-ttu-id="031cd-276">Anzahl der Anmeldung Fehler zulässig sind, bevor Arbeit Profil entfernt wird und alle Daten gelöscht.</span><span class="sxs-lookup"><span data-stu-id="031cd-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="031cd-277">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="031cd-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="031cd-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="031cd-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="031cd-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="031cd-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="031cd-280">Typ der Arbeit Profilkennwort, das erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="031cd-280">Type of work profile password that is required.</span></span> <span data-ttu-id="031cd-281">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="031cd-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="031cd-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="031cd-282">workProfileRequirePassword</span></span>|<span data-ttu-id="031cd-283">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-283">Boolean</span></span>|<span data-ttu-id="031cd-284">Kennwort erforderlich ist oder nicht für Arbeit Profil</span><span class="sxs-lookup"><span data-stu-id="031cd-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="031cd-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="031cd-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="031cd-286">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="031cd-286">Boolean</span></span>|<span data-ttu-id="031cd-287">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="031cd-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="031cd-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="031cd-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="031cd-289">String</span><span class="sxs-lookup"><span data-stu-id="031cd-289">String</span></span>|<span data-ttu-id="031cd-290">Aktivieren Sie Sperrmodus für immer auf VPN.</span><span class="sxs-lookup"><span data-stu-id="031cd-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="031cd-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="031cd-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="031cd-292">Boolesch</span><span class="sxs-lookup"><span data-stu-id="031cd-292">Boolean</span></span>|<span data-ttu-id="031cd-293">Aktivieren Sie Sperrmodus für immer auf VPN.</span><span class="sxs-lookup"><span data-stu-id="031cd-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="031cd-294">Antwort</span><span class="sxs-lookup"><span data-stu-id="031cd-294">Response</span></span>
<span data-ttu-id="031cd-295">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="031cd-295">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="031cd-296">Beispiel</span><span class="sxs-lookup"><span data-stu-id="031cd-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="031cd-297">Anforderung</span><span class="sxs-lookup"><span data-stu-id="031cd-297">Request</span></span>
<span data-ttu-id="031cd-298">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="031cd-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2102

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="031cd-299">Antwort</span><span class="sxs-lookup"><span data-stu-id="031cd-299">Response</span></span>
<span data-ttu-id="031cd-p129">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="031cd-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2210

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```





