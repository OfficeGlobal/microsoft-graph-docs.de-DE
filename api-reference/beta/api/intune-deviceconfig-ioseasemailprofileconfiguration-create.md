---
title: Erstellen von iosEasEmailProfileConfiguration
description: Erstellen eines neuen IosEasEmailProfileConfiguration-Objekts.
ms.openlocfilehash: 78cf37fc63f6cc62d40ffc1ef3deda587b65aaf3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061850"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="b8fb4-103">Erstellen von iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8fb4-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="b8fb4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8fb4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8fb4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8fb4-107">Erstellen eines neuen [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8fb4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8fb4-108">Prerequisites</span></span>
<span data-ttu-id="b8fb4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8fb4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8fb4-111">Permission type</span></span>|<span data-ttu-id="b8fb4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8fb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8fb4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8fb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8fb4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8fb4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8fb4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8fb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8fb4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8fb4-116">Not supported.</span></span>|
|<span data-ttu-id="b8fb4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8fb4-117">Application</span></span>|<span data-ttu-id="b8fb4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8fb4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8fb4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8fb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8fb4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8fb4-120">Request headers</span></span>
|<span data-ttu-id="b8fb4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8fb4-121">Header</span></span>|<span data-ttu-id="b8fb4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b8fb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8fb4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8fb4-123">Authorization</span></span>|<span data-ttu-id="b8fb4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8fb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8fb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8fb4-125">Accept</span></span>|<span data-ttu-id="b8fb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8fb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8fb4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8fb4-127">Request body</span></span>
<span data-ttu-id="b8fb4-128">Geben Sie im Textkörper Anforderung für das Objekt IosEasEmailProfileConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="b8fb4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosEasEmailProfileConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="b8fb4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8fb4-130">Property</span></span>|<span data-ttu-id="b8fb4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b8fb4-131">Type</span></span>|<span data-ttu-id="b8fb4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8fb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8fb4-133">id</span><span class="sxs-lookup"><span data-stu-id="b8fb4-133">id</span></span>|<span data-ttu-id="b8fb4-134">String</span><span class="sxs-lookup"><span data-stu-id="b8fb4-134">String</span></span>|<span data-ttu-id="b8fb4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b8fb4-135">Key of the entity.</span></span> <span data-ttu-id="b8fb4-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8fb4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8fb4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8fb4-138">DateTimeOffset</span></span>|<span data-ttu-id="b8fb4-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8fb4-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8fb4-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8fb4-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b8fb4-142">String collection</span></span>|<span data-ttu-id="b8fb4-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8fb4-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8fb4-145">supportsScopeTags</span></span>|<span data-ttu-id="b8fb4-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-146">Boolean</span></span>|<span data-ttu-id="b8fb4-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8fb4-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8fb4-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8fb4-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-150">This property is read-only.</span></span> <span data-ttu-id="b8fb4-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8fb4-152">createdDateTime</span></span>|<span data-ttu-id="b8fb4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8fb4-153">DateTimeOffset</span></span>|<span data-ttu-id="b8fb4-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-154">DateTime the object was created.</span></span> <span data-ttu-id="b8fb4-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-156">description</span><span class="sxs-lookup"><span data-stu-id="b8fb4-156">description</span></span>|<span data-ttu-id="b8fb4-157">String</span><span class="sxs-lookup"><span data-stu-id="b8fb4-157">String</span></span>|<span data-ttu-id="b8fb4-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8fb4-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b8fb4-160">displayName</span></span>|<span data-ttu-id="b8fb4-161">String</span><span class="sxs-lookup"><span data-stu-id="b8fb4-161">String</span></span>|<span data-ttu-id="b8fb4-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8fb4-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-164">Version</span><span class="sxs-lookup"><span data-stu-id="b8fb4-164">version</span></span>|<span data-ttu-id="b8fb4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b8fb4-165">Int32</span></span>|<span data-ttu-id="b8fb4-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-166">Version of the device configuration.</span></span> <span data-ttu-id="b8fb4-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8fb4-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-168">usernameSource</span></span>|[<span data-ttu-id="b8fb4-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b8fb4-170">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b8fb4-171">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b8fb4-172">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b8fb4-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-173">usernameAADSource</span></span>|[<span data-ttu-id="b8fb4-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="b8fb4-175">Name des Felds AAD, mit der Benutzername für e-Mail-Profil abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="b8fb4-176">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b8fb4-177">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="b8fb4-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-178">userDomainNameSource</span></span>|[<span data-ttu-id="b8fb4-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="b8fb4-180">UserDomainname-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b8fb4-181">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b8fb4-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b8fb4-182">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="b8fb4-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="b8fb4-183">customDomainName</span></span>|<span data-ttu-id="b8fb4-184">String</span><span class="sxs-lookup"><span data-stu-id="b8fb4-184">String</span></span>|<span data-ttu-id="b8fb4-185">Benutzerdefinierte Domäne Name-Wert beim Generieren von einem e-Mail-Profil vor der Installation auf dem Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="b8fb4-186">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="b8fb4-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="b8fb4-187">accountName</span><span class="sxs-lookup"><span data-stu-id="b8fb4-187">accountName</span></span>|<span data-ttu-id="b8fb4-188">String</span><span class="sxs-lookup"><span data-stu-id="b8fb4-188">String</span></span>|<span data-ttu-id="b8fb4-189">Name des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-189">Account name.</span></span>|
|<span data-ttu-id="b8fb4-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b8fb4-190">authenticationMethod</span></span>|[<span data-ttu-id="b8fb4-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b8fb4-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b8fb4-192">Authentifizierungsmethode für dieses E-Mail-Profil.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="b8fb4-193">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="b8fb4-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="b8fb4-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="b8fb4-195">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-195">Boolean</span></span>|<span data-ttu-id="b8fb4-196">Gibt an, ob das Verschieben von Nachrichten an andere e-Mail-Konten zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="b8fb4-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="b8fb4-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="b8fb4-198">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-198">Boolean</span></span>|<span data-ttu-id="b8fb4-199">Gibt an, ob sendende e-Mail von Drittanbieter-apps zu sperren.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="b8fb4-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="b8fb4-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="b8fb4-201">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-201">Boolean</span></span>|<span data-ttu-id="b8fb4-202">Gibt an, ob Synchronisierung zuletzt verwendete e-Mail-Adressen, beispielsweise - blockieren, wenn die neue e-Mails verfassen.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="b8fb4-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="b8fb4-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="b8fb4-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b8fb4-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b8fb4-205">Dauer der Zeit e-Mail sollte wieder auf synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="b8fb4-206">.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-206"></span></span> <span data-ttu-id="b8fb4-207">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b8fb4-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-208">emailAddressSource</span></span>|[<span data-ttu-id="b8fb4-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="b8fb4-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b8fb4-210">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b8fb4-211">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b8fb4-212">hostName</span><span class="sxs-lookup"><span data-stu-id="b8fb4-212">hostName</span></span>|<span data-ttu-id="b8fb4-213">String</span><span class="sxs-lookup"><span data-stu-id="b8fb4-213">String</span></span>|<span data-ttu-id="b8fb4-214">Exchange-Speicherort (URL), die die systemeigene Mail-app stellt eine Verbindung zur.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="b8fb4-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="b8fb4-215">requireSmime</span></span>|<span data-ttu-id="b8fb4-216">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-216">Boolean</span></span>|<span data-ttu-id="b8fb4-217">Gibt an, ob S/MIME-Zertifikat verwenden.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="b8fb4-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="b8fb4-219">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-219">Boolean</span></span>|<span data-ttu-id="b8fb4-220">Gibt an, ob unverschlüsselte-e-Mails zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="b8fb4-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="b8fb4-221">requireSsl</span></span>|<span data-ttu-id="b8fb4-222">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-222">Boolean</span></span>|<span data-ttu-id="b8fb4-223">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="b8fb4-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="b8fb4-224">useOAuth</span></span>|<span data-ttu-id="b8fb4-225">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b8fb4-225">Boolean</span></span>|<span data-ttu-id="b8fb4-226">Gibt an, ob die Verbindung OAuth für die Authentifizierung verwenden soll.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="b8fb4-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8fb4-227">Response</span></span>
<span data-ttu-id="b8fb4-228">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-228">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8fb4-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8fb4-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8fb4-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8fb4-230">Request</span></span>
<span data-ttu-id="b8fb4-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "requireSsl": true,
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="b8fb4-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8fb4-232">Response</span></span>
<span data-ttu-id="b8fb4-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8fb4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "requireSsl": true,
  "useOAuth": true
}
```





