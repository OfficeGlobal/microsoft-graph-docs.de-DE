---
title: Erstellen von „macOSGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 859c1d90029e085c0ade42e58f12c0d34138ce3e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173122"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="1b818-103">Erstellen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="1b818-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1b818-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b818-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b818-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1b818-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b818-106">Diese Methode erstellt ein neues Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b818-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b818-107">Prerequisites</span></span>
<span data-ttu-id="1b818-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1b818-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b818-110">Permission type</span></span>|<span data-ttu-id="1b818-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b818-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b818-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b818-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b818-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b818-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b818-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b818-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b818-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b818-115">Not supported.</span></span>|
|<span data-ttu-id="1b818-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b818-116">Application</span></span>|<span data-ttu-id="1b818-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b818-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b818-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b818-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1b818-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b818-119">Request headers</span></span>
|<span data-ttu-id="1b818-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1b818-120">Header</span></span>|<span data-ttu-id="1b818-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b818-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b818-122">Authorization</span></span>|<span data-ttu-id="1b818-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b818-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b818-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1b818-124">Accept</span></span>|<span data-ttu-id="1b818-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b818-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b818-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b818-126">Request body</span></span>
<span data-ttu-id="1b818-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="1b818-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="1b818-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b818-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="1b818-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b818-129">Property</span></span>|<span data-ttu-id="1b818-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1b818-130">Type</span></span>|<span data-ttu-id="1b818-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b818-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b818-132">id</span><span class="sxs-lookup"><span data-stu-id="1b818-132">id</span></span>|<span data-ttu-id="1b818-133">string</span><span class="sxs-lookup"><span data-stu-id="1b818-133">String</span></span>|<span data-ttu-id="1b818-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1b818-134">Key of the entity.</span></span> <span data-ttu-id="1b818-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b818-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1b818-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b818-137">DateTimeOffset</span></span>|<span data-ttu-id="1b818-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b818-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1b818-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="1b818-140">roleScopeTagIds</span></span>|<span data-ttu-id="1b818-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1b818-141">String collection</span></span>|<span data-ttu-id="1b818-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="1b818-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1b818-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1b818-144">supportsScopeTags</span></span>|<span data-ttu-id="1b818-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-145">Boolean</span></span>|<span data-ttu-id="1b818-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b818-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1b818-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="1b818-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1b818-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="1b818-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1b818-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1b818-149">This property is read-only.</span></span> <span data-ttu-id="1b818-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b818-151">createdDateTime</span></span>|<span data-ttu-id="1b818-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b818-152">DateTimeOffset</span></span>|<span data-ttu-id="1b818-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b818-153">DateTime the object was created.</span></span> <span data-ttu-id="1b818-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-155">description</span><span class="sxs-lookup"><span data-stu-id="1b818-155">description</span></span>|<span data-ttu-id="1b818-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b818-156">String</span></span>|<span data-ttu-id="1b818-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1b818-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b818-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1b818-159">displayName</span></span>|<span data-ttu-id="1b818-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b818-160">String</span></span>|<span data-ttu-id="1b818-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1b818-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b818-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b818-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-163">Version</span><span class="sxs-lookup"><span data-stu-id="1b818-163">version</span></span>|<span data-ttu-id="1b818-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-164">Int32</span></span>|<span data-ttu-id="1b818-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1b818-165">Version of the device configuration.</span></span> <span data-ttu-id="1b818-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b818-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b818-167">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1b818-167">compliantAppsList</span></span>|<span data-ttu-id="1b818-168">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b818-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1b818-169">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="1b818-169">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1b818-170">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="1b818-170">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1b818-171">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1b818-171">compliantAppListType</span></span>|[<span data-ttu-id="1b818-172">appListType</span><span class="sxs-lookup"><span data-stu-id="1b818-172">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1b818-173">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="1b818-173">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="1b818-174">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1b818-174">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1b818-175">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="1b818-175">emailInDomainSuffixes</span></span>|<span data-ttu-id="1b818-176">String collection</span><span class="sxs-lookup"><span data-stu-id="1b818-176">String collection</span></span>|<span data-ttu-id="1b818-177">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="1b818-177">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="1b818-178">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1b818-178">passwordBlockSimple</span></span>|<span data-ttu-id="1b818-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b818-179">Boolean</span></span>|<span data-ttu-id="1b818-180">Unterbindet die Verwendung einfacher Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="1b818-180">Block simple passwords.</span></span>|
|<span data-ttu-id="1b818-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1b818-181">passwordExpirationDays</span></span>|<span data-ttu-id="1b818-182">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-182">Int32</span></span>|<span data-ttu-id="1b818-183">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="1b818-183">Number of days before the password expires.</span></span>|
|<span data-ttu-id="1b818-184">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1b818-184">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1b818-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-185">Int32</span></span>|<span data-ttu-id="1b818-186">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss.</span><span class="sxs-lookup"><span data-stu-id="1b818-186">Number of character sets a password must contain.</span></span> <span data-ttu-id="1b818-187">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="1b818-187">Valid values 0 to 4</span></span>|
|<span data-ttu-id="1b818-188">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1b818-188">passwordMinimumLength</span></span>|<span data-ttu-id="1b818-189">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-189">Int32</span></span>|<span data-ttu-id="1b818-190">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="1b818-190">Minimum length of passwords.</span></span>|
|<span data-ttu-id="1b818-191">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1b818-191">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1b818-192">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-192">Int32</span></span>|<span data-ttu-id="1b818-193">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="1b818-193">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="1b818-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1b818-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1b818-195">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-195">Int32</span></span>|<span data-ttu-id="1b818-196">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="1b818-196">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="1b818-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1b818-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1b818-198">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-198">Int32</span></span>|<span data-ttu-id="1b818-199">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="1b818-199">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="1b818-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1b818-200">passwordRequiredType</span></span>|[<span data-ttu-id="1b818-201">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1b818-201">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1b818-202">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="1b818-202">Type of password that is required.</span></span> <span data-ttu-id="1b818-203">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1b818-203">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1b818-204">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1b818-204">passwordRequired</span></span>|<span data-ttu-id="1b818-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-205">Boolean</span></span>|<span data-ttu-id="1b818-206">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="1b818-206">Whether or not to require a password.</span></span>|
|<span data-ttu-id="1b818-207">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="1b818-207">keychainBlockCloudSync</span></span>|<span data-ttu-id="1b818-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-208">Boolean</span></span>|<span data-ttu-id="1b818-209">Gibt an, ob die iCloud-Schlüsselbund Synchronisierung blockiert ist (macOS 10,12 und höher).</span><span class="sxs-lookup"><span data-stu-id="1b818-209">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="1b818-210">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="1b818-210">airPrintBlocked</span></span>|<span data-ttu-id="1b818-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-211">Boolean</span></span>|<span data-ttu-id="1b818-212">Gibt an, ob der druckDruck blockiert ist (macOS 10,12 und höher).</span><span class="sxs-lookup"><span data-stu-id="1b818-212">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="1b818-213">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="1b818-213">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="1b818-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-214">Boolean</span></span>|<span data-ttu-id="1b818-215">Gibt an, ob vertrauenswürdige Zertifikate für die TLS-Druckkommunikation erforderlich sind (macOS 10,13 und höher).</span><span class="sxs-lookup"><span data-stu-id="1b818-215">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="1b818-216">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="1b818-216">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="1b818-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-217">Boolean</span></span>|<span data-ttu-id="1b818-218">Gibt an, ob die iBeacon-Erkennung von Druckern blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="1b818-218">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="1b818-219">Dadurch wird verhindert, dass falsche druckfunk-Bluetooth-Baken für Netzwerkdatenverkehr von Phishing (macOS 10,3 und höher).</span><span class="sxs-lookup"><span data-stu-id="1b818-219">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="1b818-220">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="1b818-220">safariBlockAutofill</span></span>|<span data-ttu-id="1b818-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-221">Boolean</span></span>|<span data-ttu-id="1b818-222">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="1b818-222">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="1b818-223">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1b818-223">cameraBlocked</span></span>|<span data-ttu-id="1b818-224">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-224">Boolean</span></span>|<span data-ttu-id="1b818-225">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="1b818-225">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="1b818-226">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="1b818-226">iTunesBlockMusicService</span></span>|<span data-ttu-id="1b818-227">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-227">Boolean</span></span>|<span data-ttu-id="1b818-228">Gibt an, ob der Musikdienst blockiert und die Musik-app im klassischen Modus wiederhergestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-228">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="1b818-229">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="1b818-229">spotlightBlockInternetResults</span></span>|<span data-ttu-id="1b818-230">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-230">Boolean</span></span>|<span data-ttu-id="1b818-231">Gibt an, ob Spotlight die Rückgabe von Ergebnissen aus einer Internet Suche blockieren soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-231">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="1b818-232">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="1b818-232">keyboardBlockDictation</span></span>|<span data-ttu-id="1b818-233">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-233">Boolean</span></span>|<span data-ttu-id="1b818-234">Gibt an, ob die Verwendung der Diktat Eingabe durch den Benutzer blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-234">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="1b818-235">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="1b818-235">definitionLookupBlocked</span></span>|<span data-ttu-id="1b818-236">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-236">Boolean</span></span>|<span data-ttu-id="1b818-237">Gibt an, ob die Definitions Suche blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-237">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="1b818-238">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="1b818-238">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="1b818-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-239">Boolean</span></span>|<span data-ttu-id="1b818-240">Gibt an, ob Benutzer das Aufheben der Sperre für Ihren Mac mit Apple Watch blockieren möchten.</span><span class="sxs-lookup"><span data-stu-id="1b818-240">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="1b818-241">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="1b818-241">iTunesBlockFileSharing</span></span>|<span data-ttu-id="1b818-242">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-242">Boolean</span></span>|<span data-ttu-id="1b818-243">Gibt an, ob das Übertragen von Dateien mithilfe von iTunes verhindert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-243">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="1b818-244">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="1b818-244">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="1b818-245">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-245">Boolean</span></span>|<span data-ttu-id="1b818-246">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-246">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="1b818-247">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="1b818-247">iCloudBlockMail</span></span>|<span data-ttu-id="1b818-248">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-248">Boolean</span></span>|<span data-ttu-id="1b818-249">Gibt an, ob die Synchronisierung von e-Mails durch iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-249">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="1b818-250">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="1b818-250">iCloudBlockAddressBook</span></span>|<span data-ttu-id="1b818-251">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-251">Boolean</span></span>|<span data-ttu-id="1b818-252">Gibt an, ob die Synchronisierung von Kontakten durch iCloud verhindert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-252">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="1b818-253">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="1b818-253">iCloudBlockCalendar</span></span>|<span data-ttu-id="1b818-254">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-254">Boolean</span></span>|<span data-ttu-id="1b818-255">Gibt an, ob das Synchronisieren von Kalendern für iCloud verhindert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-255">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="1b818-256">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="1b818-256">iCloudBlockReminders</span></span>|<span data-ttu-id="1b818-257">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-257">Boolean</span></span>|<span data-ttu-id="1b818-258">Gibt an, ob das Synchronisieren von Erinnerungen durch iCloud verhindert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-258">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="1b818-259">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="1b818-259">iCloudBlockBookmarks</span></span>|<span data-ttu-id="1b818-260">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-260">Boolean</span></span>|<span data-ttu-id="1b818-261">Gibt an, ob das Synchronisieren von Textmarken durch iCloud verhindert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-261">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="1b818-262">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="1b818-262">iCloudBlockNotes</span></span>|<span data-ttu-id="1b818-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-263">Boolean</span></span>|<span data-ttu-id="1b818-264">Gibt an, ob das Synchronisieren von Notizen durch iCloud verhindert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-264">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="1b818-265">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="1b818-265">airDropBlocked</span></span>|<span data-ttu-id="1b818-266">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-266">Boolean</span></span>|<span data-ttu-id="1b818-267">Gibt an, ob das abLegen zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-267">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="1b818-268">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="1b818-268">passwordBlockModification</span></span>|<span data-ttu-id="1b818-269">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-269">Boolean</span></span>|<span data-ttu-id="1b818-270">Gibt an, ob die Änderung von Passwörtern zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="1b818-270">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="1b818-271">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1b818-271">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1b818-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b818-272">Boolean</span></span>|<span data-ttu-id="1b818-273">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-273">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1b818-274">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="1b818-274">passwordBlockAutoFill</span></span>|<span data-ttu-id="1b818-275">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-275">Boolean</span></span>|<span data-ttu-id="1b818-276">Gibt an, ob das Feature AutoFill passwords blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-276">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="1b818-277">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="1b818-277">passwordBlockProximityRequests</span></span>|<span data-ttu-id="1b818-278">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-278">Boolean</span></span>|<span data-ttu-id="1b818-279">Gibt an, ob das Anfordern von Kennwörtern von benachbarten Geräten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-279">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="1b818-280">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="1b818-280">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="1b818-281">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-281">Boolean</span></span>|<span data-ttu-id="1b818-282">Gibt an, ob das Freigeben von Kennwörtern mit der Funktion für Kennwörter blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b818-282">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="1b818-283">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="1b818-283">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="1b818-284">Int32</span><span class="sxs-lookup"><span data-stu-id="1b818-284">Int32</span></span>|<span data-ttu-id="1b818-285">Legt fest, wie viele Tage ein Software Update für ein überwachte Gerät delyed wird.</span><span class="sxs-lookup"><span data-stu-id="1b818-285">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="1b818-286">Gültige Werte: 0 bis 90.</span><span class="sxs-lookup"><span data-stu-id="1b818-286">Valid values 0 to 90</span></span>|
|<span data-ttu-id="1b818-287">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="1b818-287">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="1b818-288">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-288">Boolean</span></span>|<span data-ttu-id="1b818-289">Gibt an, ob die Benutzersicht barkeit von Softwareupdates verzögert werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="1b818-289">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1b818-290">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="1b818-290">contentCachingBlocked</span></span>|<span data-ttu-id="1b818-291">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b818-291">Boolean</span></span>|<span data-ttu-id="1b818-292">Gibt an, ob das Zwischenspeichern von Inhalten zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="1b818-292">Indicates whether or not to allow content caching.</span></span>|



## <a name="response"></a><span data-ttu-id="1b818-293">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b818-293">Response</span></span>
<span data-ttu-id="1b818-294">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1b818-294">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b818-295">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b818-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b818-296">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b818-296">Request</span></span>
<span data-ttu-id="1b818-297">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b818-297">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="1b818-298">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b818-298">Response</span></span>
<span data-ttu-id="1b818-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b818-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true
}
```




