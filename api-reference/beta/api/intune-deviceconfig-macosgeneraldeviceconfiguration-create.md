---
title: Erstellen von „macOSGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6dd521646246914508a24f4c9188defff04bad9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406514"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="13580-103">Erstellen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="13580-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="13580-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="13580-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13580-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13580-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13580-107">Diese Methode erstellt ein neues Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13580-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13580-108">Prerequisites</span></span>
<span data-ttu-id="13580-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13580-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13580-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13580-111">Permission type</span></span>|<span data-ttu-id="13580-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13580-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13580-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13580-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13580-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13580-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13580-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13580-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13580-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13580-116">Not supported.</span></span>|
|<span data-ttu-id="13580-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13580-117">Application</span></span>|<span data-ttu-id="13580-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13580-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13580-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13580-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13580-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13580-120">Request headers</span></span>
|<span data-ttu-id="13580-121">Header</span><span class="sxs-lookup"><span data-stu-id="13580-121">Header</span></span>|<span data-ttu-id="13580-122">Wert</span><span class="sxs-lookup"><span data-stu-id="13580-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13580-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="13580-123">Authorization</span></span>|<span data-ttu-id="13580-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13580-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13580-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="13580-125">Accept</span></span>|<span data-ttu-id="13580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13580-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13580-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13580-127">Request body</span></span>
<span data-ttu-id="13580-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="13580-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="13580-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="13580-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="13580-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13580-130">Property</span></span>|<span data-ttu-id="13580-131">Typ</span><span class="sxs-lookup"><span data-stu-id="13580-131">Type</span></span>|<span data-ttu-id="13580-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13580-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13580-133">id</span><span class="sxs-lookup"><span data-stu-id="13580-133">id</span></span>|<span data-ttu-id="13580-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13580-134">String</span></span>|<span data-ttu-id="13580-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="13580-135">Key of the entity.</span></span> <span data-ttu-id="13580-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13580-137">lastModifiedDateTime</span></span>|<span data-ttu-id="13580-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13580-138">DateTimeOffset</span></span>|<span data-ttu-id="13580-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="13580-139">DateTime the object was last modified.</span></span> <span data-ttu-id="13580-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13580-141">roleScopeTagIds</span></span>|<span data-ttu-id="13580-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="13580-142">String collection</span></span>|<span data-ttu-id="13580-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="13580-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13580-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="13580-145">supportsScopeTags</span></span>|<span data-ttu-id="13580-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-146">Boolean</span></span>|<span data-ttu-id="13580-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13580-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="13580-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="13580-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="13580-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="13580-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="13580-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13580-150">This property is read-only.</span></span> <span data-ttu-id="13580-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13580-152">createdDateTime</span></span>|<span data-ttu-id="13580-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13580-153">DateTimeOffset</span></span>|<span data-ttu-id="13580-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="13580-154">DateTime the object was created.</span></span> <span data-ttu-id="13580-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-156">description</span><span class="sxs-lookup"><span data-stu-id="13580-156">description</span></span>|<span data-ttu-id="13580-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13580-157">String</span></span>|<span data-ttu-id="13580-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="13580-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13580-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-160">displayName</span><span class="sxs-lookup"><span data-stu-id="13580-160">displayName</span></span>|<span data-ttu-id="13580-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13580-161">String</span></span>|<span data-ttu-id="13580-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="13580-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13580-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-164">Version</span><span class="sxs-lookup"><span data-stu-id="13580-164">version</span></span>|<span data-ttu-id="13580-165">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-165">Int32</span></span>|<span data-ttu-id="13580-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="13580-166">Version of the device configuration.</span></span> <span data-ttu-id="13580-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13580-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13580-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="13580-168">compliantAppsList</span></span>|<span data-ttu-id="13580-169">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="13580-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="13580-170">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="13580-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="13580-171">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="13580-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="13580-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="13580-172">compliantAppListType</span></span>|[<span data-ttu-id="13580-173">appListType</span><span class="sxs-lookup"><span data-stu-id="13580-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="13580-174">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="13580-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="13580-175">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="13580-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="13580-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="13580-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="13580-177">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="13580-177">String collection</span></span>|<span data-ttu-id="13580-178">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="13580-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="13580-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="13580-179">passwordBlockSimple</span></span>|<span data-ttu-id="13580-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-180">Boolean</span></span>|<span data-ttu-id="13580-181">Unterbindet die Verwendung einfacher Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="13580-181">Block simple passwords.</span></span>|
|<span data-ttu-id="13580-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="13580-182">passwordExpirationDays</span></span>|<span data-ttu-id="13580-183">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-183">Int32</span></span>|<span data-ttu-id="13580-184">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="13580-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="13580-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="13580-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="13580-186">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-186">Int32</span></span>|<span data-ttu-id="13580-187">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss.</span><span class="sxs-lookup"><span data-stu-id="13580-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="13580-188">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="13580-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="13580-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="13580-189">passwordMinimumLength</span></span>|<span data-ttu-id="13580-190">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-190">Int32</span></span>|<span data-ttu-id="13580-191">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="13580-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="13580-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="13580-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="13580-193">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-193">Int32</span></span>|<span data-ttu-id="13580-194">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="13580-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="13580-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="13580-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="13580-196">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-196">Int32</span></span>|<span data-ttu-id="13580-197">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="13580-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="13580-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="13580-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="13580-199">Int32</span><span class="sxs-lookup"><span data-stu-id="13580-199">Int32</span></span>|<span data-ttu-id="13580-200">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="13580-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="13580-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="13580-201">passwordRequiredType</span></span>|[<span data-ttu-id="13580-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="13580-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="13580-203">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="13580-203">Type of password that is required.</span></span> <span data-ttu-id="13580-204">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="13580-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="13580-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="13580-205">passwordRequired</span></span>|<span data-ttu-id="13580-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-206">Boolean</span></span>|<span data-ttu-id="13580-207">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="13580-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="13580-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="13580-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="13580-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-209">Boolean</span></span>|<span data-ttu-id="13580-210">Gibt an, ob iCloud Schlüsselsammlung Synchronisierung blockierte (Mac OS 10.12 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="13580-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="13580-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="13580-211">airPrintBlocked</span></span>|<span data-ttu-id="13580-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-212">Boolean</span></span>|<span data-ttu-id="13580-213">Gibt an, ob AirPrint blockierte (Mac OS 10.12 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="13580-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="13580-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="13580-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="13580-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-215">Boolean</span></span>|<span data-ttu-id="13580-216">Gibt an, ob vertrauenswürdige Zertifikate für Drucken TLS-Kommunikation (Mac OS 10.13 und höher) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="13580-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="13580-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="13580-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="13580-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-218">Boolean</span></span>|<span data-ttu-id="13580-219">Gibt an, ob iBeacon Ermittlung von AirPrint Drucker ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="13580-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="13580-220">Dies verhindert, dass falsche AirPrint Bluetooth Beacons vor Phishing für den Netzwerkdatenverkehr (Mac OS 10.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="13580-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="13580-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="13580-221">safariBlockAutofill</span></span>|<span data-ttu-id="13580-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-222">Boolean</span></span>|<span data-ttu-id="13580-223">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="13580-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="13580-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="13580-224">cameraBlocked</span></span>|<span data-ttu-id="13580-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-225">Boolean</span></span>|<span data-ttu-id="13580-226">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="13580-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="13580-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="13580-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="13580-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-228">Boolean</span></span>|<span data-ttu-id="13580-229">Gibt an, ob Musik Service blockieren und Musik-app im klassischen Modus zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="13580-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="13580-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="13580-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="13580-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-231">Boolean</span></span>|<span data-ttu-id="13580-232">Gibt an, ob Spotlight blockieren aus einer Internet-Suche Ergebnisse zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13580-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="13580-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="13580-233">keyboardBlockDictation</span></span>|<span data-ttu-id="13580-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-234">Boolean</span></span>|<span data-ttu-id="13580-235">Gibt an, ob die Benutzer mit Dictation Input blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="13580-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="13580-236">definitionLookupBlocked</span></span>|<span data-ttu-id="13580-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-237">Boolean</span></span>|<span data-ttu-id="13580-238">Gibt an, ob Definition Lookup blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="13580-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="13580-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="13580-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-240">Boolean</span></span>|<span data-ttu-id="13580-241">Gibt an, ob oder blockieren Benutzer ihre Mac mit Apple Watch entsperren.</span><span class="sxs-lookup"><span data-stu-id="13580-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="13580-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="13580-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="13580-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-243">Boolean</span></span>|<span data-ttu-id="13580-244">Gibt an, ob Dateien verhindern blockieren übertragen iTunes verwenden.</span><span class="sxs-lookup"><span data-stu-id="13580-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="13580-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="13580-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="13580-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-246">Boolean</span></span>|<span data-ttu-id="13580-247">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="13580-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="13580-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="13580-248">iCloudBlockMail</span></span>|<span data-ttu-id="13580-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-249">Boolean</span></span>|<span data-ttu-id="13580-250">Gibt an, ob iCloud aus der Synchronisierung von e-Mail-Nachrichten zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="13580-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="13580-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="13580-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-252">Boolean</span></span>|<span data-ttu-id="13580-253">Gibt an, ob iCloud aus der Synchronisierung von Kontakten zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="13580-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="13580-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="13580-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-255">Boolean</span></span>|<span data-ttu-id="13580-256">Gibt an, ob iCloud aus der Synchronisierung von Kalendern blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="13580-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="13580-257">iCloudBlockReminders</span></span>|<span data-ttu-id="13580-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-258">Boolean</span></span>|<span data-ttu-id="13580-259">Gibt an, ob iCloud aus der Synchronisierung Erinnerungen blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="13580-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="13580-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="13580-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-261">Boolean</span></span>|<span data-ttu-id="13580-262">Gibt an, ob iCloud von Lesezeichen synchronisieren blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="13580-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="13580-263">iCloudBlockNotes</span></span>|<span data-ttu-id="13580-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-264">Boolean</span></span>|<span data-ttu-id="13580-265">Gibt an, ob iCloud aus der Synchronisierung von Notizen zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="13580-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="13580-266">airDropBlocked</span></span>|<span data-ttu-id="13580-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-267">Boolean</span></span>|<span data-ttu-id="13580-268">Gibt an, ob AirDrop zulassen.</span><span class="sxs-lookup"><span data-stu-id="13580-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="13580-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="13580-269">passwordBlockModification</span></span>|<span data-ttu-id="13580-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-270">Boolean</span></span>|<span data-ttu-id="13580-271">Gibt an, ob Kennung für die Änderung zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="13580-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="13580-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="13580-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="13580-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-273">Boolean</span></span>|<span data-ttu-id="13580-274">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="13580-274">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="13580-275">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="13580-275">passwordBlockAutoFill</span></span>|<span data-ttu-id="13580-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-276">Boolean</span></span>|<span data-ttu-id="13580-277">Gibt an, ob das Feature AutoAusfüllen-Kennwörter zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-277">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="13580-278">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="13580-278">passwordBlockProximityRequests</span></span>|<span data-ttu-id="13580-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-279">Boolean</span></span>|<span data-ttu-id="13580-280">Gibt an, ob anfordernde Kennwörter von Geräten in der Nähe zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-280">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="13580-281">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="13580-281">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="13580-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="13580-282">Boolean</span></span>|<span data-ttu-id="13580-283">Gibt an, ob sharing Kennwörter mit dem AirDrop Kennwörter Feature blockieren.</span><span class="sxs-lookup"><span data-stu-id="13580-283">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|



## <a name="response"></a><span data-ttu-id="13580-284">Antwort</span><span class="sxs-lookup"><span data-stu-id="13580-284">Response</span></span>
<span data-ttu-id="13580-285">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13580-285">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13580-286">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13580-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="13580-287">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13580-287">Request</span></span>
<span data-ttu-id="13580-288">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13580-288">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1870

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
  "passwordBlockAirDropSharing": true
}
```

### <a name="response"></a><span data-ttu-id="13580-289">Antwort</span><span class="sxs-lookup"><span data-stu-id="13580-289">Response</span></span>
<span data-ttu-id="13580-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13580-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2042

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
  "passwordBlockAirDropSharing": true
}
```




