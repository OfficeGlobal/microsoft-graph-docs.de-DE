---
title: Aktualisieren von „windows81GeneralConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21de1e83d2153bfebdb6e3099a91dde5c7cca1b2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252826"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="2e7cc-103">Aktualisieren von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="2e7cc-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="2e7cc-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e7cc-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-105">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e7cc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e7cc-106">Prerequisites</span></span>
<span data-ttu-id="2e7cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2e7cc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e7cc-109">Permission type</span></span>|<span data-ttu-id="2e7cc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e7cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e7cc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e7cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e7cc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e7cc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e7cc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e7cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e7cc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e7cc-114">Not supported.</span></span>|
|<span data-ttu-id="2e7cc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e7cc-115">Application</span></span>|<span data-ttu-id="2e7cc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e7cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e7cc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e7cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2e7cc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e7cc-118">Request headers</span></span>
|<span data-ttu-id="2e7cc-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e7cc-119">Header</span></span>|<span data-ttu-id="2e7cc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2e7cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e7cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e7cc-121">Authorization</span></span>|<span data-ttu-id="2e7cc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e7cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e7cc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e7cc-123">Accept</span></span>|<span data-ttu-id="2e7cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e7cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e7cc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e7cc-125">Request body</span></span>
<span data-ttu-id="2e7cc-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-126">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="2e7cc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-127">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="2e7cc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e7cc-128">Property</span></span>|<span data-ttu-id="2e7cc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2e7cc-129">Type</span></span>|<span data-ttu-id="2e7cc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e7cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e7cc-131">id</span><span class="sxs-lookup"><span data-stu-id="2e7cc-131">id</span></span>|<span data-ttu-id="2e7cc-132">string</span><span class="sxs-lookup"><span data-stu-id="2e7cc-132">String</span></span>|<span data-ttu-id="2e7cc-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2e7cc-133">Key of the entity.</span></span> <span data-ttu-id="2e7cc-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e7cc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e7cc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2e7cc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e7cc-136">DateTimeOffset</span></span>|<span data-ttu-id="2e7cc-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2e7cc-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e7cc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e7cc-139">createdDateTime</span></span>|<span data-ttu-id="2e7cc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e7cc-140">DateTimeOffset</span></span>|<span data-ttu-id="2e7cc-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-141">DateTime the object was created.</span></span> <span data-ttu-id="2e7cc-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e7cc-143">description</span><span class="sxs-lookup"><span data-stu-id="2e7cc-143">description</span></span>|<span data-ttu-id="2e7cc-144">String</span><span class="sxs-lookup"><span data-stu-id="2e7cc-144">String</span></span>|<span data-ttu-id="2e7cc-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2e7cc-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e7cc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2e7cc-147">displayName</span></span>|<span data-ttu-id="2e7cc-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e7cc-148">String</span></span>|<span data-ttu-id="2e7cc-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2e7cc-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2e7cc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e7cc-151">Version</span><span class="sxs-lookup"><span data-stu-id="2e7cc-151">version</span></span>|<span data-ttu-id="2e7cc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-152">Int32</span></span>|<span data-ttu-id="2e7cc-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-153">Version of the device configuration.</span></span> <span data-ttu-id="2e7cc-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e7cc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e7cc-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="2e7cc-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="2e7cc-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-156">Boolean</span></span>|<span data-ttu-id="2e7cc-157">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="2e7cc-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="2e7cc-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="2e7cc-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-159">Boolean</span></span>|<span data-ttu-id="2e7cc-160">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="2e7cc-161">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-161">This property is read-only.</span></span>|
|<span data-ttu-id="2e7cc-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="2e7cc-162">browserBlockAutofill</span></span>|<span data-ttu-id="2e7cc-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-163">Boolean</span></span>|<span data-ttu-id="2e7cc-164">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="2e7cc-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="2e7cc-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="2e7cc-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-166">Boolean</span></span>|<span data-ttu-id="2e7cc-167">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="2e7cc-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="2e7cc-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="2e7cc-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-169">Boolean</span></span>|<span data-ttu-id="2e7cc-170">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="2e7cc-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="2e7cc-171">browserBlockJavaScript</span></span>|<span data-ttu-id="2e7cc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-172">Boolean</span></span>|<span data-ttu-id="2e7cc-173">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="2e7cc-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="2e7cc-174">browserBlockPlugins</span></span>|<span data-ttu-id="2e7cc-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-175">Boolean</span></span>|<span data-ttu-id="2e7cc-176">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="2e7cc-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="2e7cc-177">browserBlockPopups</span></span>|<span data-ttu-id="2e7cc-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-178">Boolean</span></span>|<span data-ttu-id="2e7cc-179">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="2e7cc-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="2e7cc-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="2e7cc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-181">Boolean</span></span>|<span data-ttu-id="2e7cc-182">Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="2e7cc-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="2e7cc-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="2e7cc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-184">Boolean</span></span>|<span data-ttu-id="2e7cc-185">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="2e7cc-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="2e7cc-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="2e7cc-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2e7cc-187">Boolean</span></span>|<span data-ttu-id="2e7cc-188">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="2e7cc-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="2e7cc-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="2e7cc-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e7cc-190">String</span></span>|<span data-ttu-id="2e7cc-191">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-191">The enterprise mode site list location.</span></span> <span data-ttu-id="2e7cc-192">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="2e7cc-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="2e7cc-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="2e7cc-195">Internetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-195">The internet security level.</span></span> <span data-ttu-id="2e7cc-196">Mögliche Werte: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="2e7cc-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="2e7cc-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="2e7cc-199">Intranetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-199">The Intranet security level.</span></span> <span data-ttu-id="2e7cc-200">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="2e7cc-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="2e7cc-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="2e7cc-202">String</span><span class="sxs-lookup"><span data-stu-id="2e7cc-202">String</span></span>|<span data-ttu-id="2e7cc-203">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="2e7cc-203">The logging report location.</span></span>|
|<span data-ttu-id="2e7cc-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="2e7cc-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="2e7cc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-205">Boolean</span></span>|<span data-ttu-id="2e7cc-206">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="2e7cc-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="2e7cc-207">browserRequireFirewall</span></span>|<span data-ttu-id="2e7cc-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-208">Boolean</span></span>|<span data-ttu-id="2e7cc-209">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="2e7cc-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="2e7cc-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="2e7cc-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-211">Boolean</span></span>|<span data-ttu-id="2e7cc-212">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="2e7cc-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="2e7cc-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="2e7cc-215">Sicherheitsstufe für vertrauenswürdige Websites.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-215">The trusted sites security level.</span></span> <span data-ttu-id="2e7cc-216">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="2e7cc-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="2e7cc-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="2e7cc-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-218">Boolean</span></span>|<span data-ttu-id="2e7cc-219">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="2e7cc-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="2e7cc-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="2e7cc-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-221">Boolean</span></span>|<span data-ttu-id="2e7cc-222">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="2e7cc-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="2e7cc-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="2e7cc-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-224">Boolean</span></span>|<span data-ttu-id="2e7cc-225">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="2e7cc-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2e7cc-226">passwordExpirationDays</span></span>|<span data-ttu-id="2e7cc-227">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-227">Int32</span></span>|<span data-ttu-id="2e7cc-228">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="2e7cc-228">Password expiration in days.</span></span>|
|<span data-ttu-id="2e7cc-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2e7cc-229">passwordMinimumLength</span></span>|<span data-ttu-id="2e7cc-230">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-230">Int32</span></span>|<span data-ttu-id="2e7cc-231">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="2e7cc-231">The minimum password length.</span></span>|
|<span data-ttu-id="2e7cc-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2e7cc-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2e7cc-233">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-233">Int32</span></span>|<span data-ttu-id="2e7cc-234">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="2e7cc-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2e7cc-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2e7cc-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2e7cc-236">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-236">Int32</span></span>|<span data-ttu-id="2e7cc-237">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="2e7cc-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2e7cc-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2e7cc-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2e7cc-239">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-239">Int32</span></span>|<span data-ttu-id="2e7cc-240">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="2e7cc-241">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2e7cc-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2e7cc-242">passwordRequiredType</span></span>|[<span data-ttu-id="2e7cc-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2e7cc-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2e7cc-244">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-244">The required password type.</span></span> <span data-ttu-id="2e7cc-245">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2e7cc-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2e7cc-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2e7cc-247">Int32</span><span class="sxs-lookup"><span data-stu-id="2e7cc-247">Int32</span></span>|<span data-ttu-id="2e7cc-248">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="2e7cc-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="2e7cc-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="2e7cc-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7cc-250">Boolean</span></span>|<span data-ttu-id="2e7cc-251">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="2e7cc-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="2e7cc-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="2e7cc-253">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2e7cc-253">Boolean</span></span>|<span data-ttu-id="2e7cc-254">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="2e7cc-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="2e7cc-255">userAccountControlSettings</span></span>|[<span data-ttu-id="2e7cc-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="2e7cc-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="2e7cc-257">Einstellungen der Benutzerkontensteuerung.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-257">The user account control settings.</span></span> <span data-ttu-id="2e7cc-258">Mögliche Werte: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="2e7cc-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="2e7cc-259">workFoldersUrl</span></span>|<span data-ttu-id="2e7cc-260">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e7cc-260">String</span></span>|<span data-ttu-id="2e7cc-261">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="2e7cc-262">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e7cc-262">Response</span></span>
<span data-ttu-id="2e7cc-263">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-263">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e7cc-264">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e7cc-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e7cc-265">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e7cc-265">Request</span></span>
<span data-ttu-id="2e7cc-266">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="2e7cc-267">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e7cc-267">Response</span></span>
<span data-ttu-id="2e7cc-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e7cc-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```



