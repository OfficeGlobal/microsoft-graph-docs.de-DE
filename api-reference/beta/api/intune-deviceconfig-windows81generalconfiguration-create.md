---
title: Erstellen von „windows81GeneralConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6d48a4d1426c05993639b8662af8a1e605124e3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965942"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="ea003-103">Erstellen von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ea003-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="ea003-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea003-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea003-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ea003-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea003-106">Diese Methode erstellt ein neues Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea003-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea003-107">Prerequisites</span></span>
<span data-ttu-id="ea003-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea003-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea003-110">Permission type</span></span>|<span data-ttu-id="ea003-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea003-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea003-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea003-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea003-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea003-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea003-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea003-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea003-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea003-115">Not supported.</span></span>|
|<span data-ttu-id="ea003-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea003-116">Application</span></span>|<span data-ttu-id="ea003-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea003-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea003-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea003-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ea003-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea003-119">Request headers</span></span>
|<span data-ttu-id="ea003-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea003-120">Header</span></span>|<span data-ttu-id="ea003-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea003-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea003-122">Authorization</span></span>|<span data-ttu-id="ea003-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea003-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea003-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea003-124">Accept</span></span>|<span data-ttu-id="ea003-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea003-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea003-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea003-126">Request body</span></span>
<span data-ttu-id="ea003-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="ea003-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="ea003-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ea003-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="ea003-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea003-129">Property</span></span>|<span data-ttu-id="ea003-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ea003-130">Type</span></span>|<span data-ttu-id="ea003-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea003-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea003-132">id</span><span class="sxs-lookup"><span data-stu-id="ea003-132">id</span></span>|<span data-ttu-id="ea003-133">String</span><span class="sxs-lookup"><span data-stu-id="ea003-133">String</span></span>|<span data-ttu-id="ea003-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ea003-134">Key of the entity.</span></span> <span data-ttu-id="ea003-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea003-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ea003-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea003-137">DateTimeOffset</span></span>|<span data-ttu-id="ea003-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea003-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ea003-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ea003-140">roleScopeTagIds</span></span>|<span data-ttu-id="ea003-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ea003-141">String collection</span></span>|<span data-ttu-id="ea003-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ea003-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ea003-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ea003-144">supportsScopeTags</span></span>|<span data-ttu-id="ea003-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-145">Boolean</span></span>|<span data-ttu-id="ea003-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea003-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ea003-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="ea003-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ea003-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ea003-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ea003-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ea003-149">This property is read-only.</span></span> <span data-ttu-id="ea003-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea003-151">createdDateTime</span></span>|<span data-ttu-id="ea003-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea003-152">DateTimeOffset</span></span>|<span data-ttu-id="ea003-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea003-153">DateTime the object was created.</span></span> <span data-ttu-id="ea003-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-155">description</span><span class="sxs-lookup"><span data-stu-id="ea003-155">description</span></span>|<span data-ttu-id="ea003-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea003-156">String</span></span>|<span data-ttu-id="ea003-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ea003-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea003-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ea003-159">displayName</span></span>|<span data-ttu-id="ea003-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea003-160">String</span></span>|<span data-ttu-id="ea003-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ea003-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea003-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea003-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-163">Version</span><span class="sxs-lookup"><span data-stu-id="ea003-163">version</span></span>|<span data-ttu-id="ea003-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-164">Int32</span></span>|<span data-ttu-id="ea003-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea003-165">Version of the device configuration.</span></span> <span data-ttu-id="ea003-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea003-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea003-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="ea003-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="ea003-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-168">Boolean</span></span>|<span data-ttu-id="ea003-169">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="ea003-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="ea003-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ea003-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="ea003-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-171">Boolean</span></span>|<span data-ttu-id="ea003-172">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="ea003-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ea003-173">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ea003-173">This property is read-only.</span></span>|
|<span data-ttu-id="ea003-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ea003-174">browserBlockAutofill</span></span>|<span data-ttu-id="ea003-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-175">Boolean</span></span>|<span data-ttu-id="ea003-176">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="ea003-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ea003-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="ea003-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-178">Boolean</span></span>|<span data-ttu-id="ea003-179">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="ea003-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="ea003-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="ea003-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-181">Boolean</span></span>|<span data-ttu-id="ea003-182">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="ea003-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ea003-183">browserBlockJavaScript</span></span>|<span data-ttu-id="ea003-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-184">Boolean</span></span>|<span data-ttu-id="ea003-185">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="ea003-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="ea003-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="ea003-186">browserBlockPlugins</span></span>|<span data-ttu-id="ea003-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-187">Boolean</span></span>|<span data-ttu-id="ea003-188">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ea003-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="ea003-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ea003-189">browserBlockPopups</span></span>|<span data-ttu-id="ea003-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-190">Boolean</span></span>|<span data-ttu-id="ea003-191">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ea003-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="ea003-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="ea003-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="ea003-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-193">Boolean</span></span>|<span data-ttu-id="ea003-194">Gibt an, ob verhindert werden soll, dass der Benutzer die Kopfzeile „Do Not Track“ (nicht verfolgen) sendet.</span><span class="sxs-lookup"><span data-stu-id="ea003-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="ea003-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ea003-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="ea003-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-196">Boolean</span></span>|<span data-ttu-id="ea003-197">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ea003-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="ea003-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="ea003-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="ea003-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-199">Boolean</span></span>|<span data-ttu-id="ea003-200">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="ea003-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="ea003-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="ea003-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="ea003-202">String</span><span class="sxs-lookup"><span data-stu-id="ea003-202">String</span></span>|<span data-ttu-id="ea003-203">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="ea003-203">The enterprise mode site list location.</span></span> <span data-ttu-id="ea003-204">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein http-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="ea003-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="ea003-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ea003-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="ea003-206">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ea003-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="ea003-207">Internetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="ea003-207">The internet security level.</span></span> <span data-ttu-id="ea003-208">Mögliche Werte sind: `userDefined`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="ea003-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ea003-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ea003-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="ea003-210">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ea003-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ea003-211">Intranetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="ea003-211">The Intranet security level.</span></span> <span data-ttu-id="ea003-212">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="ea003-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ea003-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="ea003-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="ea003-214">String</span><span class="sxs-lookup"><span data-stu-id="ea003-214">String</span></span>|<span data-ttu-id="ea003-215">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="ea003-215">The logging report location.</span></span>|
|<span data-ttu-id="ea003-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="ea003-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="ea003-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-217">Boolean</span></span>|<span data-ttu-id="ea003-218">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="ea003-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="ea003-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="ea003-219">browserRequireFirewall</span></span>|<span data-ttu-id="ea003-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-220">Boolean</span></span>|<span data-ttu-id="ea003-221">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ea003-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="ea003-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ea003-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="ea003-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea003-223">Boolean</span></span>|<span data-ttu-id="ea003-224">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ea003-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="ea003-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ea003-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="ea003-226">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ea003-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ea003-227">Sicherheitsstufe für vertrauenswürdige Websites.</span><span class="sxs-lookup"><span data-stu-id="ea003-227">The trusted sites security level.</span></span> <span data-ttu-id="ea003-228">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="ea003-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ea003-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ea003-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ea003-230">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-230">Boolean</span></span>|<span data-ttu-id="ea003-231">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ea003-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="ea003-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="ea003-233">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-233">Boolean</span></span>|<span data-ttu-id="ea003-234">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ea003-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="ea003-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="ea003-236">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-236">Boolean</span></span>|<span data-ttu-id="ea003-237">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="ea003-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="ea003-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ea003-238">passwordExpirationDays</span></span>|<span data-ttu-id="ea003-239">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-239">Int32</span></span>|<span data-ttu-id="ea003-240">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="ea003-240">Password expiration in days.</span></span>|
|<span data-ttu-id="ea003-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ea003-241">passwordMinimumLength</span></span>|<span data-ttu-id="ea003-242">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-242">Int32</span></span>|<span data-ttu-id="ea003-243">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="ea003-243">The minimum password length.</span></span>|
|<span data-ttu-id="ea003-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ea003-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ea003-245">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-245">Int32</span></span>|<span data-ttu-id="ea003-246">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="ea003-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ea003-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ea003-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ea003-248">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-248">Int32</span></span>|<span data-ttu-id="ea003-249">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="ea003-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ea003-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ea003-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ea003-251">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-251">Int32</span></span>|<span data-ttu-id="ea003-252">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="ea003-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="ea003-253">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="ea003-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ea003-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ea003-254">passwordRequiredType</span></span>|[<span data-ttu-id="ea003-255">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ea003-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ea003-256">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="ea003-256">The required password type.</span></span> <span data-ttu-id="ea003-257">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ea003-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ea003-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ea003-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ea003-259">Int32</span><span class="sxs-lookup"><span data-stu-id="ea003-259">Int32</span></span>|<span data-ttu-id="ea003-260">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="ea003-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="ea003-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="ea003-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="ea003-262">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ea003-262">Boolean</span></span>|<span data-ttu-id="ea003-263">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ea003-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="ea003-264">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="ea003-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="ea003-265">updateClassification</span><span class="sxs-lookup"><span data-stu-id="ea003-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="ea003-266">Die minimale Updateklassifizierung, die automatisch installiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="ea003-267">Mögliche Werte sind: `userDefined`, `recommendedAndImportant`, `important` und `none`.</span><span class="sxs-lookup"><span data-stu-id="ea003-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="ea003-268">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="ea003-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="ea003-269">updateClassification</span><span class="sxs-lookup"><span data-stu-id="ea003-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="ea003-270">Die minimale Updateklassifizierung, die automatisch installiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea003-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="ea003-271">Mögliche Werte sind: `userDefined`, `recommendedAndImportant`, `important` und `none`.</span><span class="sxs-lookup"><span data-stu-id="ea003-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="ea003-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="ea003-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="ea003-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea003-273">Boolean</span></span>|<span data-ttu-id="ea003-274">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ea003-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="ea003-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ea003-275">userAccountControlSettings</span></span>|[<span data-ttu-id="ea003-276">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ea003-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="ea003-277">Einstellungen der Benutzerkontensteuerung.</span><span class="sxs-lookup"><span data-stu-id="ea003-277">The user account control settings.</span></span> <span data-ttu-id="ea003-278">Mögliche Werte: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="ea003-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="ea003-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="ea003-279">workFoldersUrl</span></span>|<span data-ttu-id="ea003-280">String</span><span class="sxs-lookup"><span data-stu-id="ea003-280">String</span></span>|<span data-ttu-id="ea003-281">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="ea003-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="ea003-282">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea003-282">Response</span></span>
<span data-ttu-id="ea003-283">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ea003-283">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea003-284">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea003-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea003-285">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea003-285">Request</span></span>
<span data-ttu-id="ea003-286">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea003-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1924

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="ea003-287">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea003-287">Response</span></span>
<span data-ttu-id="ea003-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea003-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




