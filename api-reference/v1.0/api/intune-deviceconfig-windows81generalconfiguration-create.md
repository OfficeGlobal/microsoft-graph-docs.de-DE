---
title: Erstellen von „windows81GeneralConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: afdeec91b1e7737b2948efb45a0a496ee15d327a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250523"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="0118f-103">Erstellen von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="0118f-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="0118f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0118f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0118f-105">Diese Methode erstellt ein neues Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-105">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0118f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0118f-106">Prerequisites</span></span>
<span data-ttu-id="0118f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0118f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0118f-109">Permission type</span></span>|<span data-ttu-id="0118f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0118f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0118f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0118f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0118f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0118f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0118f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0118f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0118f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0118f-114">Not supported.</span></span>|
|<span data-ttu-id="0118f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0118f-115">Application</span></span>|<span data-ttu-id="0118f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0118f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0118f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0118f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0118f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0118f-118">Request headers</span></span>
|<span data-ttu-id="0118f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0118f-119">Header</span></span>|<span data-ttu-id="0118f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0118f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0118f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0118f-121">Authorization</span></span>|<span data-ttu-id="0118f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0118f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0118f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0118f-123">Accept</span></span>|<span data-ttu-id="0118f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0118f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0118f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0118f-125">Request body</span></span>
<span data-ttu-id="0118f-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="0118f-126">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="0118f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0118f-127">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="0118f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0118f-128">Property</span></span>|<span data-ttu-id="0118f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0118f-129">Type</span></span>|<span data-ttu-id="0118f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0118f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0118f-131">id</span><span class="sxs-lookup"><span data-stu-id="0118f-131">id</span></span>|<span data-ttu-id="0118f-132">string</span><span class="sxs-lookup"><span data-stu-id="0118f-132">String</span></span>|<span data-ttu-id="0118f-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0118f-133">Key of the entity.</span></span> <span data-ttu-id="0118f-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0118f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0118f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0118f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0118f-136">DateTimeOffset</span></span>|<span data-ttu-id="0118f-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0118f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0118f-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0118f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0118f-139">createdDateTime</span></span>|<span data-ttu-id="0118f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0118f-140">DateTimeOffset</span></span>|<span data-ttu-id="0118f-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0118f-141">DateTime the object was created.</span></span> <span data-ttu-id="0118f-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0118f-143">description</span><span class="sxs-lookup"><span data-stu-id="0118f-143">description</span></span>|<span data-ttu-id="0118f-144">String</span><span class="sxs-lookup"><span data-stu-id="0118f-144">String</span></span>|<span data-ttu-id="0118f-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0118f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0118f-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0118f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0118f-147">displayName</span></span>|<span data-ttu-id="0118f-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0118f-148">String</span></span>|<span data-ttu-id="0118f-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0118f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0118f-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0118f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0118f-151">Version</span><span class="sxs-lookup"><span data-stu-id="0118f-151">version</span></span>|<span data-ttu-id="0118f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-152">Int32</span></span>|<span data-ttu-id="0118f-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0118f-153">Version of the device configuration.</span></span> <span data-ttu-id="0118f-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0118f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0118f-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="0118f-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="0118f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-156">Boolean</span></span>|<span data-ttu-id="0118f-157">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="0118f-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="0118f-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="0118f-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="0118f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-159">Boolean</span></span>|<span data-ttu-id="0118f-160">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="0118f-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="0118f-161">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0118f-161">This property is read-only.</span></span>|
|<span data-ttu-id="0118f-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="0118f-162">browserBlockAutofill</span></span>|<span data-ttu-id="0118f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-163">Boolean</span></span>|<span data-ttu-id="0118f-164">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0118f-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="0118f-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="0118f-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="0118f-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-166">Boolean</span></span>|<span data-ttu-id="0118f-167">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0118f-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="0118f-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="0118f-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="0118f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-169">Boolean</span></span>|<span data-ttu-id="0118f-170">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0118f-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="0118f-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="0118f-171">browserBlockJavaScript</span></span>|<span data-ttu-id="0118f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-172">Boolean</span></span>|<span data-ttu-id="0118f-173">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="0118f-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="0118f-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="0118f-174">browserBlockPlugins</span></span>|<span data-ttu-id="0118f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-175">Boolean</span></span>|<span data-ttu-id="0118f-176">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0118f-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="0118f-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="0118f-177">browserBlockPopups</span></span>|<span data-ttu-id="0118f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-178">Boolean</span></span>|<span data-ttu-id="0118f-179">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0118f-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="0118f-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="0118f-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="0118f-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-181">Boolean</span></span>|<span data-ttu-id="0118f-182">Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.</span><span class="sxs-lookup"><span data-stu-id="0118f-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="0118f-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="0118f-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="0118f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-184">Boolean</span></span>|<span data-ttu-id="0118f-185">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0118f-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="0118f-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="0118f-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="0118f-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0118f-187">Boolean</span></span>|<span data-ttu-id="0118f-188">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="0118f-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="0118f-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="0118f-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="0118f-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0118f-190">String</span></span>|<span data-ttu-id="0118f-191">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="0118f-191">The enterprise mode site list location.</span></span> <span data-ttu-id="0118f-192">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="0118f-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="0118f-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0118f-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="0118f-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0118f-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="0118f-195">Internetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="0118f-195">The internet security level.</span></span> <span data-ttu-id="0118f-196">Mögliche Werte: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="0118f-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="0118f-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0118f-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="0118f-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0118f-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="0118f-199">Intranetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="0118f-199">The Intranet security level.</span></span> <span data-ttu-id="0118f-200">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="0118f-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="0118f-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="0118f-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="0118f-202">String</span><span class="sxs-lookup"><span data-stu-id="0118f-202">String</span></span>|<span data-ttu-id="0118f-203">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="0118f-203">The logging report location.</span></span>|
|<span data-ttu-id="0118f-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="0118f-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="0118f-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-205">Boolean</span></span>|<span data-ttu-id="0118f-206">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="0118f-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="0118f-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="0118f-207">browserRequireFirewall</span></span>|<span data-ttu-id="0118f-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-208">Boolean</span></span>|<span data-ttu-id="0118f-209">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0118f-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="0118f-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="0118f-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="0118f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-211">Boolean</span></span>|<span data-ttu-id="0118f-212">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0118f-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="0118f-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0118f-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="0118f-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0118f-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="0118f-215">Sicherheitsstufe für vertrauenswürdige Websites.</span><span class="sxs-lookup"><span data-stu-id="0118f-215">The trusted sites security level.</span></span> <span data-ttu-id="0118f-216">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="0118f-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="0118f-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="0118f-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="0118f-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-218">Boolean</span></span>|<span data-ttu-id="0118f-219">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0118f-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="0118f-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="0118f-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="0118f-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-221">Boolean</span></span>|<span data-ttu-id="0118f-222">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0118f-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="0118f-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="0118f-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="0118f-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-224">Boolean</span></span>|<span data-ttu-id="0118f-225">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="0118f-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="0118f-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0118f-226">passwordExpirationDays</span></span>|<span data-ttu-id="0118f-227">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-227">Int32</span></span>|<span data-ttu-id="0118f-228">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="0118f-228">Password expiration in days.</span></span>|
|<span data-ttu-id="0118f-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0118f-229">passwordMinimumLength</span></span>|<span data-ttu-id="0118f-230">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-230">Int32</span></span>|<span data-ttu-id="0118f-231">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="0118f-231">The minimum password length.</span></span>|
|<span data-ttu-id="0118f-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0118f-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0118f-233">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-233">Int32</span></span>|<span data-ttu-id="0118f-234">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="0118f-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="0118f-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0118f-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0118f-236">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-236">Int32</span></span>|<span data-ttu-id="0118f-237">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="0118f-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0118f-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0118f-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0118f-239">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-239">Int32</span></span>|<span data-ttu-id="0118f-240">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="0118f-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="0118f-241">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="0118f-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0118f-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0118f-242">passwordRequiredType</span></span>|[<span data-ttu-id="0118f-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0118f-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0118f-244">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="0118f-244">The required password type.</span></span> <span data-ttu-id="0118f-245">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0118f-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0118f-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0118f-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0118f-247">Int32</span><span class="sxs-lookup"><span data-stu-id="0118f-247">Int32</span></span>|<span data-ttu-id="0118f-248">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="0118f-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="0118f-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="0118f-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="0118f-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="0118f-250">Boolean</span></span>|<span data-ttu-id="0118f-251">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="0118f-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="0118f-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="0118f-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="0118f-253">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0118f-253">Boolean</span></span>|<span data-ttu-id="0118f-254">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0118f-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="0118f-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="0118f-255">userAccountControlSettings</span></span>|[<span data-ttu-id="0118f-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="0118f-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="0118f-257">Einstellungen der Benutzerkontensteuerung.</span><span class="sxs-lookup"><span data-stu-id="0118f-257">The user account control settings.</span></span> <span data-ttu-id="0118f-258">Mögliche Werte: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="0118f-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="0118f-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="0118f-259">workFoldersUrl</span></span>|<span data-ttu-id="0118f-260">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0118f-260">String</span></span>|<span data-ttu-id="0118f-261">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="0118f-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="0118f-262">Antwort</span><span class="sxs-lookup"><span data-stu-id="0118f-262">Response</span></span>
<span data-ttu-id="0118f-263">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0118f-263">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0118f-264">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0118f-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="0118f-265">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0118f-265">Request</span></span>
<span data-ttu-id="0118f-266">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0118f-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0118f-267">Antwort</span><span class="sxs-lookup"><span data-stu-id="0118f-267">Response</span></span>
<span data-ttu-id="0118f-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0118f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



