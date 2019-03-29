---
title: AndroidWorkProfileGeneralDeviceConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fc6526c2d01ad8aecef932f6cf78c6065540f2f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973565"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="b8354-103">AndroidWorkProfileGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b8354-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b8354-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8354-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8354-106">Aktualisieren der Eigenschaften eines [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8354-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8354-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8354-107">Prerequisites</span></span>
<span data-ttu-id="b8354-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8354-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8354-110">Permission type</span></span>|<span data-ttu-id="b8354-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8354-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8354-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8354-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8354-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8354-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8354-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8354-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8354-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8354-115">Not supported.</span></span>|
|<span data-ttu-id="b8354-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8354-116">Application</span></span>|<span data-ttu-id="b8354-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8354-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8354-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8354-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b8354-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8354-119">Request headers</span></span>
|<span data-ttu-id="b8354-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8354-120">Header</span></span>|<span data-ttu-id="b8354-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8354-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8354-122">Authorization</span></span>|<span data-ttu-id="b8354-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8354-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8354-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8354-124">Accept</span></span>|<span data-ttu-id="b8354-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8354-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8354-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8354-126">Request body</span></span>
<span data-ttu-id="b8354-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b8354-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b8354-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b8354-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8354-129">Property</span></span>|<span data-ttu-id="b8354-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b8354-130">Type</span></span>|<span data-ttu-id="b8354-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8354-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8354-132">id</span><span class="sxs-lookup"><span data-stu-id="b8354-132">id</span></span>|<span data-ttu-id="b8354-133">String</span><span class="sxs-lookup"><span data-stu-id="b8354-133">String</span></span>|<span data-ttu-id="b8354-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b8354-134">Key of the entity.</span></span> <span data-ttu-id="b8354-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8354-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b8354-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8354-137">DateTimeOffset</span></span>|<span data-ttu-id="b8354-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8354-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b8354-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b8354-140">roleScopeTagIds</span></span>|<span data-ttu-id="b8354-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b8354-141">String collection</span></span>|<span data-ttu-id="b8354-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="b8354-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8354-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8354-144">supportsScopeTags</span></span>|<span data-ttu-id="b8354-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-145">Boolean</span></span>|<span data-ttu-id="b8354-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8354-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8354-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8354-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b8354-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8354-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b8354-149">This property is read-only.</span></span> <span data-ttu-id="b8354-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8354-151">createdDateTime</span></span>|<span data-ttu-id="b8354-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8354-152">DateTimeOffset</span></span>|<span data-ttu-id="b8354-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8354-153">DateTime the object was created.</span></span> <span data-ttu-id="b8354-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-155">description</span><span class="sxs-lookup"><span data-stu-id="b8354-155">description</span></span>|<span data-ttu-id="b8354-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8354-156">String</span></span>|<span data-ttu-id="b8354-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b8354-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8354-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b8354-159">displayName</span></span>|<span data-ttu-id="b8354-160">String</span><span class="sxs-lookup"><span data-stu-id="b8354-160">String</span></span>|<span data-ttu-id="b8354-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b8354-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8354-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-163">Version</span><span class="sxs-lookup"><span data-stu-id="b8354-163">version</span></span>|<span data-ttu-id="b8354-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-164">Int32</span></span>|<span data-ttu-id="b8354-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b8354-165">Version of the device configuration.</span></span> <span data-ttu-id="b8354-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8354-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8354-167">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b8354-167">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b8354-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-168">Boolean</span></span>|<span data-ttu-id="b8354-169">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8354-169">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b8354-170">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="b8354-170">passwordBlockTrustAgents</span></span>|<span data-ttu-id="b8354-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8354-171">Boolean</span></span>|<span data-ttu-id="b8354-172">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b8354-172">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="b8354-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b8354-173">passwordExpirationDays</span></span>|<span data-ttu-id="b8354-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-174">Int32</span></span>|<span data-ttu-id="b8354-175">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="b8354-175">Number of days before the password expires.</span></span> <span data-ttu-id="b8354-176">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="b8354-176">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b8354-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b8354-177">passwordMinimumLength</span></span>|<span data-ttu-id="b8354-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-178">Int32</span></span>|<span data-ttu-id="b8354-179">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="b8354-179">Minimum length of passwords.</span></span> <span data-ttu-id="b8354-180">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="b8354-180">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b8354-181">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b8354-181">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b8354-182">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-182">Int32</span></span>|<span data-ttu-id="b8354-183">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="b8354-183">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b8354-184">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b8354-184">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b8354-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-185">Int32</span></span>|<span data-ttu-id="b8354-186">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="b8354-186">Number of previous passwords to block.</span></span> <span data-ttu-id="b8354-187">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="b8354-187">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b8354-188">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b8354-188">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b8354-189">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-189">Int32</span></span>|<span data-ttu-id="b8354-190">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="b8354-190">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="b8354-191">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="b8354-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b8354-192">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b8354-192">passwordRequiredType</span></span>|[<span data-ttu-id="b8354-193">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b8354-193">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="b8354-194">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="b8354-194">Type of password that is required.</span></span> <span data-ttu-id="b8354-195">Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="b8354-195">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="b8354-196">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="b8354-196">workProfileDataSharingType</span></span>|[<span data-ttu-id="b8354-197">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="b8354-197">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="b8354-198">Typ der zulässigen Datenfreigabe.</span><span class="sxs-lookup"><span data-stu-id="b8354-198">Type of data sharing that is allowed.</span></span> <span data-ttu-id="b8354-199">Mögliche Werte sind: `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="b8354-199">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="b8354-200">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="b8354-200">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="b8354-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-201">Boolean</span></span>|<span data-ttu-id="b8354-202">Gibt an, ob Benachrichtigungen blockiert werden sollen, während das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="b8354-202">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="b8354-203">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="b8354-203">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="b8354-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-204">Boolean</span></span>|<span data-ttu-id="b8354-205">Verhindern, dass Benutzerkonten im Arbeitsprofil hinzufügen/entfernen.</span><span class="sxs-lookup"><span data-stu-id="b8354-205">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="b8354-206">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="b8354-206">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="b8354-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-207">Boolean</span></span>|<span data-ttu-id="b8354-208">Bluetooth-Geräte können auf Enterprise-Kontakte zugreifen.</span><span class="sxs-lookup"><span data-stu-id="b8354-208">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="b8354-209">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="b8354-209">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="b8354-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-210">Boolean</span></span>|<span data-ttu-id="b8354-211">Blockieren der Bildschirmaufzeichnung im Arbeitsprofil.</span><span class="sxs-lookup"><span data-stu-id="b8354-211">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="b8354-212">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="b8354-212">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="b8354-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-213">Boolean</span></span>|<span data-ttu-id="b8354-214">Blockieren der Anzeige von Arbeitsprofil-Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="b8354-214">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="b8354-215">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="b8354-215">workProfileBlockCamera</span></span>|<span data-ttu-id="b8354-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-216">Boolean</span></span>|<span data-ttu-id="b8354-217">Arbeitsprofil Kamera blockieren.</span><span class="sxs-lookup"><span data-stu-id="b8354-217">Block work profile camera.</span></span>|
|<span data-ttu-id="b8354-218">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="b8354-218">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="b8354-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-219">Boolean</span></span>|<span data-ttu-id="b8354-220">Blockieren der Verfügbarkeit von Arbeitsprofil Kontakten im persönlichen Profil</span><span class="sxs-lookup"><span data-stu-id="b8354-220">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="b8354-221">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="b8354-221">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="b8354-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-222">Boolean</span></span>|<span data-ttu-id="b8354-223">Boolescher Wert, der angibt, ob die Einstellung Cross profile Copy/Paste nicht zulassen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b8354-223">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="b8354-224">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="b8354-224">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="b8354-225">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="b8354-225">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="b8354-226">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="b8354-226">Type of password that is required.</span></span> <span data-ttu-id="b8354-227">Mögliche Werte sind: `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="b8354-227">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="b8354-228">Eigenschaften workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="b8354-228">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b8354-229">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-229">Boolean</span></span>|<span data-ttu-id="b8354-230">Gibt an, ob die Fingerabdruck Sperre für das Arbeitsprofil blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8354-230">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="b8354-231">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="b8354-231">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="b8354-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-232">Boolean</span></span>|<span data-ttu-id="b8354-233">Gibt an, ob die Smart Lock-und andere Trust-Agents für das Arbeitsprofil blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b8354-233">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="b8354-234">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b8354-234">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="b8354-235">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-235">Int32</span></span>|<span data-ttu-id="b8354-236">Anzahl der Tage vor Ablauf des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="b8354-236">Number of days before the work profile password expires.</span></span> <span data-ttu-id="b8354-237">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="b8354-237">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b8354-238">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b8354-238">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="b8354-239">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-239">Int32</span></span>|<span data-ttu-id="b8354-240">Minimale Länge des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="b8354-240">Minimum length of work profile password.</span></span> <span data-ttu-id="b8354-241">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="b8354-241">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b8354-242">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="b8354-242">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="b8354-243">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-243">Int32</span></span>|<span data-ttu-id="b8354-244">Minimale Anzahl von numerischen Zeichen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-244">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="b8354-245">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="b8354-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b8354-246">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b8354-246">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="b8354-247">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-247">Int32</span></span>|<span data-ttu-id="b8354-248">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-248">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="b8354-249">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="b8354-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b8354-250">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b8354-250">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="b8354-251">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-251">Int32</span></span>|<span data-ttu-id="b8354-252">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-252">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="b8354-253">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="b8354-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b8354-254">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b8354-254">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="b8354-255">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-255">Int32</span></span>|<span data-ttu-id="b8354-256">Minimale Anzahl von Kleinbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-256">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="b8354-257">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="b8354-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b8354-258">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b8354-258">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="b8354-259">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-259">Int32</span></span>|<span data-ttu-id="b8354-260">Minimale Anzahl von Großbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-260">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="b8354-261">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="b8354-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b8354-262">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="b8354-262">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="b8354-263">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-263">Int32</span></span>|<span data-ttu-id="b8354-264">Minimale Anzahl von Symbolen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b8354-264">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="b8354-265">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="b8354-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="b8354-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b8354-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b8354-267">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-267">Int32</span></span>|<span data-ttu-id="b8354-268">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="b8354-268">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b8354-269">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b8354-269">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b8354-270">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-270">Int32</span></span>|<span data-ttu-id="b8354-271">Anzahl der vorherigen Arbeitsprofil Kennwörter, die blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b8354-271">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="b8354-272">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="b8354-272">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b8354-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b8354-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b8354-274">Int32</span><span class="sxs-lookup"><span data-stu-id="b8354-274">Int32</span></span>|<span data-ttu-id="b8354-275">Anzahl der zulässigen Anmeldefehler vor dem Entfernen des Arbeitsprofils und aller gelöschten Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="b8354-275">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="b8354-276">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="b8354-276">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b8354-277">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b8354-277">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="b8354-278">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b8354-278">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="b8354-279">Typ des erforderlichen Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="b8354-279">Type of work profile password that is required.</span></span> <span data-ttu-id="b8354-280">Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="b8354-280">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="b8354-281">Workprofilerequirepassword wurden</span><span class="sxs-lookup"><span data-stu-id="b8354-281">workProfileRequirePassword</span></span>|<span data-ttu-id="b8354-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-282">Boolean</span></span>|<span data-ttu-id="b8354-283">Kennwort ist erforderlich oder nicht für das Arbeitsprofil</span><span class="sxs-lookup"><span data-stu-id="b8354-283">Password is required or not for work profile</span></span>|
|<span data-ttu-id="b8354-284">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b8354-284">securityRequireVerifyApps</span></span>|<span data-ttu-id="b8354-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8354-285">Boolean</span></span>|<span data-ttu-id="b8354-286">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="b8354-286">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b8354-287">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8354-287">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="b8354-288">String</span><span class="sxs-lookup"><span data-stu-id="b8354-288">String</span></span>|<span data-ttu-id="b8354-289">Aktivieren Sie den Sperrmodus für Always-on-VPN.</span><span class="sxs-lookup"><span data-stu-id="b8354-289">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="b8354-290">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="b8354-290">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="b8354-291">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8354-291">Boolean</span></span>|<span data-ttu-id="b8354-292">Aktivieren Sie den Sperrmodus für Always-on-VPN.</span><span class="sxs-lookup"><span data-stu-id="b8354-292">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="b8354-293">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8354-293">Response</span></span>
<span data-ttu-id="b8354-294">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8354-294">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8354-295">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8354-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8354-296">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8354-296">Request</span></span>
<span data-ttu-id="b8354-297">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8354-297">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="b8354-298">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8354-298">Response</span></span>
<span data-ttu-id="b8354-p128">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8354-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




