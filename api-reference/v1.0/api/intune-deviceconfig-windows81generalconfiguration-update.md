---
title: Aktualisieren von „windows81GeneralConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c5a0d1f5ab921859a7af19a9257f79c2f1f9a03c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964886"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="83be5-103">Aktualisieren von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="83be5-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="83be5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83be5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83be5-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-105">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83be5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83be5-106">Prerequisites</span></span>
<span data-ttu-id="83be5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83be5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83be5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83be5-109">Permission type</span></span>|<span data-ttu-id="83be5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83be5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83be5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83be5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83be5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83be5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83be5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83be5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83be5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83be5-114">Not supported.</span></span>|
|<span data-ttu-id="83be5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83be5-115">Application</span></span>|<span data-ttu-id="83be5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83be5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83be5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83be5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83be5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83be5-118">Request headers</span></span>
|<span data-ttu-id="83be5-119">Header</span><span class="sxs-lookup"><span data-stu-id="83be5-119">Header</span></span>|<span data-ttu-id="83be5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83be5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83be5-121">Authorization</span></span>|<span data-ttu-id="83be5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83be5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83be5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="83be5-123">Accept</span></span>|<span data-ttu-id="83be5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83be5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83be5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83be5-125">Request body</span></span>
<span data-ttu-id="83be5-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="83be5-126">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="83be5-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="83be5-127">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="83be5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83be5-128">Property</span></span>|<span data-ttu-id="83be5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="83be5-129">Type</span></span>|<span data-ttu-id="83be5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83be5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83be5-131">id</span><span class="sxs-lookup"><span data-stu-id="83be5-131">id</span></span>|<span data-ttu-id="83be5-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83be5-132">String</span></span>|<span data-ttu-id="83be5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="83be5-133">Key of the entity.</span></span> <span data-ttu-id="83be5-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83be5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83be5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="83be5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83be5-136">DateTimeOffset</span></span>|<span data-ttu-id="83be5-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="83be5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="83be5-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83be5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83be5-139">createdDateTime</span></span>|<span data-ttu-id="83be5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83be5-140">DateTimeOffset</span></span>|<span data-ttu-id="83be5-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="83be5-141">DateTime the object was created.</span></span> <span data-ttu-id="83be5-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83be5-143">description</span><span class="sxs-lookup"><span data-stu-id="83be5-143">description</span></span>|<span data-ttu-id="83be5-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83be5-144">String</span></span>|<span data-ttu-id="83be5-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="83be5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83be5-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83be5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="83be5-147">displayName</span></span>|<span data-ttu-id="83be5-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83be5-148">String</span></span>|<span data-ttu-id="83be5-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="83be5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83be5-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83be5-151">Version</span><span class="sxs-lookup"><span data-stu-id="83be5-151">version</span></span>|<span data-ttu-id="83be5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-152">Int32</span></span>|<span data-ttu-id="83be5-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="83be5-153">Version of the device configuration.</span></span> <span data-ttu-id="83be5-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83be5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83be5-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="83be5-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="83be5-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-156">Boolean</span></span>|<span data-ttu-id="83be5-157">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="83be5-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="83be5-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="83be5-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="83be5-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-159">Boolean</span></span>|<span data-ttu-id="83be5-160">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="83be5-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="83be5-161">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="83be5-161">This property is read-only.</span></span>|
|<span data-ttu-id="83be5-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="83be5-162">browserBlockAutofill</span></span>|<span data-ttu-id="83be5-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-163">Boolean</span></span>|<span data-ttu-id="83be5-164">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83be5-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="83be5-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="83be5-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="83be5-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-166">Boolean</span></span>|<span data-ttu-id="83be5-167">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83be5-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="83be5-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="83be5-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="83be5-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-169">Boolean</span></span>|<span data-ttu-id="83be5-170">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83be5-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="83be5-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="83be5-171">browserBlockJavaScript</span></span>|<span data-ttu-id="83be5-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-172">Boolean</span></span>|<span data-ttu-id="83be5-173">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="83be5-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="83be5-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="83be5-174">browserBlockPlugins</span></span>|<span data-ttu-id="83be5-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-175">Boolean</span></span>|<span data-ttu-id="83be5-176">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83be5-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="83be5-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="83be5-177">browserBlockPopups</span></span>|<span data-ttu-id="83be5-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-178">Boolean</span></span>|<span data-ttu-id="83be5-179">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83be5-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="83be5-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="83be5-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="83be5-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-181">Boolean</span></span>|<span data-ttu-id="83be5-182">Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.</span><span class="sxs-lookup"><span data-stu-id="83be5-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="83be5-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="83be5-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="83be5-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-184">Boolean</span></span>|<span data-ttu-id="83be5-185">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83be5-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="83be5-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="83be5-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="83be5-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-187">Boolean</span></span>|<span data-ttu-id="83be5-188">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="83be5-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="83be5-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="83be5-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="83be5-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83be5-190">String</span></span>|<span data-ttu-id="83be5-191">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="83be5-191">The enterprise mode site list location.</span></span> <span data-ttu-id="83be5-192">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="83be5-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="83be5-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="83be5-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="83be5-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="83be5-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="83be5-195">Internetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="83be5-195">The internet security level.</span></span> <span data-ttu-id="83be5-196">Mögliche Werte: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="83be5-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="83be5-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="83be5-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="83be5-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="83be5-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="83be5-199">Intranetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="83be5-199">The Intranet security level.</span></span> <span data-ttu-id="83be5-200">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="83be5-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="83be5-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="83be5-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="83be5-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83be5-202">String</span></span>|<span data-ttu-id="83be5-203">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="83be5-203">The logging report location.</span></span>|
|<span data-ttu-id="83be5-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="83be5-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="83be5-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-205">Boolean</span></span>|<span data-ttu-id="83be5-206">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="83be5-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="83be5-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="83be5-207">browserRequireFirewall</span></span>|<span data-ttu-id="83be5-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-208">Boolean</span></span>|<span data-ttu-id="83be5-209">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="83be5-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="83be5-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="83be5-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="83be5-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-211">Boolean</span></span>|<span data-ttu-id="83be5-212">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="83be5-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="83be5-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="83be5-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="83be5-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="83be5-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="83be5-215">Sicherheitsstufe für vertrauenswürdige Websites.</span><span class="sxs-lookup"><span data-stu-id="83be5-215">The trusted sites security level.</span></span> <span data-ttu-id="83be5-216">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="83be5-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="83be5-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="83be5-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="83be5-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-218">Boolean</span></span>|<span data-ttu-id="83be5-219">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83be5-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="83be5-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="83be5-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="83be5-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-221">Boolean</span></span>|<span data-ttu-id="83be5-222">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83be5-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="83be5-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="83be5-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="83be5-224">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-224">Boolean</span></span>|<span data-ttu-id="83be5-225">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="83be5-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="83be5-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="83be5-226">passwordExpirationDays</span></span>|<span data-ttu-id="83be5-227">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-227">Int32</span></span>|<span data-ttu-id="83be5-228">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="83be5-228">Password expiration in days.</span></span>|
|<span data-ttu-id="83be5-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="83be5-229">passwordMinimumLength</span></span>|<span data-ttu-id="83be5-230">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-230">Int32</span></span>|<span data-ttu-id="83be5-231">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="83be5-231">The minimum password length.</span></span>|
|<span data-ttu-id="83be5-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="83be5-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="83be5-233">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-233">Int32</span></span>|<span data-ttu-id="83be5-234">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="83be5-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="83be5-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="83be5-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="83be5-236">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-236">Int32</span></span>|<span data-ttu-id="83be5-237">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="83be5-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="83be5-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="83be5-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="83be5-239">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-239">Int32</span></span>|<span data-ttu-id="83be5-240">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="83be5-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="83be5-241">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="83be5-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="83be5-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="83be5-242">passwordRequiredType</span></span>|[<span data-ttu-id="83be5-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="83be5-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="83be5-244">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="83be5-244">The required password type.</span></span> <span data-ttu-id="83be5-245">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="83be5-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="83be5-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="83be5-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="83be5-247">Int32</span><span class="sxs-lookup"><span data-stu-id="83be5-247">Int32</span></span>|<span data-ttu-id="83be5-248">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="83be5-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="83be5-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="83be5-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="83be5-250">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-250">Boolean</span></span>|<span data-ttu-id="83be5-251">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="83be5-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="83be5-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="83be5-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="83be5-253">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83be5-253">Boolean</span></span>|<span data-ttu-id="83be5-254">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="83be5-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="83be5-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="83be5-255">userAccountControlSettings</span></span>|[<span data-ttu-id="83be5-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="83be5-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="83be5-257">Einstellungen der Benutzerkontensteuerung.</span><span class="sxs-lookup"><span data-stu-id="83be5-257">The user account control settings.</span></span> <span data-ttu-id="83be5-258">Mögliche Werte sind: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming` und `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="83be5-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="83be5-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="83be5-259">workFoldersUrl</span></span>|<span data-ttu-id="83be5-260">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83be5-260">String</span></span>|<span data-ttu-id="83be5-261">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="83be5-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="83be5-262">Antwort</span><span class="sxs-lookup"><span data-stu-id="83be5-262">Response</span></span>
<span data-ttu-id="83be5-263">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83be5-263">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83be5-264">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83be5-264">Example</span></span>
### <a name="request"></a><span data-ttu-id="83be5-265">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83be5-265">Request</span></span>
<span data-ttu-id="83be5-266">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83be5-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83be5-267">Antwort</span><span class="sxs-lookup"><span data-stu-id="83be5-267">Response</span></span>
<span data-ttu-id="83be5-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83be5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



