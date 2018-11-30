---
title: Erstellen von androidWorkProfileGeneralDeviceConfiguration
description: Erstellen eines neuen AndroidWorkProfileGeneralDeviceConfiguration-Objekts.
ms.openlocfilehash: 50437bb84a1c4d0c4aa31785511128abf15eaa13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062005"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="16c5b-103">Erstellen von androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="16c5b-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="16c5b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16c5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16c5b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16c5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16c5b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16c5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16c5b-107">Erstellen eines neuen [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="16c5b-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16c5b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16c5b-108">Prerequisites</span></span>
<span data-ttu-id="16c5b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16c5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16c5b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16c5b-111">Permission type</span></span>|<span data-ttu-id="16c5b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16c5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16c5b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16c5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16c5b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16c5b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16c5b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16c5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16c5b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16c5b-116">Not supported.</span></span>|
|<span data-ttu-id="16c5b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16c5b-117">Application</span></span>|<span data-ttu-id="16c5b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16c5b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16c5b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16c5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="16c5b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16c5b-120">Request headers</span></span>
|<span data-ttu-id="16c5b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="16c5b-121">Header</span></span>|<span data-ttu-id="16c5b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="16c5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16c5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16c5b-123">Authorization</span></span>|<span data-ttu-id="16c5b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16c5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16c5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16c5b-125">Accept</span></span>|<span data-ttu-id="16c5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16c5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16c5b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16c5b-127">Request body</span></span>
<span data-ttu-id="16c5b-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileGeneralDeviceConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="16c5b-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="16c5b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="16c5b-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="16c5b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16c5b-130">Property</span></span>|<span data-ttu-id="16c5b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="16c5b-131">Type</span></span>|<span data-ttu-id="16c5b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16c5b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16c5b-133">id</span><span class="sxs-lookup"><span data-stu-id="16c5b-133">id</span></span>|<span data-ttu-id="16c5b-134">String</span><span class="sxs-lookup"><span data-stu-id="16c5b-134">String</span></span>|<span data-ttu-id="16c5b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="16c5b-135">Key of the entity.</span></span> <span data-ttu-id="16c5b-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16c5b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="16c5b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16c5b-138">DateTimeOffset</span></span>|<span data-ttu-id="16c5b-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="16c5b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="16c5b-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16c5b-141">roleScopeTagIds</span></span>|<span data-ttu-id="16c5b-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="16c5b-142">String collection</span></span>|<span data-ttu-id="16c5b-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="16c5b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16c5b-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="16c5b-145">supportsScopeTags</span></span>|<span data-ttu-id="16c5b-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-146">Boolean</span></span>|<span data-ttu-id="16c5b-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16c5b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16c5b-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="16c5b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16c5b-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="16c5b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16c5b-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16c5b-150">This property is read-only.</span></span> <span data-ttu-id="16c5b-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16c5b-152">createdDateTime</span></span>|<span data-ttu-id="16c5b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16c5b-153">DateTimeOffset</span></span>|<span data-ttu-id="16c5b-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="16c5b-154">DateTime the object was created.</span></span> <span data-ttu-id="16c5b-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-156">description</span><span class="sxs-lookup"><span data-stu-id="16c5b-156">description</span></span>|<span data-ttu-id="16c5b-157">String</span><span class="sxs-lookup"><span data-stu-id="16c5b-157">String</span></span>|<span data-ttu-id="16c5b-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="16c5b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16c5b-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="16c5b-160">displayName</span></span>|<span data-ttu-id="16c5b-161">String</span><span class="sxs-lookup"><span data-stu-id="16c5b-161">String</span></span>|<span data-ttu-id="16c5b-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="16c5b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16c5b-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-164">Version</span><span class="sxs-lookup"><span data-stu-id="16c5b-164">version</span></span>|<span data-ttu-id="16c5b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-165">Int32</span></span>|<span data-ttu-id="16c5b-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="16c5b-166">Version of the device configuration.</span></span> <span data-ttu-id="16c5b-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c5b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16c5b-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="16c5b-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="16c5b-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="16c5b-169">Boolean</span></span>|<span data-ttu-id="16c5b-170">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="16c5b-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="16c5b-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="16c5b-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="16c5b-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="16c5b-172">Boolean</span></span>|<span data-ttu-id="16c5b-173">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="16c5b-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="16c5b-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="16c5b-174">passwordExpirationDays</span></span>|<span data-ttu-id="16c5b-175">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-175">Int32</span></span>|<span data-ttu-id="16c5b-176">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="16c5b-176">Number of days before the password expires.</span></span> <span data-ttu-id="16c5b-177">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="16c5b-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="16c5b-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="16c5b-178">passwordMinimumLength</span></span>|<span data-ttu-id="16c5b-179">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-179">Int32</span></span>|<span data-ttu-id="16c5b-180">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="16c5b-180">Minimum length of passwords.</span></span> <span data-ttu-id="16c5b-181">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="16c5b-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="16c5b-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="16c5b-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="16c5b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-183">Int32</span></span>|<span data-ttu-id="16c5b-184">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="16c5b-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="16c5b-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="16c5b-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="16c5b-186">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-186">Int32</span></span>|<span data-ttu-id="16c5b-187">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="16c5b-187">Number of previous passwords to block.</span></span> <span data-ttu-id="16c5b-188">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="16c5b-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="16c5b-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="16c5b-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="16c5b-190">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-190">Int32</span></span>|<span data-ttu-id="16c5b-191">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="16c5b-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="16c5b-192">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="16c5b-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="16c5b-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="16c5b-193">passwordRequiredType</span></span>|[<span data-ttu-id="16c5b-194">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="16c5b-194">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="16c5b-195">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="16c5b-195">Type of password that is required.</span></span> <span data-ttu-id="16c5b-196">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="16c5b-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="16c5b-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="16c5b-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="16c5b-198">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="16c5b-198">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="16c5b-199">Typ der Daten, die Freigabe ist zulässig.</span><span class="sxs-lookup"><span data-stu-id="16c5b-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="16c5b-200">Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="16c5b-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="16c5b-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="16c5b-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="16c5b-202">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-202">Boolean</span></span>|<span data-ttu-id="16c5b-203">Gibt an, ob beim Gerät gesperrt Benachrichtigungen zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="16c5b-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="16c5b-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="16c5b-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="16c5b-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-205">Boolean</span></span>|<span data-ttu-id="16c5b-206">Blockieren Sie den Benutzer hinzufügen/entfernen von Konten im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="16c5b-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="16c5b-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="16c5b-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="16c5b-208">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-208">Boolean</span></span>|<span data-ttu-id="16c5b-209">Können Sie Bluetooth-Geräte können Kontakte im Unternehmen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="16c5b-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="16c5b-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="16c5b-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="16c5b-211">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-211">Boolean</span></span>|<span data-ttu-id="16c5b-212">Blockiert die Bildschirmaufnahme im Profil Arbeit.</span><span class="sxs-lookup"><span data-stu-id="16c5b-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="16c5b-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="16c5b-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="16c5b-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-214">Boolean</span></span>|<span data-ttu-id="16c5b-215">Block Anzeige Arbeit Profil Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="16c5b-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="16c5b-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="16c5b-216">workProfileBlockCamera</span></span>|<span data-ttu-id="16c5b-217">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-217">Boolean</span></span>|<span data-ttu-id="16c5b-218">Blockieren der Profil Kamera.</span><span class="sxs-lookup"><span data-stu-id="16c5b-218">Block work profile camera.</span></span>|
|<span data-ttu-id="16c5b-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="16c5b-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="16c5b-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-220">Boolean</span></span>|<span data-ttu-id="16c5b-221">Verfügbarkeit der Block Arbeit Profil Kontakte im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="16c5b-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="16c5b-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="16c5b-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="16c5b-223">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-223">Boolean</span></span>|<span data-ttu-id="16c5b-224">Boolescher Wert, der angibt, wenn die Einstellung firewallübergreifenden disallow Profil kopieren und einfügen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="16c5b-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="16c5b-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="16c5b-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="16c5b-226">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="16c5b-226">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="16c5b-227">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="16c5b-227">Type of password that is required.</span></span> <span data-ttu-id="16c5b-228">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="16c5b-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="16c5b-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="16c5b-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="16c5b-230">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-230">Boolean</span></span>|<span data-ttu-id="16c5b-231">Gibt an, ob blockieren Fingerabdruck Entsperren für Arbeit Profil.</span><span class="sxs-lookup"><span data-stu-id="16c5b-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="16c5b-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="16c5b-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="16c5b-233">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-233">Boolean</span></span>|<span data-ttu-id="16c5b-234">Gibt an, ob intelligente sperren und andere Trust-Agenten für Arbeit Profil zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="16c5b-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="16c5b-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="16c5b-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="16c5b-236">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-236">Int32</span></span>|<span data-ttu-id="16c5b-237">Anzahl von Tagen vor der Arbeit Profilkennwort läuft ab.</span><span class="sxs-lookup"><span data-stu-id="16c5b-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="16c5b-238">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="16c5b-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="16c5b-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="16c5b-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="16c5b-240">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-240">Int32</span></span>|<span data-ttu-id="16c5b-241">Minimale Länge der Arbeit Profilkennwort.</span><span class="sxs-lookup"><span data-stu-id="16c5b-241">Minimum length of work profile password.</span></span> <span data-ttu-id="16c5b-242">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="16c5b-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="16c5b-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="16c5b-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="16c5b-244">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-244">Int32</span></span>|<span data-ttu-id="16c5b-245">Minimale Anzahl der numerische Zeichen in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c5b-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="16c5b-246">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="16c5b-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="16c5b-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="16c5b-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="16c5b-248">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-248">Int32</span></span>|<span data-ttu-id="16c5b-249">Minimale Anzahl der nicht-Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c5b-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="16c5b-250">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="16c5b-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="16c5b-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="16c5b-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="16c5b-252">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-252">Int32</span></span>|<span data-ttu-id="16c5b-253">Minimale Anzahl der Buchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c5b-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="16c5b-254">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="16c5b-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="16c5b-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="16c5b-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="16c5b-256">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-256">Int32</span></span>|<span data-ttu-id="16c5b-257">Minimale Anzahl der Kleinbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c5b-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="16c5b-258">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="16c5b-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="16c5b-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="16c5b-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="16c5b-260">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-260">Int32</span></span>|<span data-ttu-id="16c5b-261">Minimale Anzahl der Großbuchstaben in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c5b-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="16c5b-262">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="16c5b-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="16c5b-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="16c5b-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="16c5b-264">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-264">Int32</span></span>|<span data-ttu-id="16c5b-265">Minimale Anzahl der Symbole in Arbeit Profilkennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c5b-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="16c5b-266">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="16c5b-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="16c5b-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="16c5b-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="16c5b-268">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-268">Int32</span></span>|<span data-ttu-id="16c5b-269">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="16c5b-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="16c5b-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="16c5b-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="16c5b-271">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-271">Int32</span></span>|<span data-ttu-id="16c5b-272">Anzahl der vorherigen Arbeit Profil Kennwörter zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="16c5b-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="16c5b-273">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="16c5b-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="16c5b-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="16c5b-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="16c5b-275">Int32</span><span class="sxs-lookup"><span data-stu-id="16c5b-275">Int32</span></span>|<span data-ttu-id="16c5b-276">Anzahl der Anmeldung Fehler zulässig sind, bevor Arbeit Profil entfernt wird und alle Daten gelöscht.</span><span class="sxs-lookup"><span data-stu-id="16c5b-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="16c5b-277">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="16c5b-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="16c5b-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="16c5b-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="16c5b-279">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="16c5b-279">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="16c5b-280">Typ der Arbeit Profilkennwort, das erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="16c5b-280">Type of work profile password that is required.</span></span> <span data-ttu-id="16c5b-281">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="16c5b-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="16c5b-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="16c5b-282">workProfileRequirePassword</span></span>|<span data-ttu-id="16c5b-283">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-283">Boolean</span></span>|<span data-ttu-id="16c5b-284">Kennwort erforderlich ist oder nicht für Arbeit Profil</span><span class="sxs-lookup"><span data-stu-id="16c5b-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="16c5b-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="16c5b-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="16c5b-286">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="16c5b-286">Boolean</span></span>|<span data-ttu-id="16c5b-287">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="16c5b-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="16c5b-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="16c5b-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="16c5b-289">String</span><span class="sxs-lookup"><span data-stu-id="16c5b-289">String</span></span>|<span data-ttu-id="16c5b-290">Aktivieren Sie Sperrmodus für immer auf VPN.</span><span class="sxs-lookup"><span data-stu-id="16c5b-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="16c5b-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="16c5b-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="16c5b-292">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16c5b-292">Boolean</span></span>|<span data-ttu-id="16c5b-293">Aktivieren Sie Sperrmodus für immer auf VPN.</span><span class="sxs-lookup"><span data-stu-id="16c5b-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="16c5b-294">Antwort</span><span class="sxs-lookup"><span data-stu-id="16c5b-294">Response</span></span>
<span data-ttu-id="16c5b-295">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="16c5b-295">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16c5b-296">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16c5b-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="16c5b-297">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16c5b-297">Request</span></span>
<span data-ttu-id="16c5b-298">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16c5b-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2106

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="16c5b-299">Antwort</span><span class="sxs-lookup"><span data-stu-id="16c5b-299">Response</span></span>
<span data-ttu-id="16c5b-p129">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16c5b-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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





