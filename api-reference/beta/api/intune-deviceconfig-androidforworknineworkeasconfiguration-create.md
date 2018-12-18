---
title: Erstellen von androidForWorkNineWorkEasConfiguration
description: Erstellen eines neuen AndroidForWorkNineWorkEasConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: f30d9edc6b86de56b5ab283ac9301fbb199ba454
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310969"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="bd5ad-103">Erstellen von androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5ad-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="bd5ad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd5ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd5ad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd5ad-107">Erstellen eines neuen [AndroidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-107">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd5ad-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd5ad-108">Prerequisites</span></span>
<span data-ttu-id="bd5ad-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd5ad-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd5ad-111">Permission type</span></span>|<span data-ttu-id="bd5ad-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd5ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd5ad-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd5ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd5ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd5ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd5ad-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd5ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd5ad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd5ad-116">Not supported.</span></span>|
|<span data-ttu-id="bd5ad-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd5ad-117">Application</span></span>|<span data-ttu-id="bd5ad-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd5ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd5ad-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd5ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd5ad-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd5ad-120">Request headers</span></span>
|<span data-ttu-id="bd5ad-121">Header</span><span class="sxs-lookup"><span data-stu-id="bd5ad-121">Header</span></span>|<span data-ttu-id="bd5ad-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bd5ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd5ad-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bd5ad-123">Authorization</span></span>|<span data-ttu-id="bd5ad-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd5ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd5ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd5ad-125">Accept</span></span>|<span data-ttu-id="bd5ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd5ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5ad-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd5ad-127">Request body</span></span>
<span data-ttu-id="bd5ad-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkNineWorkEasConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-128">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="bd5ad-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkNineWorkEasConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-129">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="bd5ad-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd5ad-130">Property</span></span>|<span data-ttu-id="bd5ad-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bd5ad-131">Type</span></span>|<span data-ttu-id="bd5ad-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd5ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd5ad-133">id</span><span class="sxs-lookup"><span data-stu-id="bd5ad-133">id</span></span>|<span data-ttu-id="bd5ad-134">String</span><span class="sxs-lookup"><span data-stu-id="bd5ad-134">String</span></span>|<span data-ttu-id="bd5ad-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bd5ad-135">Key of the entity.</span></span> <span data-ttu-id="bd5ad-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5ad-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bd5ad-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5ad-138">DateTimeOffset</span></span>|<span data-ttu-id="bd5ad-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bd5ad-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd5ad-141">roleScopeTagIds</span></span>|<span data-ttu-id="bd5ad-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="bd5ad-142">String collection</span></span>|<span data-ttu-id="bd5ad-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd5ad-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bd5ad-145">supportsScopeTags</span></span>|<span data-ttu-id="bd5ad-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd5ad-146">Boolean</span></span>|<span data-ttu-id="bd5ad-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bd5ad-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bd5ad-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bd5ad-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-150">This property is read-only.</span></span> <span data-ttu-id="bd5ad-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5ad-152">createdDateTime</span></span>|<span data-ttu-id="bd5ad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5ad-153">DateTimeOffset</span></span>|<span data-ttu-id="bd5ad-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-154">DateTime the object was created.</span></span> <span data-ttu-id="bd5ad-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-156">description</span><span class="sxs-lookup"><span data-stu-id="bd5ad-156">description</span></span>|<span data-ttu-id="bd5ad-157">String</span><span class="sxs-lookup"><span data-stu-id="bd5ad-157">String</span></span>|<span data-ttu-id="bd5ad-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd5ad-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bd5ad-160">displayName</span></span>|<span data-ttu-id="bd5ad-161">String</span><span class="sxs-lookup"><span data-stu-id="bd5ad-161">String</span></span>|<span data-ttu-id="bd5ad-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd5ad-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-164">Version</span><span class="sxs-lookup"><span data-stu-id="bd5ad-164">version</span></span>|<span data-ttu-id="bd5ad-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5ad-165">Int32</span></span>|<span data-ttu-id="bd5ad-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-166">Version of the device configuration.</span></span> <span data-ttu-id="bd5ad-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd5ad-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bd5ad-168">authenticationMethod</span></span>|[<span data-ttu-id="bd5ad-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bd5ad-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="bd5ad-170">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="bd5ad-171">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bd5ad-172">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="bd5ad-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="bd5ad-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="bd5ad-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="bd5ad-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="bd5ad-175">Dauer des Zeit-e-Mail-sollte mit synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="bd5ad-176">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bd5ad-177">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="bd5ad-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="bd5ad-178">emailAddressSource</span></span>|[<span data-ttu-id="bd5ad-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="bd5ad-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="bd5ad-180">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bd5ad-181">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bd5ad-182">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bd5ad-183">hostName</span><span class="sxs-lookup"><span data-stu-id="bd5ad-183">hostName</span></span>|<span data-ttu-id="bd5ad-184">String</span><span class="sxs-lookup"><span data-stu-id="bd5ad-184">String</span></span>|<span data-ttu-id="bd5ad-185">Exchange-Speicherort (URL), die die Mail-app mit verbindet.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="bd5ad-186">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd5ad-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="bd5ad-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="bd5ad-187">requireSsl</span></span>|<span data-ttu-id="bd5ad-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd5ad-188">Boolean</span></span>|<span data-ttu-id="bd5ad-189">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="bd5ad-190">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd5ad-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="bd5ad-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="bd5ad-191">usernameSource</span></span>|[<span data-ttu-id="bd5ad-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="bd5ad-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="bd5ad-193">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bd5ad-194">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bd5ad-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bd5ad-195">Mögliche Werte: sind `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bd5ad-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="bd5ad-196">syncCalendar</span></span>|<span data-ttu-id="bd5ad-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd5ad-197">Boolean</span></span>|<span data-ttu-id="bd5ad-198">Schaltet den Kalender wird synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="bd5ad-199">Wenn der Wert false im Kalender auf dem Gerät deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="bd5ad-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="bd5ad-200">syncContacts</span></span>|<span data-ttu-id="bd5ad-201">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd5ad-201">Boolean</span></span>|<span data-ttu-id="bd5ad-202">Schaltet die Kontakte werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-202">Toggles syncing contacts.</span></span> <span data-ttu-id="bd5ad-203">Wenn es sich bei Festlegung auf "false" Kontakte auf dem Gerät deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="bd5ad-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="bd5ad-204">syncTasks</span></span>|<span data-ttu-id="bd5ad-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bd5ad-205">Boolean</span></span>|<span data-ttu-id="bd5ad-206">Schaltet Aufgaben werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-206">Toggles syncing tasks.</span></span> <span data-ttu-id="bd5ad-207">Wenn es sich bei Festlegung auf "false" Aufgaben auf dem Gerät deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="bd5ad-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd5ad-208">Response</span></span>
<span data-ttu-id="bd5ad-209">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-209">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd5ad-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd5ad-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd5ad-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd5ad-211">Request</span></span>
<span data-ttu-id="bd5ad-212">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 630

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="bd5ad-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd5ad-213">Response</span></span>
<span data-ttu-id="bd5ad-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd5ad-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 738

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```





