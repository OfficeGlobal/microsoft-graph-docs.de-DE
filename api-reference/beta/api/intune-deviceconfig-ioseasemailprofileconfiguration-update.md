---
title: IosEasEmailProfileConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosEasEmailProfileConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a82c5efe6a9967de2f20a2e97bbe4b4999ae34a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916761"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="8bca8-103">IosEasEmailProfileConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8bca8-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="8bca8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8bca8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bca8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bca8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bca8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8bca8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bca8-107">Aktualisieren Sie die Eigenschaften eines [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bca8-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bca8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8bca8-108">Prerequisites</span></span>
<span data-ttu-id="8bca8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bca8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bca8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8bca8-111">Permission type</span></span>|<span data-ttu-id="8bca8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8bca8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bca8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8bca8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bca8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bca8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bca8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8bca8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bca8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bca8-116">Not supported.</span></span>|
|<span data-ttu-id="8bca8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8bca8-117">Application</span></span>|<span data-ttu-id="8bca8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bca8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bca8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bca8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8bca8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8bca8-120">Request headers</span></span>
|<span data-ttu-id="8bca8-121">Header</span><span class="sxs-lookup"><span data-stu-id="8bca8-121">Header</span></span>|<span data-ttu-id="8bca8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bca8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bca8-123">Authorization</span></span>|<span data-ttu-id="8bca8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8bca8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bca8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8bca8-125">Accept</span></span>|<span data-ttu-id="8bca8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bca8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bca8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8bca8-127">Request body</span></span>
<span data-ttu-id="8bca8-128">Geben Sie im Textkörper Anforderung für das Objekt [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8bca8-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="8bca8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8bca8-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="8bca8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8bca8-130">Property</span></span>|<span data-ttu-id="8bca8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8bca8-131">Type</span></span>|<span data-ttu-id="8bca8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bca8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bca8-133">id</span><span class="sxs-lookup"><span data-stu-id="8bca8-133">id</span></span>|<span data-ttu-id="8bca8-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bca8-134">String</span></span>|<span data-ttu-id="8bca8-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8bca8-135">Key of the entity.</span></span> <span data-ttu-id="8bca8-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bca8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8bca8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bca8-138">DateTimeOffset</span></span>|<span data-ttu-id="8bca8-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bca8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8bca8-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8bca8-141">roleScopeTagIds</span></span>|<span data-ttu-id="8bca8-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="8bca8-142">String collection</span></span>|<span data-ttu-id="8bca8-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8bca8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8bca8-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8bca8-145">supportsScopeTags</span></span>|<span data-ttu-id="8bca8-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-146">Boolean</span></span>|<span data-ttu-id="8bca8-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bca8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8bca8-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8bca8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8bca8-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="8bca8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8bca8-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8bca8-150">This property is read-only.</span></span> <span data-ttu-id="8bca8-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bca8-152">createdDateTime</span></span>|<span data-ttu-id="8bca8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bca8-153">DateTimeOffset</span></span>|<span data-ttu-id="8bca8-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bca8-154">DateTime the object was created.</span></span> <span data-ttu-id="8bca8-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-156">description</span><span class="sxs-lookup"><span data-stu-id="8bca8-156">description</span></span>|<span data-ttu-id="8bca8-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bca8-157">String</span></span>|<span data-ttu-id="8bca8-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8bca8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8bca8-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8bca8-160">displayName</span></span>|<span data-ttu-id="8bca8-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bca8-161">String</span></span>|<span data-ttu-id="8bca8-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8bca8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8bca8-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-164">Version</span><span class="sxs-lookup"><span data-stu-id="8bca8-164">version</span></span>|<span data-ttu-id="8bca8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8bca8-165">Int32</span></span>|<span data-ttu-id="8bca8-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8bca8-166">Version of the device configuration.</span></span> <span data-ttu-id="8bca8-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bca8-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-168">usernameSource</span></span>|[<span data-ttu-id="8bca8-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8bca8-170">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="8bca8-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8bca8-171">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8bca8-172">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="8bca8-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8bca8-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-173">usernameAADSource</span></span>|[<span data-ttu-id="8bca8-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="8bca8-175">Name des Felds AAD, mit der Benutzername für e-Mail-Profil abgerufen.</span><span class="sxs-lookup"><span data-stu-id="8bca8-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="8bca8-176">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8bca8-177">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="8bca8-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="8bca8-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-178">userDomainNameSource</span></span>|[<span data-ttu-id="8bca8-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="8bca8-180">UserDomainname-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="8bca8-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8bca8-181">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8bca8-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8bca8-182">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="8bca8-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="8bca8-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="8bca8-183">customDomainName</span></span>|<span data-ttu-id="8bca8-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bca8-184">String</span></span>|<span data-ttu-id="8bca8-185">Benutzerdefinierte Domäne Name-Wert beim Generieren von einem e-Mail-Profil vor der Installation auf dem Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="8bca8-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="8bca8-186">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="8bca8-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="8bca8-187">accountName</span><span class="sxs-lookup"><span data-stu-id="8bca8-187">accountName</span></span>|<span data-ttu-id="8bca8-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bca8-188">String</span></span>|<span data-ttu-id="8bca8-189">Name des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="8bca8-189">Account name.</span></span>|
|<span data-ttu-id="8bca8-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8bca8-190">authenticationMethod</span></span>|[<span data-ttu-id="8bca8-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8bca8-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="8bca8-192">Authentifizierungsmethode für dieses E-Mail-Profil.</span><span class="sxs-lookup"><span data-stu-id="8bca8-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="8bca8-193">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="8bca8-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="8bca8-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="8bca8-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="8bca8-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-195">Boolean</span></span>|<span data-ttu-id="8bca8-196">Gibt an, ob das Verschieben von Nachrichten an andere e-Mail-Konten zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="8bca8-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="8bca8-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="8bca8-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="8bca8-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-198">Boolean</span></span>|<span data-ttu-id="8bca8-199">Gibt an, ob sendende e-Mail von Drittanbieter-apps zu sperren.</span><span class="sxs-lookup"><span data-stu-id="8bca8-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="8bca8-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="8bca8-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="8bca8-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-201">Boolean</span></span>|<span data-ttu-id="8bca8-202">Gibt an, ob Synchronisierung zuletzt verwendete e-Mail-Adressen, beispielsweise - blockieren, wenn die neue e-Mails verfassen.</span><span class="sxs-lookup"><span data-stu-id="8bca8-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="8bca8-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="8bca8-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="8bca8-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="8bca8-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="8bca8-205">Dauer der Zeit e-Mail sollte wieder auf synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="8bca8-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="8bca8-206">.</span><span class="sxs-lookup"><span data-stu-id="8bca8-206"></span></span> <span data-ttu-id="8bca8-207">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="8bca8-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="8bca8-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-208">emailAddressSource</span></span>|[<span data-ttu-id="8bca8-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8bca8-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8bca8-210">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="8bca8-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8bca8-211">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="8bca8-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8bca8-212">hostName</span><span class="sxs-lookup"><span data-stu-id="8bca8-212">hostName</span></span>|<span data-ttu-id="8bca8-213">String</span><span class="sxs-lookup"><span data-stu-id="8bca8-213">String</span></span>|<span data-ttu-id="8bca8-214">Exchange-Speicherort (URL), die die systemeigene Mail-app stellt eine Verbindung zur.</span><span class="sxs-lookup"><span data-stu-id="8bca8-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="8bca8-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="8bca8-215">requireSmime</span></span>|<span data-ttu-id="8bca8-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-216">Boolean</span></span>|<span data-ttu-id="8bca8-217">Gibt an, ob S/MIME-Zertifikat verwenden.</span><span class="sxs-lookup"><span data-stu-id="8bca8-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="8bca8-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="8bca8-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="8bca8-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-219">Boolean</span></span>|<span data-ttu-id="8bca8-220">Gibt an, ob unverschlüsselte-e-Mails zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="8bca8-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="8bca8-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="8bca8-221">requireSsl</span></span>|<span data-ttu-id="8bca8-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-222">Boolean</span></span>|<span data-ttu-id="8bca8-223">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="8bca8-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="8bca8-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="8bca8-224">useOAuth</span></span>|<span data-ttu-id="8bca8-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8bca8-225">Boolean</span></span>|<span data-ttu-id="8bca8-226">Gibt an, ob die Verbindung OAuth für die Authentifizierung verwenden soll.</span><span class="sxs-lookup"><span data-stu-id="8bca8-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="8bca8-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bca8-227">Response</span></span>
<span data-ttu-id="8bca8-228">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8bca8-228">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bca8-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8bca8-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bca8-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bca8-230">Request</span></span>
<span data-ttu-id="8bca8-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8bca8-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 904

{
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

### <a name="response"></a><span data-ttu-id="8bca8-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bca8-232">Response</span></span>
<span data-ttu-id="8bca8-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8bca8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





