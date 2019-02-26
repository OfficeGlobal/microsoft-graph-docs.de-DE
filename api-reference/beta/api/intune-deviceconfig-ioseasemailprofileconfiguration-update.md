---
title: IosEasEmailProfileConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines iosEasEmailProfileConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f43afe6d527230828a3bc75df39ea547926f01b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142518"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="a13ab-103">IosEasEmailProfileConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a13ab-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="a13ab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a13ab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a13ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a13ab-106">Aktualisieren der Eigenschaften eines [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a13ab-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a13ab-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a13ab-107">Prerequisites</span></span>
<span data-ttu-id="a13ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a13ab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a13ab-110">Permission type</span></span>|<span data-ttu-id="a13ab-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a13ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a13ab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a13ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a13ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a13ab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a13ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a13ab-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a13ab-115">Not supported.</span></span>|
|<span data-ttu-id="a13ab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a13ab-116">Application</span></span>|<span data-ttu-id="a13ab-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a13ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a13ab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a13ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a13ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a13ab-119">Request headers</span></span>
|<span data-ttu-id="a13ab-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a13ab-120">Header</span></span>|<span data-ttu-id="a13ab-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a13ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a13ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a13ab-122">Authorization</span></span>|<span data-ttu-id="a13ab-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a13ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a13ab-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a13ab-124">Accept</span></span>|<span data-ttu-id="a13ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a13ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a13ab-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a13ab-126">Request body</span></span>
<span data-ttu-id="a13ab-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a13ab-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="a13ab-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a13ab-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="a13ab-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a13ab-129">Property</span></span>|<span data-ttu-id="a13ab-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a13ab-130">Type</span></span>|<span data-ttu-id="a13ab-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a13ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a13ab-132">id</span><span class="sxs-lookup"><span data-stu-id="a13ab-132">id</span></span>|<span data-ttu-id="a13ab-133">string</span><span class="sxs-lookup"><span data-stu-id="a13ab-133">String</span></span>|<span data-ttu-id="a13ab-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a13ab-134">Key of the entity.</span></span> <span data-ttu-id="a13ab-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a13ab-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a13ab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a13ab-137">DateTimeOffset</span></span>|<span data-ttu-id="a13ab-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a13ab-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a13ab-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="a13ab-140">roleScopeTagIds</span></span>|<span data-ttu-id="a13ab-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a13ab-141">String collection</span></span>|<span data-ttu-id="a13ab-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="a13ab-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a13ab-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a13ab-144">supportsScopeTags</span></span>|<span data-ttu-id="a13ab-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-145">Boolean</span></span>|<span data-ttu-id="a13ab-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a13ab-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="a13ab-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a13ab-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a13ab-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a13ab-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-149">This property is read-only.</span></span> <span data-ttu-id="a13ab-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a13ab-151">createdDateTime</span></span>|<span data-ttu-id="a13ab-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a13ab-152">DateTimeOffset</span></span>|<span data-ttu-id="a13ab-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a13ab-153">DateTime the object was created.</span></span> <span data-ttu-id="a13ab-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-155">description</span><span class="sxs-lookup"><span data-stu-id="a13ab-155">description</span></span>|<span data-ttu-id="a13ab-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a13ab-156">String</span></span>|<span data-ttu-id="a13ab-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a13ab-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a13ab-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a13ab-159">displayName</span></span>|<span data-ttu-id="a13ab-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a13ab-160">String</span></span>|<span data-ttu-id="a13ab-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a13ab-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a13ab-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-163">Version</span><span class="sxs-lookup"><span data-stu-id="a13ab-163">version</span></span>|<span data-ttu-id="a13ab-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a13ab-164">Int32</span></span>|<span data-ttu-id="a13ab-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a13ab-165">Version of the device configuration.</span></span> <span data-ttu-id="a13ab-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a13ab-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a13ab-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-167">usernameSource</span></span>|[<span data-ttu-id="a13ab-168">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a13ab-169">UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="a13ab-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a13ab-170">Von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a13ab-171">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a13ab-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a13ab-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-172">usernameAADSource</span></span>|[<span data-ttu-id="a13ab-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="a13ab-174">Name des AAD-Felds, das zum Abrufen des Benutzernamens für das e-Mail-Profil verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="a13ab-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="a13ab-175">Von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a13ab-176">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="a13ab-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="a13ab-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-177">userDomainNameSource</span></span>|[<span data-ttu-id="a13ab-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="a13ab-179">UserDomainname-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="a13ab-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a13ab-180">Von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a13ab-181">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="a13ab-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="a13ab-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="a13ab-182">customDomainName</span></span>|<span data-ttu-id="a13ab-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a13ab-183">String</span></span>|<span data-ttu-id="a13ab-184">Benutzerdefinierter Domänenname, der beim Generieren eines e-Mail-Profils verwendet wird, bevor es auf dem Gerät installiert wird.</span><span class="sxs-lookup"><span data-stu-id="a13ab-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="a13ab-185">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a13ab-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="a13ab-186">accountName</span><span class="sxs-lookup"><span data-stu-id="a13ab-186">accountName</span></span>|<span data-ttu-id="a13ab-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a13ab-187">String</span></span>|<span data-ttu-id="a13ab-188">Kontoname.</span><span class="sxs-lookup"><span data-stu-id="a13ab-188">Account name.</span></span>|
|<span data-ttu-id="a13ab-189">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a13ab-189">authenticationMethod</span></span>|[<span data-ttu-id="a13ab-190">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a13ab-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a13ab-191">Authentifizierungsmethode für dieses e-Mail-Profil.</span><span class="sxs-lookup"><span data-stu-id="a13ab-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="a13ab-192">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="a13ab-192">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="a13ab-193">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="a13ab-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="a13ab-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-194">Boolean</span></span>|<span data-ttu-id="a13ab-195">Gibt an, ob das Nachrichten in andere e-Mail-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a13ab-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="a13ab-196">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="a13ab-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="a13ab-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-197">Boolean</span></span>|<span data-ttu-id="a13ab-198">Gibt an, ob das Senden von e-Mails von Drittanbieter-apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a13ab-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="a13ab-199">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a13ab-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="a13ab-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-200">Boolean</span></span>|<span data-ttu-id="a13ab-201">Gibt an, ob die Synchronisierung von zuletzt verwendeten e-Mail-Adressen blockiert werden soll, beispielsweise beim Erstellen neuer e-Mails.</span><span class="sxs-lookup"><span data-stu-id="a13ab-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="a13ab-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a13ab-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="a13ab-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a13ab-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a13ab-204">Dauer der Zeit, die e-Mails synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a13ab-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="a13ab-205">.</span><span class="sxs-lookup"><span data-stu-id="a13ab-205"></span></span> <span data-ttu-id="a13ab-206">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a13ab-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a13ab-207">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-207">emailAddressSource</span></span>|[<span data-ttu-id="a13ab-208">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a13ab-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a13ab-209">E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="a13ab-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a13ab-210">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a13ab-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a13ab-211">hostName</span><span class="sxs-lookup"><span data-stu-id="a13ab-211">hostName</span></span>|<span data-ttu-id="a13ab-212">String</span><span class="sxs-lookup"><span data-stu-id="a13ab-212">String</span></span>|<span data-ttu-id="a13ab-213">Exchange-Speicherort (URL), mit dem die systemeigene Mail-App eine Verbindung herstellt.</span><span class="sxs-lookup"><span data-stu-id="a13ab-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="a13ab-214">requireSmime</span><span class="sxs-lookup"><span data-stu-id="a13ab-214">requireSmime</span></span>|<span data-ttu-id="a13ab-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-215">Boolean</span></span>|<span data-ttu-id="a13ab-216">Gibt an, ob S/MIME-Zertifikat verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a13ab-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="a13ab-217">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="a13ab-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="a13ab-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-218">Boolean</span></span>|<span data-ttu-id="a13ab-219">Gibt an, ob unverschlüsselte e-Mails zugelassen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a13ab-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="a13ab-220">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="a13ab-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="a13ab-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-221">Boolean</span></span>|<span data-ttu-id="a13ab-222">Bei Festlegung auf "true" ist die S/MIME-Verschlüsselung standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="a13ab-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="a13ab-223">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="a13ab-223">smimeSigningEnabled</span></span>|<span data-ttu-id="a13ab-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-224">Boolean</span></span>|<span data-ttu-id="a13ab-225">Bei Festlegung auf "true S/MIME Signing" ist für dieses Konto aktiviert</span><span class="sxs-lookup"><span data-stu-id="a13ab-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="a13ab-226">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a13ab-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="a13ab-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-227">Boolean</span></span>|<span data-ttu-id="a13ab-228">Wenn dieser Wert auf true festgelegt ist, kann der Benutzer die S/MIME-Signierung ein-oder ausschalten.</span><span class="sxs-lookup"><span data-stu-id="a13ab-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="a13ab-229">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a13ab-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="a13ab-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-230">Boolean</span></span>|<span data-ttu-id="a13ab-231">Bei Festlegung auf "true" kann der Benutzer die Verschlüsselung standardmäßig umschalten.</span><span class="sxs-lookup"><span data-stu-id="a13ab-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="a13ab-232">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a13ab-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a13ab-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-233">Boolean</span></span>|<span data-ttu-id="a13ab-234">Wenn dieser Wert auf true festgelegt ist, kann der Benutzer die signierende Identität auswählen.</span><span class="sxs-lookup"><span data-stu-id="a13ab-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="a13ab-235">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a13ab-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a13ab-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-236">Boolean</span></span>|<span data-ttu-id="a13ab-237">Wenn dieser Wert auf true festgelegt ist, kann der Benutzer die S/MIME-Verschlüsselungs Identität auswählen.</span><span class="sxs-lookup"><span data-stu-id="a13ab-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="a13ab-238">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a13ab-238">requireSsl</span></span>|<span data-ttu-id="a13ab-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-239">Boolean</span></span>|<span data-ttu-id="a13ab-240">Gibt an, ob SSL verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a13ab-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="a13ab-241">useOAuth</span><span class="sxs-lookup"><span data-stu-id="a13ab-241">useOAuth</span></span>|<span data-ttu-id="a13ab-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13ab-242">Boolean</span></span>|<span data-ttu-id="a13ab-243">Gibt an, ob die Verbindung OAuth für die Authentifizierung verwenden soll.</span><span class="sxs-lookup"><span data-stu-id="a13ab-243">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="a13ab-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="a13ab-244">Response</span></span>
<span data-ttu-id="a13ab-245">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a13ab-245">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a13ab-246">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a13ab-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="a13ab-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a13ab-247">Request</span></span>
<span data-ttu-id="a13ab-248">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a13ab-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1193

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="a13ab-249">Antwort</span><span class="sxs-lookup"><span data-stu-id="a13ab-249">Response</span></span>
<span data-ttu-id="a13ab-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a13ab-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1365

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
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true
}
```




