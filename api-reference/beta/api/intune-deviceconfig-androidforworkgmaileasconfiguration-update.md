---
title: AndroidForWorkGmailEasConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkGmailEasConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28bfd939963ada63e3c44c657719028ed22fc995
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401355"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="ae2ff-103">AndroidForWorkGmailEasConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ae2ff-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="ae2ff-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae2ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae2ff-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae2ff-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae2ff-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae2ff-108">Prerequisites</span></span>
<span data-ttu-id="ae2ff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae2ff-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae2ff-111">Permission type</span></span>|<span data-ttu-id="ae2ff-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae2ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae2ff-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae2ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae2ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae2ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae2ff-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae2ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae2ff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae2ff-116">Not supported.</span></span>|
|<span data-ttu-id="ae2ff-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae2ff-117">Application</span></span>|<span data-ttu-id="ae2ff-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae2ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae2ff-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae2ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae2ff-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae2ff-120">Request headers</span></span>
|<span data-ttu-id="ae2ff-121">Header</span><span class="sxs-lookup"><span data-stu-id="ae2ff-121">Header</span></span>|<span data-ttu-id="ae2ff-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ae2ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae2ff-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ae2ff-123">Authorization</span></span>|<span data-ttu-id="ae2ff-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae2ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae2ff-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae2ff-125">Accept</span></span>|<span data-ttu-id="ae2ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae2ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae2ff-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae2ff-127">Request body</span></span>
<span data-ttu-id="ae2ff-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="ae2ff-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="ae2ff-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae2ff-130">Property</span></span>|<span data-ttu-id="ae2ff-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ae2ff-131">Type</span></span>|<span data-ttu-id="ae2ff-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae2ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae2ff-133">id</span><span class="sxs-lookup"><span data-stu-id="ae2ff-133">id</span></span>|<span data-ttu-id="ae2ff-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae2ff-134">String</span></span>|<span data-ttu-id="ae2ff-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ae2ff-135">Key of the entity.</span></span> <span data-ttu-id="ae2ff-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae2ff-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ae2ff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae2ff-138">DateTimeOffset</span></span>|<span data-ttu-id="ae2ff-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ae2ff-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae2ff-141">roleScopeTagIds</span></span>|<span data-ttu-id="ae2ff-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ae2ff-142">String collection</span></span>|<span data-ttu-id="ae2ff-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae2ff-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae2ff-145">supportsScopeTags</span></span>|<span data-ttu-id="ae2ff-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae2ff-146">Boolean</span></span>|<span data-ttu-id="ae2ff-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae2ff-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae2ff-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae2ff-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-150">This property is read-only.</span></span> <span data-ttu-id="ae2ff-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae2ff-152">createdDateTime</span></span>|<span data-ttu-id="ae2ff-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae2ff-153">DateTimeOffset</span></span>|<span data-ttu-id="ae2ff-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-154">DateTime the object was created.</span></span> <span data-ttu-id="ae2ff-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-156">description</span><span class="sxs-lookup"><span data-stu-id="ae2ff-156">description</span></span>|<span data-ttu-id="ae2ff-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae2ff-157">String</span></span>|<span data-ttu-id="ae2ff-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae2ff-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ae2ff-160">displayName</span></span>|<span data-ttu-id="ae2ff-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae2ff-161">String</span></span>|<span data-ttu-id="ae2ff-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae2ff-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-164">Version</span><span class="sxs-lookup"><span data-stu-id="ae2ff-164">version</span></span>|<span data-ttu-id="ae2ff-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ae2ff-165">Int32</span></span>|<span data-ttu-id="ae2ff-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-166">Version of the device configuration.</span></span> <span data-ttu-id="ae2ff-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae2ff-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ae2ff-168">authenticationMethod</span></span>|[<span data-ttu-id="ae2ff-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ae2ff-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="ae2ff-170">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="ae2ff-171">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ae2ff-172">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="ae2ff-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ae2ff-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="ae2ff-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ae2ff-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ae2ff-175">Dauer des Zeit-e-Mail-sollte mit synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="ae2ff-176">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ae2ff-177">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ae2ff-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ae2ff-178">emailAddressSource</span></span>|[<span data-ttu-id="ae2ff-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ae2ff-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ae2ff-180">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ae2ff-181">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ae2ff-182">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ae2ff-183">hostName</span><span class="sxs-lookup"><span data-stu-id="ae2ff-183">hostName</span></span>|<span data-ttu-id="ae2ff-184">String</span><span class="sxs-lookup"><span data-stu-id="ae2ff-184">String</span></span>|<span data-ttu-id="ae2ff-185">Exchange-Speicherort (URL), die die Mail-app mit verbindet.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="ae2ff-186">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ae2ff-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ae2ff-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ae2ff-187">requireSsl</span></span>|<span data-ttu-id="ae2ff-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae2ff-188">Boolean</span></span>|<span data-ttu-id="ae2ff-189">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="ae2ff-190">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ae2ff-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ae2ff-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ae2ff-191">usernameSource</span></span>|[<span data-ttu-id="ae2ff-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="ae2ff-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="ae2ff-193">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ae2ff-194">Geerbt von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ae2ff-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ae2ff-195">Mögliche Werte sind: `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="ae2ff-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae2ff-196">Response</span></span>
<span data-ttu-id="ae2ff-197">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae2ff-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae2ff-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae2ff-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae2ff-199">Request</span></span>
<span data-ttu-id="ae2ff-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ae2ff-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae2ff-201">Response</span></span>
<span data-ttu-id="ae2ff-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae2ff-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




