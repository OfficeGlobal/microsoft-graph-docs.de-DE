---
title: Erstellen von „macOSGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3cdd25bc23c59ab073e6ac540c7e81a5802eaf65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969163"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="08e8d-103">Erstellen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="08e8d-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="08e8d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08e8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08e8d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08e8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08e8d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="08e8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08e8d-107">Diese Methode erstellt ein neues Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08e8d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08e8d-108">Prerequisites</span></span>
<span data-ttu-id="08e8d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08e8d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08e8d-111">Permission type</span></span>|<span data-ttu-id="08e8d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08e8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08e8d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08e8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08e8d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e8d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08e8d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08e8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08e8d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e8d-116">Not supported.</span></span>|
|<span data-ttu-id="08e8d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08e8d-117">Application</span></span>|<span data-ttu-id="08e8d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e8d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08e8d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="08e8d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08e8d-120">Request headers</span></span>
|<span data-ttu-id="08e8d-121">Header</span><span class="sxs-lookup"><span data-stu-id="08e8d-121">Header</span></span>|<span data-ttu-id="08e8d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08e8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08e8d-123">Authorization</span></span>|<span data-ttu-id="08e8d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08e8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08e8d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08e8d-125">Accept</span></span>|<span data-ttu-id="08e8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08e8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08e8d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08e8d-127">Request body</span></span>
<span data-ttu-id="08e8d-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="08e8d-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="08e8d-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="08e8d-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="08e8d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08e8d-130">Property</span></span>|<span data-ttu-id="08e8d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="08e8d-131">Type</span></span>|<span data-ttu-id="08e8d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e8d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e8d-133">id</span><span class="sxs-lookup"><span data-stu-id="08e8d-133">id</span></span>|<span data-ttu-id="08e8d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e8d-134">String</span></span>|<span data-ttu-id="08e8d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="08e8d-135">Key of the entity.</span></span> <span data-ttu-id="08e8d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08e8d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="08e8d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08e8d-138">DateTimeOffset</span></span>|<span data-ttu-id="08e8d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="08e8d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="08e8d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08e8d-141">roleScopeTagIds</span></span>|<span data-ttu-id="08e8d-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="08e8d-142">String collection</span></span>|<span data-ttu-id="08e8d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="08e8d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08e8d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="08e8d-145">supportsScopeTags</span></span>|<span data-ttu-id="08e8d-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-146">Boolean</span></span>|<span data-ttu-id="08e8d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08e8d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08e8d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="08e8d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08e8d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="08e8d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08e8d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08e8d-150">This property is read-only.</span></span> <span data-ttu-id="08e8d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08e8d-152">createdDateTime</span></span>|<span data-ttu-id="08e8d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08e8d-153">DateTimeOffset</span></span>|<span data-ttu-id="08e8d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="08e8d-154">DateTime the object was created.</span></span> <span data-ttu-id="08e8d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-156">description</span><span class="sxs-lookup"><span data-stu-id="08e8d-156">description</span></span>|<span data-ttu-id="08e8d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e8d-157">String</span></span>|<span data-ttu-id="08e8d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="08e8d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08e8d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="08e8d-160">displayName</span></span>|<span data-ttu-id="08e8d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e8d-161">String</span></span>|<span data-ttu-id="08e8d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="08e8d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08e8d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-164">Version</span><span class="sxs-lookup"><span data-stu-id="08e8d-164">version</span></span>|<span data-ttu-id="08e8d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-165">Int32</span></span>|<span data-ttu-id="08e8d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="08e8d-166">Version of the device configuration.</span></span> <span data-ttu-id="08e8d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08e8d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08e8d-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="08e8d-168">compliantAppsList</span></span>|<span data-ttu-id="08e8d-169">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="08e8d-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="08e8d-170">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="08e8d-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="08e8d-171">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="08e8d-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="08e8d-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="08e8d-172">compliantAppListType</span></span>|[<span data-ttu-id="08e8d-173">appListType</span><span class="sxs-lookup"><span data-stu-id="08e8d-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="08e8d-174">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="08e8d-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="08e8d-175">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="08e8d-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="08e8d-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="08e8d-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="08e8d-177">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="08e8d-177">String collection</span></span>|<span data-ttu-id="08e8d-178">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="08e8d-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="08e8d-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="08e8d-179">passwordBlockSimple</span></span>|<span data-ttu-id="08e8d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e8d-180">Boolean</span></span>|<span data-ttu-id="08e8d-181">Unterbindet die Verwendung einfacher Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="08e8d-181">Block simple passwords.</span></span>|
|<span data-ttu-id="08e8d-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="08e8d-182">passwordExpirationDays</span></span>|<span data-ttu-id="08e8d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-183">Int32</span></span>|<span data-ttu-id="08e8d-184">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="08e8d-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="08e8d-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="08e8d-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="08e8d-186">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-186">Int32</span></span>|<span data-ttu-id="08e8d-187">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss.</span><span class="sxs-lookup"><span data-stu-id="08e8d-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="08e8d-188">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="08e8d-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="08e8d-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="08e8d-189">passwordMinimumLength</span></span>|<span data-ttu-id="08e8d-190">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-190">Int32</span></span>|<span data-ttu-id="08e8d-191">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="08e8d-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="08e8d-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="08e8d-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="08e8d-193">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-193">Int32</span></span>|<span data-ttu-id="08e8d-194">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="08e8d-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="08e8d-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="08e8d-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="08e8d-196">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-196">Int32</span></span>|<span data-ttu-id="08e8d-197">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="08e8d-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="08e8d-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="08e8d-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="08e8d-199">Int32</span><span class="sxs-lookup"><span data-stu-id="08e8d-199">Int32</span></span>|<span data-ttu-id="08e8d-200">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="08e8d-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="08e8d-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="08e8d-201">passwordRequiredType</span></span>|[<span data-ttu-id="08e8d-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="08e8d-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="08e8d-203">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="08e8d-203">Type of password that is required.</span></span> <span data-ttu-id="08e8d-204">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="08e8d-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="08e8d-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="08e8d-205">passwordRequired</span></span>|<span data-ttu-id="08e8d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e8d-206">Boolean</span></span>|<span data-ttu-id="08e8d-207">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="08e8d-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="08e8d-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="08e8d-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="08e8d-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-209">Boolean</span></span>|<span data-ttu-id="08e8d-210">Gibt an, ob iCloud Schlüsselsammlung Synchronisierung blockierte (Mac OS 10.12 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="08e8d-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="08e8d-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="08e8d-211">airPrintBlocked</span></span>|<span data-ttu-id="08e8d-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-212">Boolean</span></span>|<span data-ttu-id="08e8d-213">Gibt an, ob AirPrint blockierte (Mac OS 10.12 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="08e8d-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="08e8d-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="08e8d-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="08e8d-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-215">Boolean</span></span>|<span data-ttu-id="08e8d-216">Gibt an, ob vertrauenswürdige Zertifikate für Drucken TLS-Kommunikation (Mac OS 10.13 und höher) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="08e8d-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="08e8d-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="08e8d-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="08e8d-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-218">Boolean</span></span>|<span data-ttu-id="08e8d-219">Gibt an, ob iBeacon Ermittlung von AirPrint Drucker ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="08e8d-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="08e8d-220">Dies verhindert, dass falsche AirPrint Bluetooth Beacons vor Phishing für den Netzwerkdatenverkehr (Mac OS 10.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="08e8d-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="08e8d-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="08e8d-221">safariBlockAutofill</span></span>|<span data-ttu-id="08e8d-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-222">Boolean</span></span>|<span data-ttu-id="08e8d-223">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="08e8d-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="08e8d-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="08e8d-224">cameraBlocked</span></span>|<span data-ttu-id="08e8d-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-225">Boolean</span></span>|<span data-ttu-id="08e8d-226">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="08e8d-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="08e8d-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="08e8d-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="08e8d-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-228">Boolean</span></span>|<span data-ttu-id="08e8d-229">Gibt an, ob Musik Service blockieren und Musik-app im klassischen Modus zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="08e8d-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="08e8d-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="08e8d-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="08e8d-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-231">Boolean</span></span>|<span data-ttu-id="08e8d-232">Gibt an, ob Spotlight blockieren aus einer Internet-Suche Ergebnisse zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08e8d-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="08e8d-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="08e8d-233">keyboardBlockDictation</span></span>|<span data-ttu-id="08e8d-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-234">Boolean</span></span>|<span data-ttu-id="08e8d-235">Gibt an, ob die Benutzer mit Dictation Input blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="08e8d-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="08e8d-236">definitionLookupBlocked</span></span>|<span data-ttu-id="08e8d-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-237">Boolean</span></span>|<span data-ttu-id="08e8d-238">Gibt an, ob Definition Lookup blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="08e8d-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="08e8d-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="08e8d-240">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-240">Boolean</span></span>|<span data-ttu-id="08e8d-241">Gibt an, ob oder blockieren Benutzer ihre Mac mit Apple Watch entsperren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="08e8d-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="08e8d-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="08e8d-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-243">Boolean</span></span>|<span data-ttu-id="08e8d-244">Gibt an, ob Dateien verhindern blockieren übertragen iTunes verwenden.</span><span class="sxs-lookup"><span data-stu-id="08e8d-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="08e8d-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="08e8d-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="08e8d-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-246">Boolean</span></span>|<span data-ttu-id="08e8d-247">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="08e8d-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="08e8d-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="08e8d-248">iCloudBlockMail</span></span>|<span data-ttu-id="08e8d-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-249">Boolean</span></span>|<span data-ttu-id="08e8d-250">Gibt an, ob iCloud aus der Synchronisierung von e-Mail-Nachrichten zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="08e8d-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="08e8d-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="08e8d-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-252">Boolean</span></span>|<span data-ttu-id="08e8d-253">Gibt an, ob iCloud aus der Synchronisierung von Kontakten zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="08e8d-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="08e8d-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="08e8d-255">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-255">Boolean</span></span>|<span data-ttu-id="08e8d-256">Gibt an, ob iCloud aus der Synchronisierung von Kalendern blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="08e8d-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="08e8d-257">iCloudBlockReminders</span></span>|<span data-ttu-id="08e8d-258">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-258">Boolean</span></span>|<span data-ttu-id="08e8d-259">Gibt an, ob iCloud aus der Synchronisierung Erinnerungen blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="08e8d-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="08e8d-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="08e8d-261">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-261">Boolean</span></span>|<span data-ttu-id="08e8d-262">Gibt an, ob iCloud von Lesezeichen synchronisieren blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="08e8d-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="08e8d-263">iCloudBlockNotes</span></span>|<span data-ttu-id="08e8d-264">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-264">Boolean</span></span>|<span data-ttu-id="08e8d-265">Gibt an, ob iCloud aus der Synchronisierung von Notizen zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="08e8d-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="08e8d-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="08e8d-266">airDropBlocked</span></span>|<span data-ttu-id="08e8d-267">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-267">Boolean</span></span>|<span data-ttu-id="08e8d-268">Gibt an, ob AirDrop zulassen.</span><span class="sxs-lookup"><span data-stu-id="08e8d-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="08e8d-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="08e8d-269">passwordBlockModification</span></span>|<span data-ttu-id="08e8d-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-270">Boolean</span></span>|<span data-ttu-id="08e8d-271">Gibt an, ob Kennung für die Änderung zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="08e8d-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="08e8d-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="08e8d-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="08e8d-273">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08e8d-273">Boolean</span></span>|<span data-ttu-id="08e8d-274">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="08e8d-274">Indicates whether or not to block fingerprint unlock.</span></span>|



## <a name="response"></a><span data-ttu-id="08e8d-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e8d-275">Response</span></span>
<span data-ttu-id="08e8d-276">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="08e8d-276">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e8d-277">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08e8d-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="08e8d-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e8d-278">Request</span></span>
<span data-ttu-id="08e8d-279">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08e8d-279">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1817

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "passwordBlockFingerprintUnlock": true
}
```

### <a name="response"></a><span data-ttu-id="08e8d-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e8d-280">Response</span></span>
<span data-ttu-id="08e8d-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08e8d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1925

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
  "passwordBlockFingerprintUnlock": true
}
```





