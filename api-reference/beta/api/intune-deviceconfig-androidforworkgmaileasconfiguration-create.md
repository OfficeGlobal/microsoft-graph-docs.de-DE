---
title: Erstellen von androidForWorkGmailEasConfiguration
description: Erstellen eines neuen AndroidForWorkGmailEasConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fd125237e6f2557fece7dc98920e936fcd4d59c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424868"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="a2305-103">Erstellen von androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2305-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="a2305-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a2305-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2305-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2305-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2305-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2305-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2305-107">Erstellen eines neuen [AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2305-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2305-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2305-108">Prerequisites</span></span>
<span data-ttu-id="a2305-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a2305-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2305-111">Permission type</span></span>|<span data-ttu-id="a2305-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2305-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2305-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2305-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2305-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2305-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2305-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2305-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2305-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2305-116">Not supported.</span></span>|
|<span data-ttu-id="a2305-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2305-117">Application</span></span>|<span data-ttu-id="a2305-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2305-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2305-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2305-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2305-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2305-120">Request headers</span></span>
|<span data-ttu-id="a2305-121">Header</span><span class="sxs-lookup"><span data-stu-id="a2305-121">Header</span></span>|<span data-ttu-id="a2305-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a2305-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2305-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a2305-123">Authorization</span></span>|<span data-ttu-id="a2305-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2305-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2305-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a2305-125">Accept</span></span>|<span data-ttu-id="a2305-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2305-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2305-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2305-127">Request body</span></span>
<span data-ttu-id="a2305-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkGmailEasConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a2305-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="a2305-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkGmailEasConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="a2305-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="a2305-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2305-130">Property</span></span>|<span data-ttu-id="a2305-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a2305-131">Type</span></span>|<span data-ttu-id="a2305-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2305-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2305-133">id</span><span class="sxs-lookup"><span data-stu-id="a2305-133">id</span></span>|<span data-ttu-id="a2305-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2305-134">String</span></span>|<span data-ttu-id="a2305-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a2305-135">Key of the entity.</span></span> <span data-ttu-id="a2305-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2305-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a2305-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2305-138">DateTimeOffset</span></span>|<span data-ttu-id="a2305-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2305-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a2305-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2305-141">roleScopeTagIds</span></span>|<span data-ttu-id="a2305-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a2305-142">String collection</span></span>|<span data-ttu-id="a2305-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a2305-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2305-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a2305-145">supportsScopeTags</span></span>|<span data-ttu-id="a2305-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2305-146">Boolean</span></span>|<span data-ttu-id="a2305-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2305-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a2305-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a2305-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a2305-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a2305-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a2305-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a2305-150">This property is read-only.</span></span> <span data-ttu-id="a2305-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2305-152">createdDateTime</span></span>|<span data-ttu-id="a2305-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2305-153">DateTimeOffset</span></span>|<span data-ttu-id="a2305-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2305-154">DateTime the object was created.</span></span> <span data-ttu-id="a2305-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-156">description</span><span class="sxs-lookup"><span data-stu-id="a2305-156">description</span></span>|<span data-ttu-id="a2305-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2305-157">String</span></span>|<span data-ttu-id="a2305-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a2305-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2305-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a2305-160">displayName</span></span>|<span data-ttu-id="a2305-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2305-161">String</span></span>|<span data-ttu-id="a2305-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a2305-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2305-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-164">Version</span><span class="sxs-lookup"><span data-stu-id="a2305-164">version</span></span>|<span data-ttu-id="a2305-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a2305-165">Int32</span></span>|<span data-ttu-id="a2305-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a2305-166">Version of the device configuration.</span></span> <span data-ttu-id="a2305-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2305-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a2305-168">authenticationMethod</span></span>|[<span data-ttu-id="a2305-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a2305-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a2305-170">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a2305-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="a2305-171">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a2305-172">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="a2305-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="a2305-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a2305-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="a2305-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a2305-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a2305-175">Dauer des Zeit-e-Mail-sollte mit synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="a2305-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="a2305-176">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a2305-177">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a2305-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a2305-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="a2305-178">emailAddressSource</span></span>|[<span data-ttu-id="a2305-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a2305-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a2305-180">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="a2305-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a2305-181">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a2305-182">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a2305-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a2305-183">hostName</span><span class="sxs-lookup"><span data-stu-id="a2305-183">hostName</span></span>|<span data-ttu-id="a2305-184">String</span><span class="sxs-lookup"><span data-stu-id="a2305-184">String</span></span>|<span data-ttu-id="a2305-185">Exchange-Speicherort (URL), die die Mail-app mit verbindet.</span><span class="sxs-lookup"><span data-stu-id="a2305-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="a2305-186">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a2305-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a2305-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a2305-187">requireSsl</span></span>|<span data-ttu-id="a2305-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2305-188">Boolean</span></span>|<span data-ttu-id="a2305-189">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="a2305-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="a2305-190">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a2305-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a2305-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a2305-191">usernameSource</span></span>|[<span data-ttu-id="a2305-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="a2305-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="a2305-193">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="a2305-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a2305-194">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2305-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a2305-195">Mögliche Werte sind: `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a2305-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2305-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2305-196">Response</span></span>
<span data-ttu-id="a2305-197">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a2305-197">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2305-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2305-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2305-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2305-199">Request</span></span>
<span data-ttu-id="a2305-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2305-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="a2305-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2305-201">Response</span></span>
<span data-ttu-id="a2305-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2305-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 663

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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
  "usernameSource": "userPrincipalName"
}
```




