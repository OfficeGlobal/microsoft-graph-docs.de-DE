---
title: Erstellen von „windows81GeneralConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows81GeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: c06b6f4a955d904b1da65b11e99ef4af307004cb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319747"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="9aac7-103">Erstellen von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="9aac7-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="9aac7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9aac7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aac7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9aac7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9aac7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9aac7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9aac7-107">Diese Methode erstellt ein neues Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9aac7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9aac7-108">Prerequisites</span></span>
<span data-ttu-id="9aac7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aac7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aac7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9aac7-111">Permission type</span></span>|<span data-ttu-id="9aac7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9aac7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9aac7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9aac7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9aac7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aac7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9aac7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9aac7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9aac7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9aac7-116">Not supported.</span></span>|
|<span data-ttu-id="9aac7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9aac7-117">Application</span></span>|<span data-ttu-id="9aac7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9aac7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9aac7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9aac7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9aac7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9aac7-120">Request headers</span></span>
|<span data-ttu-id="9aac7-121">Header</span><span class="sxs-lookup"><span data-stu-id="9aac7-121">Header</span></span>|<span data-ttu-id="9aac7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9aac7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9aac7-123">Authorization</span></span>|<span data-ttu-id="9aac7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9aac7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9aac7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9aac7-125">Accept</span></span>|<span data-ttu-id="9aac7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9aac7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aac7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9aac7-127">Request body</span></span>
<span data-ttu-id="9aac7-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="9aac7-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="9aac7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9aac7-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="9aac7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9aac7-130">Property</span></span>|<span data-ttu-id="9aac7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9aac7-131">Type</span></span>|<span data-ttu-id="9aac7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9aac7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aac7-133">id</span><span class="sxs-lookup"><span data-stu-id="9aac7-133">id</span></span>|<span data-ttu-id="9aac7-134">String</span><span class="sxs-lookup"><span data-stu-id="9aac7-134">String</span></span>|<span data-ttu-id="9aac7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9aac7-135">Key of the entity.</span></span> <span data-ttu-id="9aac7-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9aac7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9aac7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aac7-138">DateTimeOffset</span></span>|<span data-ttu-id="9aac7-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9aac7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9aac7-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9aac7-141">roleScopeTagIds</span></span>|<span data-ttu-id="9aac7-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="9aac7-142">String collection</span></span>|<span data-ttu-id="9aac7-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="9aac7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9aac7-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9aac7-145">supportsScopeTags</span></span>|<span data-ttu-id="9aac7-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9aac7-146">Boolean</span></span>|<span data-ttu-id="9aac7-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9aac7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9aac7-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="9aac7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9aac7-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9aac7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9aac7-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9aac7-150">This property is read-only.</span></span> <span data-ttu-id="9aac7-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9aac7-152">createdDateTime</span></span>|<span data-ttu-id="9aac7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aac7-153">DateTimeOffset</span></span>|<span data-ttu-id="9aac7-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9aac7-154">DateTime the object was created.</span></span> <span data-ttu-id="9aac7-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-156">description</span><span class="sxs-lookup"><span data-stu-id="9aac7-156">description</span></span>|<span data-ttu-id="9aac7-157">String</span><span class="sxs-lookup"><span data-stu-id="9aac7-157">String</span></span>|<span data-ttu-id="9aac7-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9aac7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9aac7-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9aac7-160">displayName</span></span>|<span data-ttu-id="9aac7-161">String</span><span class="sxs-lookup"><span data-stu-id="9aac7-161">String</span></span>|<span data-ttu-id="9aac7-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9aac7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9aac7-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-164">Version</span><span class="sxs-lookup"><span data-stu-id="9aac7-164">version</span></span>|<span data-ttu-id="9aac7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-165">Int32</span></span>|<span data-ttu-id="9aac7-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9aac7-166">Version of the device configuration.</span></span> <span data-ttu-id="9aac7-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9aac7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9aac7-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="9aac7-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="9aac7-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-169">Boolean</span></span>|<span data-ttu-id="9aac7-170">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="9aac7-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="9aac7-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="9aac7-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="9aac7-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-172">Boolean</span></span>|<span data-ttu-id="9aac7-173">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="9aac7-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9aac7-174">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9aac7-174">This property is read-only.</span></span>|
|<span data-ttu-id="9aac7-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="9aac7-175">browserBlockAutofill</span></span>|<span data-ttu-id="9aac7-176">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-176">Boolean</span></span>|<span data-ttu-id="9aac7-177">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9aac7-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="9aac7-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="9aac7-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="9aac7-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-179">Boolean</span></span>|<span data-ttu-id="9aac7-180">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9aac7-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="9aac7-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="9aac7-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="9aac7-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-182">Boolean</span></span>|<span data-ttu-id="9aac7-183">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9aac7-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="9aac7-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="9aac7-184">browserBlockJavaScript</span></span>|<span data-ttu-id="9aac7-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-185">Boolean</span></span>|<span data-ttu-id="9aac7-186">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="9aac7-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="9aac7-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="9aac7-187">browserBlockPlugins</span></span>|<span data-ttu-id="9aac7-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-188">Boolean</span></span>|<span data-ttu-id="9aac7-189">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9aac7-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="9aac7-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="9aac7-190">browserBlockPopups</span></span>|<span data-ttu-id="9aac7-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-191">Boolean</span></span>|<span data-ttu-id="9aac7-192">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9aac7-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="9aac7-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="9aac7-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="9aac7-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-194">Boolean</span></span>|<span data-ttu-id="9aac7-195">Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.</span><span class="sxs-lookup"><span data-stu-id="9aac7-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="9aac7-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="9aac7-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="9aac7-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-197">Boolean</span></span>|<span data-ttu-id="9aac7-198">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9aac7-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="9aac7-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="9aac7-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="9aac7-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-200">Boolean</span></span>|<span data-ttu-id="9aac7-201">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="9aac7-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="9aac7-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="9aac7-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="9aac7-203">String</span><span class="sxs-lookup"><span data-stu-id="9aac7-203">String</span></span>|<span data-ttu-id="9aac7-204">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="9aac7-204">The enterprise mode site list location.</span></span> <span data-ttu-id="9aac7-205">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="9aac7-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="9aac7-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9aac7-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="9aac7-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9aac7-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="9aac7-208">Internetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="9aac7-208">The internet security level.</span></span> <span data-ttu-id="9aac7-209">Mögliche Werte: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="9aac7-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9aac7-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="9aac7-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9aac7-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="9aac7-212">Intranetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="9aac7-212">The Intranet security level.</span></span> <span data-ttu-id="9aac7-213">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="9aac7-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="9aac7-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="9aac7-215">String</span><span class="sxs-lookup"><span data-stu-id="9aac7-215">String</span></span>|<span data-ttu-id="9aac7-216">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="9aac7-216">The logging report location.</span></span>|
|<span data-ttu-id="9aac7-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="9aac7-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="9aac7-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-218">Boolean</span></span>|<span data-ttu-id="9aac7-219">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="9aac7-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="9aac7-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="9aac7-220">browserRequireFirewall</span></span>|<span data-ttu-id="9aac7-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-221">Boolean</span></span>|<span data-ttu-id="9aac7-222">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9aac7-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="9aac7-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="9aac7-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="9aac7-224">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-224">Boolean</span></span>|<span data-ttu-id="9aac7-225">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9aac7-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="9aac7-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9aac7-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="9aac7-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9aac7-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="9aac7-228">Sicherheitsstufe für vertrauenswürdige Websites.</span><span class="sxs-lookup"><span data-stu-id="9aac7-228">The trusted sites security level.</span></span> <span data-ttu-id="9aac7-229">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="9aac7-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="9aac7-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="9aac7-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-231">Boolean</span></span>|<span data-ttu-id="9aac7-232">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9aac7-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="9aac7-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="9aac7-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="9aac7-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-234">Boolean</span></span>|<span data-ttu-id="9aac7-235">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9aac7-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9aac7-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="9aac7-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="9aac7-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-237">Boolean</span></span>|<span data-ttu-id="9aac7-238">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="9aac7-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="9aac7-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9aac7-239">passwordExpirationDays</span></span>|<span data-ttu-id="9aac7-240">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-240">Int32</span></span>|<span data-ttu-id="9aac7-241">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="9aac7-241">Password expiration in days.</span></span>|
|<span data-ttu-id="9aac7-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9aac7-242">passwordMinimumLength</span></span>|<span data-ttu-id="9aac7-243">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-243">Int32</span></span>|<span data-ttu-id="9aac7-244">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="9aac7-244">The minimum password length.</span></span>|
|<span data-ttu-id="9aac7-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9aac7-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9aac7-246">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-246">Int32</span></span>|<span data-ttu-id="9aac7-247">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="9aac7-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9aac7-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9aac7-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9aac7-249">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-249">Int32</span></span>|<span data-ttu-id="9aac7-250">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="9aac7-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9aac7-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9aac7-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9aac7-252">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-252">Int32</span></span>|<span data-ttu-id="9aac7-253">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="9aac7-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="9aac7-254">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="9aac7-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9aac7-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9aac7-255">passwordRequiredType</span></span>|[<span data-ttu-id="9aac7-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9aac7-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9aac7-257">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="9aac7-257">The required password type.</span></span> <span data-ttu-id="9aac7-258">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9aac7-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9aac7-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9aac7-260">Int32</span><span class="sxs-lookup"><span data-stu-id="9aac7-260">Int32</span></span>|<span data-ttu-id="9aac7-261">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9aac7-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="9aac7-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="9aac7-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="9aac7-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-263">Boolean</span></span>|<span data-ttu-id="9aac7-264">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="9aac7-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="9aac7-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="9aac7-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="9aac7-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="9aac7-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="9aac7-267">Die minimale aktualisieren Klassifizierung, automatisch zu installieren.</span><span class="sxs-lookup"><span data-stu-id="9aac7-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="9aac7-268">Mögliche Werte: sind `userDefined`, `recommendedAndImportant`, `important` und `none`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="9aac7-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="9aac7-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="9aac7-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="9aac7-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="9aac7-271">Die minimale aktualisieren Klassifizierung, automatisch zu installieren.</span><span class="sxs-lookup"><span data-stu-id="9aac7-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="9aac7-272">Mögliche Werte: sind `userDefined`, `recommendedAndImportant`, `important` und `none`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="9aac7-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="9aac7-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="9aac7-274">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9aac7-274">Boolean</span></span>|<span data-ttu-id="9aac7-275">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9aac7-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="9aac7-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="9aac7-276">userAccountControlSettings</span></span>|[<span data-ttu-id="9aac7-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="9aac7-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="9aac7-278">Einstellungen der Benutzerkontensteuerung.</span><span class="sxs-lookup"><span data-stu-id="9aac7-278">The user account control settings.</span></span> <span data-ttu-id="9aac7-279">Mögliche Werte sind: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming` und `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="9aac7-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="9aac7-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="9aac7-280">workFoldersUrl</span></span>|<span data-ttu-id="9aac7-281">String</span><span class="sxs-lookup"><span data-stu-id="9aac7-281">String</span></span>|<span data-ttu-id="9aac7-282">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="9aac7-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="9aac7-283">Antwort</span><span class="sxs-lookup"><span data-stu-id="9aac7-283">Response</span></span>
<span data-ttu-id="9aac7-284">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9aac7-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aac7-285">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9aac7-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="9aac7-286">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9aac7-286">Request</span></span>
<span data-ttu-id="9aac7-287">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9aac7-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="9aac7-288">Antwort</span><span class="sxs-lookup"><span data-stu-id="9aac7-288">Response</span></span>
<span data-ttu-id="9aac7-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9aac7-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





