---
title: AndroidWorkProfileGmailEasConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidWorkProfileGmailEasConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 381cadea135bf1c09fb70250283ae829d0c0c65f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394236"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="d97a5-103">AndroidWorkProfileGmailEasConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d97a5-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="d97a5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d97a5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d97a5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d97a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d97a5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d97a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d97a5-107">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d97a5-107">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d97a5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d97a5-108">Prerequisites</span></span>
<span data-ttu-id="d97a5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d97a5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d97a5-111">Permission type</span></span>|<span data-ttu-id="d97a5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d97a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d97a5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d97a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d97a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d97a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d97a5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d97a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d97a5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d97a5-116">Not supported.</span></span>|
|<span data-ttu-id="d97a5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d97a5-117">Application</span></span>|<span data-ttu-id="d97a5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d97a5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d97a5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d97a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d97a5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d97a5-120">Request headers</span></span>
|<span data-ttu-id="d97a5-121">Header</span><span class="sxs-lookup"><span data-stu-id="d97a5-121">Header</span></span>|<span data-ttu-id="d97a5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d97a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d97a5-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d97a5-123">Authorization</span></span>|<span data-ttu-id="d97a5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d97a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d97a5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d97a5-125">Accept</span></span>|<span data-ttu-id="d97a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d97a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d97a5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d97a5-127">Request body</span></span>
<span data-ttu-id="d97a5-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d97a5-128">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="d97a5-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d97a5-129">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="d97a5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d97a5-130">Property</span></span>|<span data-ttu-id="d97a5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d97a5-131">Type</span></span>|<span data-ttu-id="d97a5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d97a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d97a5-133">id</span><span class="sxs-lookup"><span data-stu-id="d97a5-133">id</span></span>|<span data-ttu-id="d97a5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d97a5-134">String</span></span>|<span data-ttu-id="d97a5-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d97a5-135">Key of the entity.</span></span> <span data-ttu-id="d97a5-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d97a5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d97a5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d97a5-138">DateTimeOffset</span></span>|<span data-ttu-id="d97a5-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d97a5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d97a5-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d97a5-141">roleScopeTagIds</span></span>|<span data-ttu-id="d97a5-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d97a5-142">String collection</span></span>|<span data-ttu-id="d97a5-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="d97a5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d97a5-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d97a5-145">supportsScopeTags</span></span>|<span data-ttu-id="d97a5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d97a5-146">Boolean</span></span>|<span data-ttu-id="d97a5-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d97a5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d97a5-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="d97a5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d97a5-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d97a5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d97a5-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d97a5-150">This property is read-only.</span></span> <span data-ttu-id="d97a5-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d97a5-152">createdDateTime</span></span>|<span data-ttu-id="d97a5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d97a5-153">DateTimeOffset</span></span>|<span data-ttu-id="d97a5-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d97a5-154">DateTime the object was created.</span></span> <span data-ttu-id="d97a5-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-156">description</span><span class="sxs-lookup"><span data-stu-id="d97a5-156">description</span></span>|<span data-ttu-id="d97a5-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d97a5-157">String</span></span>|<span data-ttu-id="d97a5-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d97a5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d97a5-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d97a5-160">displayName</span></span>|<span data-ttu-id="d97a5-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d97a5-161">String</span></span>|<span data-ttu-id="d97a5-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d97a5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d97a5-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-164">Version</span><span class="sxs-lookup"><span data-stu-id="d97a5-164">version</span></span>|<span data-ttu-id="d97a5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d97a5-165">Int32</span></span>|<span data-ttu-id="d97a5-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d97a5-166">Version of the device configuration.</span></span> <span data-ttu-id="d97a5-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d97a5-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d97a5-168">authenticationMethod</span></span>|[<span data-ttu-id="d97a5-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d97a5-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d97a5-170">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d97a5-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="d97a5-171">Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d97a5-172">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="d97a5-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="d97a5-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d97a5-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="d97a5-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d97a5-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d97a5-175">Dauer des Zeit-e-Mail-sollte mit synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="d97a5-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="d97a5-176">Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d97a5-177">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d97a5-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d97a5-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="d97a5-178">emailAddressSource</span></span>|[<span data-ttu-id="d97a5-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d97a5-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d97a5-180">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d97a5-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d97a5-181">Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d97a5-182">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d97a5-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d97a5-183">hostName</span><span class="sxs-lookup"><span data-stu-id="d97a5-183">hostName</span></span>|<span data-ttu-id="d97a5-184">String</span><span class="sxs-lookup"><span data-stu-id="d97a5-184">String</span></span>|<span data-ttu-id="d97a5-185">Exchange-Speicherort (URL), die die Mail-app mit verbindet.</span><span class="sxs-lookup"><span data-stu-id="d97a5-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="d97a5-186">Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d97a5-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d97a5-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d97a5-187">requireSsl</span></span>|<span data-ttu-id="d97a5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d97a5-188">Boolean</span></span>|<span data-ttu-id="d97a5-189">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="d97a5-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="d97a5-190">Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d97a5-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d97a5-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d97a5-191">usernameSource</span></span>|[<span data-ttu-id="d97a5-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="d97a5-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="d97a5-193">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d97a5-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d97a5-194">Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d97a5-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d97a5-195">Mögliche Werte sind: `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d97a5-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="d97a5-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="d97a5-196">Response</span></span>
<span data-ttu-id="d97a5-197">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d97a5-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d97a5-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d97a5-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="d97a5-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d97a5-199">Request</span></span>
<span data-ttu-id="d97a5-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d97a5-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d97a5-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="d97a5-201">Response</span></span>
<span data-ttu-id="d97a5-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d97a5-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




