---
title: AndroidWorkProfileGmailEasConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileGmailEasConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40bfa97e8502b68f92c56c2ba31fcef0084caa1a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142035"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="13de9-103">AndroidWorkProfileGmailEasConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="13de9-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="13de9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13de9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13de9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="13de9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13de9-106">Aktualisieren der Eigenschaften eines [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="13de9-106">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13de9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13de9-107">Prerequisites</span></span>
<span data-ttu-id="13de9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13de9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13de9-110">Permission type</span></span>|<span data-ttu-id="13de9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13de9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13de9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13de9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13de9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13de9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13de9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13de9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13de9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13de9-115">Not supported.</span></span>|
|<span data-ttu-id="13de9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13de9-116">Application</span></span>|<span data-ttu-id="13de9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13de9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13de9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13de9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="13de9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13de9-119">Request headers</span></span>
|<span data-ttu-id="13de9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="13de9-120">Header</span></span>|<span data-ttu-id="13de9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="13de9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13de9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13de9-122">Authorization</span></span>|<span data-ttu-id="13de9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13de9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13de9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="13de9-124">Accept</span></span>|<span data-ttu-id="13de9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13de9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13de9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13de9-126">Request body</span></span>
<span data-ttu-id="13de9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="13de9-127">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="13de9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="13de9-128">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="13de9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13de9-129">Property</span></span>|<span data-ttu-id="13de9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="13de9-130">Type</span></span>|<span data-ttu-id="13de9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13de9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13de9-132">id</span><span class="sxs-lookup"><span data-stu-id="13de9-132">id</span></span>|<span data-ttu-id="13de9-133">string</span><span class="sxs-lookup"><span data-stu-id="13de9-133">String</span></span>|<span data-ttu-id="13de9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="13de9-134">Key of the entity.</span></span> <span data-ttu-id="13de9-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13de9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="13de9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13de9-137">DateTimeOffset</span></span>|<span data-ttu-id="13de9-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="13de9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="13de9-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="13de9-140">roleScopeTagIds</span></span>|<span data-ttu-id="13de9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="13de9-141">String collection</span></span>|<span data-ttu-id="13de9-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="13de9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13de9-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="13de9-144">supportsScopeTags</span></span>|<span data-ttu-id="13de9-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13de9-145">Boolean</span></span>|<span data-ttu-id="13de9-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13de9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="13de9-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="13de9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="13de9-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="13de9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="13de9-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13de9-149">This property is read-only.</span></span> <span data-ttu-id="13de9-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13de9-151">createdDateTime</span></span>|<span data-ttu-id="13de9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13de9-152">DateTimeOffset</span></span>|<span data-ttu-id="13de9-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="13de9-153">DateTime the object was created.</span></span> <span data-ttu-id="13de9-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-155">description</span><span class="sxs-lookup"><span data-stu-id="13de9-155">description</span></span>|<span data-ttu-id="13de9-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13de9-156">String</span></span>|<span data-ttu-id="13de9-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="13de9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13de9-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="13de9-159">displayName</span></span>|<span data-ttu-id="13de9-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13de9-160">String</span></span>|<span data-ttu-id="13de9-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="13de9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13de9-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-163">Version</span><span class="sxs-lookup"><span data-stu-id="13de9-163">version</span></span>|<span data-ttu-id="13de9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="13de9-164">Int32</span></span>|<span data-ttu-id="13de9-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="13de9-165">Version of the device configuration.</span></span> <span data-ttu-id="13de9-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13de9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13de9-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="13de9-167">authenticationMethod</span></span>|[<span data-ttu-id="13de9-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="13de9-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="13de9-169">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="13de9-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="13de9-170">Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="13de9-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13de9-171">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="13de9-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="13de9-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="13de9-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="13de9-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="13de9-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="13de9-174">Uhrzeit, zu der e-Mails synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="13de9-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="13de9-175">Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="13de9-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13de9-176">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="13de9-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="13de9-177">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="13de9-177">emailAddressSource</span></span>|[<span data-ttu-id="13de9-178">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="13de9-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="13de9-179">E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="13de9-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="13de9-180">Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="13de9-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13de9-181">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="13de9-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="13de9-182">hostName</span><span class="sxs-lookup"><span data-stu-id="13de9-182">hostName</span></span>|<span data-ttu-id="13de9-183">String</span><span class="sxs-lookup"><span data-stu-id="13de9-183">String</span></span>|<span data-ttu-id="13de9-184">Exchange-Speicherort (URL), mit dem die Mail-App eine Verbindung herstellt.</span><span class="sxs-lookup"><span data-stu-id="13de9-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="13de9-185">Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13de9-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="13de9-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="13de9-186">requireSsl</span></span>|<span data-ttu-id="13de9-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13de9-187">Boolean</span></span>|<span data-ttu-id="13de9-188">Gibt an, ob SSL verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="13de9-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="13de9-189">Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13de9-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="13de9-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="13de9-190">usernameSource</span></span>|[<span data-ttu-id="13de9-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="13de9-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="13de9-192">UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="13de9-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="13de9-193">Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="13de9-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13de9-194">Mögliche Werte sind: `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="13de9-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="13de9-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="13de9-195">Response</span></span>
<span data-ttu-id="13de9-196">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13de9-196">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13de9-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13de9-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="13de9-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13de9-198">Request</span></span>
<span data-ttu-id="13de9-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13de9-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="13de9-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="13de9-200">Response</span></span>
<span data-ttu-id="13de9-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13de9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
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




