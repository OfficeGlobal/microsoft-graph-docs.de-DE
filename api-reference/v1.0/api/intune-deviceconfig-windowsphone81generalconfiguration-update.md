---
title: Aktualisieren von „windowsPhone81GeneralConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49a200ef46b9f7f068d7100888daae576d7e8c9c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263931"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="e488a-103">Aktualisieren von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e488a-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="e488a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e488a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e488a-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-105">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e488a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e488a-106">Prerequisites</span></span>
<span data-ttu-id="e488a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e488a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e488a-109">Permission type</span></span>|<span data-ttu-id="e488a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e488a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e488a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e488a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e488a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e488a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e488a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e488a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e488a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e488a-114">Not supported.</span></span>|
|<span data-ttu-id="e488a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e488a-115">Application</span></span>|<span data-ttu-id="e488a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e488a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e488a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e488a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e488a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e488a-118">Request headers</span></span>
|<span data-ttu-id="e488a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e488a-119">Header</span></span>|<span data-ttu-id="e488a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e488a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e488a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e488a-121">Authorization</span></span>|<span data-ttu-id="e488a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e488a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e488a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e488a-123">Accept</span></span>|<span data-ttu-id="e488a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e488a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e488a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e488a-125">Request body</span></span>
<span data-ttu-id="e488a-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="e488a-126">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="e488a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e488a-127">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="e488a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e488a-128">Property</span></span>|<span data-ttu-id="e488a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e488a-129">Type</span></span>|<span data-ttu-id="e488a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e488a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e488a-131">id</span><span class="sxs-lookup"><span data-stu-id="e488a-131">id</span></span>|<span data-ttu-id="e488a-132">string</span><span class="sxs-lookup"><span data-stu-id="e488a-132">String</span></span>|<span data-ttu-id="e488a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e488a-133">Key of the entity.</span></span> <span data-ttu-id="e488a-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e488a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e488a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e488a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e488a-136">DateTimeOffset</span></span>|<span data-ttu-id="e488a-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e488a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="e488a-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e488a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e488a-139">createdDateTime</span></span>|<span data-ttu-id="e488a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e488a-140">DateTimeOffset</span></span>|<span data-ttu-id="e488a-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e488a-141">DateTime the object was created.</span></span> <span data-ttu-id="e488a-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e488a-143">description</span><span class="sxs-lookup"><span data-stu-id="e488a-143">description</span></span>|<span data-ttu-id="e488a-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e488a-144">String</span></span>|<span data-ttu-id="e488a-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e488a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e488a-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e488a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e488a-147">displayName</span></span>|<span data-ttu-id="e488a-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e488a-148">String</span></span>|<span data-ttu-id="e488a-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e488a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e488a-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e488a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e488a-151">Version</span><span class="sxs-lookup"><span data-stu-id="e488a-151">version</span></span>|<span data-ttu-id="e488a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-152">Int32</span></span>|<span data-ttu-id="e488a-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e488a-153">Version of the device configuration.</span></span> <span data-ttu-id="e488a-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e488a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e488a-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="e488a-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="e488a-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-156">Boolean</span></span>|<span data-ttu-id="e488a-157">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="e488a-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="e488a-158">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e488a-158">This property is read-only.</span></span>|
|<span data-ttu-id="e488a-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e488a-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="e488a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-160">Boolean</span></span>|<span data-ttu-id="e488a-161">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="e488a-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-162">bluetoothBlocked</span></span>|<span data-ttu-id="e488a-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-163">Boolean</span></span>|<span data-ttu-id="e488a-164">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="e488a-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-165">cameraBlocked</span></span>|<span data-ttu-id="e488a-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-166">Boolean</span></span>|<span data-ttu-id="e488a-167">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="e488a-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="e488a-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="e488a-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-169">Boolean</span></span>|<span data-ttu-id="e488a-170">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="e488a-171">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="e488a-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="e488a-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e488a-172">compliantAppsList</span></span>|<span data-ttu-id="e488a-173">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e488a-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e488a-174">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="e488a-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e488a-175">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e488a-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e488a-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e488a-176">compliantAppListType</span></span>|[<span data-ttu-id="e488a-177">appListType</span><span class="sxs-lookup"><span data-stu-id="e488a-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e488a-178">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="e488a-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="e488a-179">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="e488a-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e488a-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="e488a-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="e488a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-181">Boolean</span></span>|<span data-ttu-id="e488a-182">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="e488a-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="e488a-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="e488a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-184">Boolean</span></span>|<span data-ttu-id="e488a-185">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e488a-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="e488a-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-186">locationServicesBlocked</span></span>|<span data-ttu-id="e488a-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-187">Boolean</span></span>|<span data-ttu-id="e488a-188">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e488a-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="e488a-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="e488a-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e488a-190">Boolean</span></span>|<span data-ttu-id="e488a-191">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="e488a-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="e488a-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-192">nfcBlocked</span></span>|<span data-ttu-id="e488a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-193">Boolean</span></span>|<span data-ttu-id="e488a-194">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="e488a-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e488a-195">passwordBlockSimple</span></span>|<span data-ttu-id="e488a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-196">Boolean</span></span>|<span data-ttu-id="e488a-197">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e488a-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e488a-198">passwordExpirationDays</span></span>|<span data-ttu-id="e488a-199">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-199">Int32</span></span>|<span data-ttu-id="e488a-200">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="e488a-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e488a-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e488a-201">passwordMinimumLength</span></span>|<span data-ttu-id="e488a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-202">Int32</span></span>|<span data-ttu-id="e488a-203">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="e488a-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e488a-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e488a-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e488a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-205">Int32</span></span>|<span data-ttu-id="e488a-206">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="e488a-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="e488a-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e488a-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e488a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-208">Int32</span></span>|<span data-ttu-id="e488a-209">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="e488a-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="e488a-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e488a-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e488a-211">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-211">Int32</span></span>|<span data-ttu-id="e488a-212">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="e488a-212">Number of previous passwords to block.</span></span> <span data-ttu-id="e488a-213">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="e488a-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e488a-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e488a-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e488a-215">Int32</span><span class="sxs-lookup"><span data-stu-id="e488a-215">Int32</span></span>|<span data-ttu-id="e488a-216">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="e488a-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="e488a-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e488a-217">passwordRequiredType</span></span>|[<span data-ttu-id="e488a-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e488a-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e488a-219">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="e488a-219">Password type that is required.</span></span> <span data-ttu-id="e488a-220">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e488a-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e488a-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e488a-221">passwordRequired</span></span>|<span data-ttu-id="e488a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-222">Boolean</span></span>|<span data-ttu-id="e488a-223">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e488a-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="e488a-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-224">screenCaptureBlocked</span></span>|<span data-ttu-id="e488a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-225">Boolean</span></span>|<span data-ttu-id="e488a-226">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e488a-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="e488a-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="e488a-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="e488a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-228">Boolean</span></span>|<span data-ttu-id="e488a-229">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e488a-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="e488a-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e488a-230">storageRequireEncryption</span></span>|<span data-ttu-id="e488a-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e488a-231">Boolean</span></span>|<span data-ttu-id="e488a-232">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e488a-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="e488a-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-233">webBrowserBlocked</span></span>|<span data-ttu-id="e488a-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e488a-234">Boolean</span></span>|<span data-ttu-id="e488a-235">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="e488a-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-236">wifiBlocked</span></span>|<span data-ttu-id="e488a-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-237">Boolean</span></span>|<span data-ttu-id="e488a-238">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="e488a-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="e488a-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="e488a-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-240">Boolean</span></span>|<span data-ttu-id="e488a-241">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="e488a-242">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="e488a-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="e488a-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="e488a-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="e488a-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-244">Boolean</span></span>|<span data-ttu-id="e488a-245">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="e488a-246">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="e488a-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="e488a-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e488a-247">windowsStoreBlocked</span></span>|<span data-ttu-id="e488a-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="e488a-248">Boolean</span></span>|<span data-ttu-id="e488a-249">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e488a-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="e488a-250">Antwort</span><span class="sxs-lookup"><span data-stu-id="e488a-250">Response</span></span>
<span data-ttu-id="e488a-251">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e488a-251">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e488a-252">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e488a-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="e488a-253">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e488a-253">Request</span></span>
<span data-ttu-id="e488a-254">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e488a-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="e488a-255">Antwort</span><span class="sxs-lookup"><span data-stu-id="e488a-255">Response</span></span>
<span data-ttu-id="e488a-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e488a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



