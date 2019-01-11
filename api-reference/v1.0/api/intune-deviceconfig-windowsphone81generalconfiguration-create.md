---
title: Erstellen von „windowsPhone81GeneralConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 594dc82a4be7e939bd04d937cbf4d2ed583d7ddd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867081"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="662be-103">Erstellen von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="662be-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="662be-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="662be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="662be-105">Diese Methode erstellt ein neues Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-105">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="662be-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="662be-106">Prerequisites</span></span>
<span data-ttu-id="662be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="662be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="662be-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="662be-109">Permission type</span></span>|<span data-ttu-id="662be-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="662be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="662be-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="662be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="662be-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="662be-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="662be-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="662be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="662be-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="662be-114">Not supported.</span></span>|
|<span data-ttu-id="662be-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="662be-115">Application</span></span>|<span data-ttu-id="662be-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="662be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="662be-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="662be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="662be-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="662be-118">Request headers</span></span>
|<span data-ttu-id="662be-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="662be-119">Header</span></span>|<span data-ttu-id="662be-120">Wert</span><span class="sxs-lookup"><span data-stu-id="662be-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="662be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="662be-121">Authorization</span></span>|<span data-ttu-id="662be-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="662be-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="662be-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="662be-123">Accept</span></span>|<span data-ttu-id="662be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="662be-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="662be-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="662be-125">Request body</span></span>
<span data-ttu-id="662be-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsPhone81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="662be-126">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="662be-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsPhone81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="662be-127">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="662be-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="662be-128">Property</span></span>|<span data-ttu-id="662be-129">Typ</span><span class="sxs-lookup"><span data-stu-id="662be-129">Type</span></span>|<span data-ttu-id="662be-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="662be-131">id</span><span class="sxs-lookup"><span data-stu-id="662be-131">id</span></span>|<span data-ttu-id="662be-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662be-132">String</span></span>|<span data-ttu-id="662be-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="662be-133">Key of the entity.</span></span> <span data-ttu-id="662be-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="662be-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="662be-135">lastModifiedDateTime</span></span>|<span data-ttu-id="662be-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662be-136">DateTimeOffset</span></span>|<span data-ttu-id="662be-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="662be-137">DateTime the object was last modified.</span></span> <span data-ttu-id="662be-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="662be-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="662be-139">createdDateTime</span></span>|<span data-ttu-id="662be-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662be-140">DateTimeOffset</span></span>|<span data-ttu-id="662be-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="662be-141">DateTime the object was created.</span></span> <span data-ttu-id="662be-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="662be-143">description</span><span class="sxs-lookup"><span data-stu-id="662be-143">description</span></span>|<span data-ttu-id="662be-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662be-144">String</span></span>|<span data-ttu-id="662be-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="662be-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="662be-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="662be-147">displayName</span><span class="sxs-lookup"><span data-stu-id="662be-147">displayName</span></span>|<span data-ttu-id="662be-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662be-148">String</span></span>|<span data-ttu-id="662be-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="662be-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="662be-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="662be-151">Version</span><span class="sxs-lookup"><span data-stu-id="662be-151">version</span></span>|<span data-ttu-id="662be-152">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-152">Int32</span></span>|<span data-ttu-id="662be-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="662be-153">Version of the device configuration.</span></span> <span data-ttu-id="662be-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="662be-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="662be-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="662be-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="662be-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-156">Boolean</span></span>|<span data-ttu-id="662be-157">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="662be-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="662be-158">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="662be-158">This property is read-only.</span></span>|
|<span data-ttu-id="662be-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="662be-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="662be-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-160">Boolean</span></span>|<span data-ttu-id="662be-161">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="662be-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-162">bluetoothBlocked</span></span>|<span data-ttu-id="662be-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-163">Boolean</span></span>|<span data-ttu-id="662be-164">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="662be-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-165">cameraBlocked</span></span>|<span data-ttu-id="662be-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-166">Boolean</span></span>|<span data-ttu-id="662be-167">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="662be-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="662be-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="662be-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-169">Boolean</span></span>|<span data-ttu-id="662be-170">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="662be-171">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="662be-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="662be-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="662be-172">compliantAppsList</span></span>|<span data-ttu-id="662be-173">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="662be-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="662be-174">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="662be-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="662be-175">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="662be-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="662be-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="662be-176">compliantAppListType</span></span>|[<span data-ttu-id="662be-177">appListType</span><span class="sxs-lookup"><span data-stu-id="662be-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="662be-178">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="662be-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="662be-179">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="662be-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="662be-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="662be-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="662be-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="662be-181">Boolean</span></span>|<span data-ttu-id="662be-182">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="662be-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="662be-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="662be-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-184">Boolean</span></span>|<span data-ttu-id="662be-185">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="662be-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="662be-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-186">locationServicesBlocked</span></span>|<span data-ttu-id="662be-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="662be-187">Boolean</span></span>|<span data-ttu-id="662be-188">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="662be-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="662be-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="662be-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-190">Boolean</span></span>|<span data-ttu-id="662be-191">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="662be-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="662be-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-192">nfcBlocked</span></span>|<span data-ttu-id="662be-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="662be-193">Boolean</span></span>|<span data-ttu-id="662be-194">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="662be-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="662be-195">passwordBlockSimple</span></span>|<span data-ttu-id="662be-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-196">Boolean</span></span>|<span data-ttu-id="662be-197">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="662be-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="662be-198">passwordExpirationDays</span></span>|<span data-ttu-id="662be-199">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-199">Int32</span></span>|<span data-ttu-id="662be-200">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="662be-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="662be-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="662be-201">passwordMinimumLength</span></span>|<span data-ttu-id="662be-202">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-202">Int32</span></span>|<span data-ttu-id="662be-203">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="662be-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="662be-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="662be-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="662be-205">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-205">Int32</span></span>|<span data-ttu-id="662be-206">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="662be-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="662be-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="662be-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="662be-208">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-208">Int32</span></span>|<span data-ttu-id="662be-209">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="662be-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="662be-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="662be-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="662be-211">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-211">Int32</span></span>|<span data-ttu-id="662be-212">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="662be-212">Number of previous passwords to block.</span></span> <span data-ttu-id="662be-213">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="662be-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="662be-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="662be-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="662be-215">Int32</span><span class="sxs-lookup"><span data-stu-id="662be-215">Int32</span></span>|<span data-ttu-id="662be-216">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="662be-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="662be-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="662be-217">passwordRequiredType</span></span>|[<span data-ttu-id="662be-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="662be-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="662be-219">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="662be-219">Password type that is required.</span></span> <span data-ttu-id="662be-220">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="662be-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="662be-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="662be-221">passwordRequired</span></span>|<span data-ttu-id="662be-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="662be-222">Boolean</span></span>|<span data-ttu-id="662be-223">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="662be-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="662be-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-224">screenCaptureBlocked</span></span>|<span data-ttu-id="662be-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="662be-225">Boolean</span></span>|<span data-ttu-id="662be-226">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="662be-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="662be-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="662be-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="662be-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-228">Boolean</span></span>|<span data-ttu-id="662be-229">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="662be-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="662be-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="662be-230">storageRequireEncryption</span></span>|<span data-ttu-id="662be-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-231">Boolean</span></span>|<span data-ttu-id="662be-232">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="662be-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="662be-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-233">webBrowserBlocked</span></span>|<span data-ttu-id="662be-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="662be-234">Boolean</span></span>|<span data-ttu-id="662be-235">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="662be-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-236">wifiBlocked</span></span>|<span data-ttu-id="662be-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-237">Boolean</span></span>|<span data-ttu-id="662be-238">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="662be-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="662be-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="662be-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-240">Boolean</span></span>|<span data-ttu-id="662be-241">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="662be-242">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="662be-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="662be-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="662be-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="662be-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-244">Boolean</span></span>|<span data-ttu-id="662be-245">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="662be-246">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="662be-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="662be-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="662be-247">windowsStoreBlocked</span></span>|<span data-ttu-id="662be-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="662be-248">Boolean</span></span>|<span data-ttu-id="662be-249">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="662be-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="662be-250">Antwort</span><span class="sxs-lookup"><span data-stu-id="662be-250">Response</span></span>
<span data-ttu-id="662be-251">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="662be-251">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="662be-252">Beispiel</span><span class="sxs-lookup"><span data-stu-id="662be-252">Example</span></span>
### <a name="request"></a><span data-ttu-id="662be-253">Anforderung</span><span class="sxs-lookup"><span data-stu-id="662be-253">Request</span></span>
<span data-ttu-id="662be-254">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="662be-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="662be-255">Antwort</span><span class="sxs-lookup"><span data-stu-id="662be-255">Response</span></span>
<span data-ttu-id="662be-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="662be-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



