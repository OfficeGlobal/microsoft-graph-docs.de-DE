---
title: AndroidWorkProfileGeneralDeviceConfiguration erstellen
description: Erstellen eines neuen androidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f59e923aeb083846d57f33f8524b5cba44cf8e5f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262867"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="8f6a8-103">AndroidWorkProfileGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="8f6a8-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8f6a8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f6a8-105">Erstellen eines neuen [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f6a8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8f6a8-106">Prerequisites</span></span>
<span data-ttu-id="8f6a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f6a8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f6a8-109">Permission type</span></span>|<span data-ttu-id="8f6a8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f6a8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f6a8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f6a8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f6a8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f6a8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f6a8-114">Not supported.</span></span>|
|<span data-ttu-id="8f6a8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f6a8-115">Application</span></span>|<span data-ttu-id="8f6a8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f6a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f6a8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f6a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f6a8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f6a8-118">Request headers</span></span>
|<span data-ttu-id="8f6a8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8f6a8-119">Header</span></span>|<span data-ttu-id="8f6a8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8f6a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f6a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f6a8-121">Authorization</span></span>|<span data-ttu-id="8f6a8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8f6a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f6a8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8f6a8-123">Accept</span></span>|<span data-ttu-id="8f6a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f6a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f6a8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f6a8-125">Request body</span></span>
<span data-ttu-id="8f6a8-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidWorkProfileGeneralDeviceConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="8f6a8-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidWorkProfileGeneralDeviceConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="8f6a8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f6a8-128">Property</span></span>|<span data-ttu-id="8f6a8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8f6a8-129">Type</span></span>|<span data-ttu-id="8f6a8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f6a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f6a8-131">id</span><span class="sxs-lookup"><span data-stu-id="8f6a8-131">id</span></span>|<span data-ttu-id="8f6a8-132">string</span><span class="sxs-lookup"><span data-stu-id="8f6a8-132">String</span></span>|<span data-ttu-id="8f6a8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8f6a8-133">Key of the entity.</span></span> <span data-ttu-id="8f6a8-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f6a8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f6a8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8f6a8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f6a8-136">DateTimeOffset</span></span>|<span data-ttu-id="8f6a8-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8f6a8-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f6a8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f6a8-139">createdDateTime</span></span>|<span data-ttu-id="8f6a8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f6a8-140">DateTimeOffset</span></span>|<span data-ttu-id="8f6a8-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-141">DateTime the object was created.</span></span> <span data-ttu-id="8f6a8-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f6a8-143">description</span><span class="sxs-lookup"><span data-stu-id="8f6a8-143">description</span></span>|<span data-ttu-id="8f6a8-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f6a8-144">String</span></span>|<span data-ttu-id="8f6a8-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f6a8-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f6a8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8f6a8-147">displayName</span></span>|<span data-ttu-id="8f6a8-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f6a8-148">String</span></span>|<span data-ttu-id="8f6a8-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f6a8-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f6a8-151">Version</span><span class="sxs-lookup"><span data-stu-id="8f6a8-151">version</span></span>|<span data-ttu-id="8f6a8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-152">Int32</span></span>|<span data-ttu-id="8f6a8-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-153">Version of the device configuration.</span></span> <span data-ttu-id="8f6a8-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f6a8-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="8f6a8-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="8f6a8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-156">Boolean</span></span>|<span data-ttu-id="8f6a8-157">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="8f6a8-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="8f6a8-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="8f6a8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-159">Boolean</span></span>|<span data-ttu-id="8f6a8-160">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="8f6a8-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8f6a8-161">passwordExpirationDays</span></span>|<span data-ttu-id="8f6a8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-162">Int32</span></span>|<span data-ttu-id="8f6a8-163">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-163">Number of days before the password expires.</span></span> <span data-ttu-id="8f6a8-164">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8f6a8-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8f6a8-165">passwordMinimumLength</span></span>|<span data-ttu-id="8f6a8-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-166">Int32</span></span>|<span data-ttu-id="8f6a8-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-167">Minimum length of passwords.</span></span> <span data-ttu-id="8f6a8-168">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8f6a8-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8f6a8-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8f6a8-170">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-170">Int32</span></span>|<span data-ttu-id="8f6a8-171">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="8f6a8-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8f6a8-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8f6a8-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8f6a8-173">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-173">Int32</span></span>|<span data-ttu-id="8f6a8-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-174">Number of previous passwords to block.</span></span> <span data-ttu-id="8f6a8-175">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8f6a8-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8f6a8-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8f6a8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-177">Int32</span></span>|<span data-ttu-id="8f6a8-178">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="8f6a8-179">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="8f6a8-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8f6a8-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-180">passwordRequiredType</span></span>|[<span data-ttu-id="8f6a8-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="8f6a8-182">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-182">Type of password that is required.</span></span> <span data-ttu-id="8f6a8-183">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="8f6a8-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="8f6a8-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="8f6a8-186">Typ der zulässigen Datenfreigabe.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="8f6a8-187">Mögliche Werte: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="8f6a8-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="8f6a8-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="8f6a8-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-189">Boolean</span></span>|<span data-ttu-id="8f6a8-190">Gibt an, ob Benachrichtigungen blockiert werden sollen, während das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="8f6a8-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="8f6a8-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="8f6a8-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-192">Boolean</span></span>|<span data-ttu-id="8f6a8-193">Verhindern, dass Benutzerkonten im Arbeitsprofil hinzufügen/entfernen.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="8f6a8-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="8f6a8-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="8f6a8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-195">Boolean</span></span>|<span data-ttu-id="8f6a8-196">Bluetooth-Geräte können auf Enterprise-Kontakte zugreifen.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="8f6a8-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="8f6a8-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="8f6a8-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-198">Boolean</span></span>|<span data-ttu-id="8f6a8-199">Blockieren der Bildschirmaufzeichnung im Arbeitsprofil.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="8f6a8-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="8f6a8-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="8f6a8-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-201">Boolean</span></span>|<span data-ttu-id="8f6a8-202">Blockieren der Anzeige von Arbeitsprofil-Anrufer-ID im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="8f6a8-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="8f6a8-203">workProfileBlockCamera</span></span>|<span data-ttu-id="8f6a8-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-204">Boolean</span></span>|<span data-ttu-id="8f6a8-205">Arbeitsprofil Kamera blockieren.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-205">Block work profile camera.</span></span>|
|<span data-ttu-id="8f6a8-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="8f6a8-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="8f6a8-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-207">Boolean</span></span>|<span data-ttu-id="8f6a8-208">Blockieren der Verfügbarkeit von Arbeitsprofil Kontakten im persönlichen Profil</span><span class="sxs-lookup"><span data-stu-id="8f6a8-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="8f6a8-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="8f6a8-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="8f6a8-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-210">Boolean</span></span>|<span data-ttu-id="8f6a8-211">Boolescher Wert, der angibt, ob die Einstellung Cross profile Copy/Paste nicht zulassen aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="8f6a8-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="8f6a8-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="8f6a8-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="8f6a8-214">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-214">Type of password that is required.</span></span> <span data-ttu-id="8f6a8-215">Mögliche Werte: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="8f6a8-216">Eigenschaften workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="8f6a8-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="8f6a8-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-217">Boolean</span></span>|<span data-ttu-id="8f6a8-218">Gibt an, ob die Fingerabdruck Sperre für das Arbeitsprofil blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="8f6a8-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="8f6a8-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="8f6a8-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-220">Boolean</span></span>|<span data-ttu-id="8f6a8-221">Gibt an, ob die Smart Lock-und andere Trust-Agents für das Arbeitsprofil blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="8f6a8-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8f6a8-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="8f6a8-223">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-223">Int32</span></span>|<span data-ttu-id="8f6a8-224">Anzahl der Tage vor Ablauf des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="8f6a8-225">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8f6a8-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8f6a8-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="8f6a8-227">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-227">Int32</span></span>|<span data-ttu-id="8f6a8-228">Minimale Länge des Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-228">Minimum length of work profile password.</span></span> <span data-ttu-id="8f6a8-229">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8f6a8-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="8f6a8-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="8f6a8-231">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-231">Int32</span></span>|<span data-ttu-id="8f6a8-232">Minimale Anzahl von numerischen Zeichen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="8f6a8-233">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="8f6a8-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="8f6a8-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="8f6a8-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="8f6a8-235">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-235">Int32</span></span>|<span data-ttu-id="8f6a8-236">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="8f6a8-237">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="8f6a8-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="8f6a8-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="8f6a8-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="8f6a8-239">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-239">Int32</span></span>|<span data-ttu-id="8f6a8-240">Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="8f6a8-241">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="8f6a8-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="8f6a8-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="8f6a8-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="8f6a8-243">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-243">Int32</span></span>|<span data-ttu-id="8f6a8-244">Minimale Anzahl von Kleinbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="8f6a8-245">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="8f6a8-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="8f6a8-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="8f6a8-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="8f6a8-247">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-247">Int32</span></span>|<span data-ttu-id="8f6a8-248">Minimale Anzahl von Großbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="8f6a8-249">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="8f6a8-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="8f6a8-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="8f6a8-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="8f6a8-251">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-251">Int32</span></span>|<span data-ttu-id="8f6a8-252">Minimale Anzahl von Symbolen, die im Arbeitsprofil Kennwort erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="8f6a8-253">Gültige Werte 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="8f6a8-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="8f6a8-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8f6a8-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8f6a8-255">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-255">Int32</span></span>|<span data-ttu-id="8f6a8-256">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="8f6a8-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8f6a8-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8f6a8-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8f6a8-258">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-258">Int32</span></span>|<span data-ttu-id="8f6a8-259">Anzahl der vorherigen Arbeitsprofil Kennwörter, die blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="8f6a8-260">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8f6a8-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8f6a8-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8f6a8-262">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6a8-262">Int32</span></span>|<span data-ttu-id="8f6a8-263">Anzahl der zulässigen Anmeldefehler vor dem Entfernen des Arbeitsprofils und aller gelöschten Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="8f6a8-264">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="8f6a8-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8f6a8-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="8f6a8-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8f6a8-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="8f6a8-267">Typ des erforderlichen Arbeitsprofil Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-267">Type of work profile password that is required.</span></span> <span data-ttu-id="8f6a8-268">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="8f6a8-269">Workprofilerequirepassword wurden</span><span class="sxs-lookup"><span data-stu-id="8f6a8-269">workProfileRequirePassword</span></span>|<span data-ttu-id="8f6a8-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-270">Boolean</span></span>|<span data-ttu-id="8f6a8-271">Kennwort ist erforderlich oder nicht für das Arbeitsprofil</span><span class="sxs-lookup"><span data-stu-id="8f6a8-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="8f6a8-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8f6a8-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="8f6a8-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f6a8-273">Boolean</span></span>|<span data-ttu-id="8f6a8-274">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="8f6a8-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f6a8-275">Response</span></span>
<span data-ttu-id="8f6a8-276">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f6a8-277">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f6a8-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f6a8-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f6a8-278">Request</span></span>
<span data-ttu-id="8f6a8-279">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f6a8-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f6a8-280">Response</span></span>
<span data-ttu-id="8f6a8-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



