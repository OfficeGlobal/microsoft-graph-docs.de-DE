---
title: Erstellen von windows10EasEmailProfileConfiguration
description: Erstellen eines neuen windows10EasEmailProfileConfiguration-Objekts.
ms.openlocfilehash: 8c3eed8547de75538cfce2a7260deaa0a67fa407
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061105"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="b836a-103">Erstellen von windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="b836a-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="b836a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b836a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b836a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b836a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b836a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b836a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b836a-107">Erstellen eines neuen [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b836a-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b836a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b836a-108">Prerequisites</span></span>
<span data-ttu-id="b836a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b836a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b836a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b836a-111">Permission type</span></span>|<span data-ttu-id="b836a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b836a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b836a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b836a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b836a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b836a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b836a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b836a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b836a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b836a-116">Not supported.</span></span>|
|<span data-ttu-id="b836a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b836a-117">Application</span></span>|<span data-ttu-id="b836a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b836a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b836a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b836a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b836a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b836a-120">Request headers</span></span>
|<span data-ttu-id="b836a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b836a-121">Header</span></span>|<span data-ttu-id="b836a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b836a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b836a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b836a-123">Authorization</span></span>|<span data-ttu-id="b836a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b836a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b836a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b836a-125">Accept</span></span>|<span data-ttu-id="b836a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b836a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b836a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b836a-127">Request body</span></span>
<span data-ttu-id="b836a-128">Geben Sie im Textkörper Anforderung für das Objekt windows10EasEmailProfileConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b836a-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="b836a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10EasEmailProfileConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="b836a-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="b836a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b836a-130">Property</span></span>|<span data-ttu-id="b836a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b836a-131">Type</span></span>|<span data-ttu-id="b836a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b836a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b836a-133">id</span><span class="sxs-lookup"><span data-stu-id="b836a-133">id</span></span>|<span data-ttu-id="b836a-134">String</span><span class="sxs-lookup"><span data-stu-id="b836a-134">String</span></span>|<span data-ttu-id="b836a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b836a-135">Key of the entity.</span></span> <span data-ttu-id="b836a-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b836a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b836a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b836a-138">DateTimeOffset</span></span>|<span data-ttu-id="b836a-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b836a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b836a-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b836a-141">roleScopeTagIds</span></span>|<span data-ttu-id="b836a-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b836a-142">String collection</span></span>|<span data-ttu-id="b836a-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b836a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b836a-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b836a-145">supportsScopeTags</span></span>|<span data-ttu-id="b836a-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b836a-146">Boolean</span></span>|<span data-ttu-id="b836a-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b836a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b836a-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b836a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b836a-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b836a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b836a-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b836a-150">This property is read-only.</span></span> <span data-ttu-id="b836a-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b836a-152">createdDateTime</span></span>|<span data-ttu-id="b836a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b836a-153">DateTimeOffset</span></span>|<span data-ttu-id="b836a-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b836a-154">DateTime the object was created.</span></span> <span data-ttu-id="b836a-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-156">description</span><span class="sxs-lookup"><span data-stu-id="b836a-156">description</span></span>|<span data-ttu-id="b836a-157">String</span><span class="sxs-lookup"><span data-stu-id="b836a-157">String</span></span>|<span data-ttu-id="b836a-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b836a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b836a-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b836a-160">displayName</span></span>|<span data-ttu-id="b836a-161">String</span><span class="sxs-lookup"><span data-stu-id="b836a-161">String</span></span>|<span data-ttu-id="b836a-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b836a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b836a-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-164">Version</span><span class="sxs-lookup"><span data-stu-id="b836a-164">version</span></span>|<span data-ttu-id="b836a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b836a-165">Int32</span></span>|<span data-ttu-id="b836a-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b836a-166">Version of the device configuration.</span></span> <span data-ttu-id="b836a-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b836a-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b836a-168">usernameSource</span></span>|[<span data-ttu-id="b836a-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="b836a-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b836a-170">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b836a-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b836a-171">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b836a-172">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b836a-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b836a-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="b836a-173">usernameAADSource</span></span>|[<span data-ttu-id="b836a-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b836a-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="b836a-175">Name des Felds AAD, mit der Benutzername für e-Mail-Profil abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b836a-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="b836a-176">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b836a-177">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="b836a-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="b836a-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="b836a-178">userDomainNameSource</span></span>|[<span data-ttu-id="b836a-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="b836a-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="b836a-180">UserDomainname-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b836a-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b836a-181">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b836a-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b836a-182">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="b836a-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="b836a-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="b836a-183">customDomainName</span></span>|<span data-ttu-id="b836a-184">String</span><span class="sxs-lookup"><span data-stu-id="b836a-184">String</span></span>|<span data-ttu-id="b836a-185">Benutzerdefinierte Domäne Name-Wert beim Generieren von einem e-Mail-Profil vor der Installation auf dem Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="b836a-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="b836a-186">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="b836a-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="b836a-187">accountName</span><span class="sxs-lookup"><span data-stu-id="b836a-187">accountName</span></span>|<span data-ttu-id="b836a-188">String</span><span class="sxs-lookup"><span data-stu-id="b836a-188">String</span></span>|<span data-ttu-id="b836a-189">Name des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="b836a-189">Account name.</span></span>|
|<span data-ttu-id="b836a-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="b836a-190">syncCalendar</span></span>|<span data-ttu-id="b836a-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b836a-191">Boolean</span></span>|<span data-ttu-id="b836a-192">Ob den Kalender synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="b836a-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="b836a-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="b836a-193">syncContacts</span></span>|<span data-ttu-id="b836a-194">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b836a-194">Boolean</span></span>|<span data-ttu-id="b836a-195">Ob Kontakte synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="b836a-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="b836a-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="b836a-196">syncTasks</span></span>|<span data-ttu-id="b836a-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b836a-197">Boolean</span></span>|<span data-ttu-id="b836a-198">Ob Sie Vorgänge synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="b836a-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="b836a-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="b836a-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="b836a-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b836a-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b836a-201">Dauer der e-Mails zu synchronisieren. Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="b836a-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b836a-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="b836a-202">emailAddressSource</span></span>|[<span data-ttu-id="b836a-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="b836a-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b836a-204">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b836a-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b836a-205">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b836a-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b836a-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="b836a-206">emailSyncSchedule</span></span>|[<span data-ttu-id="b836a-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="b836a-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="b836a-208">E-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="b836a-208">Email sync schedule.</span></span> <span data-ttu-id="b836a-209">Mögliche Werte sind: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes` und `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="b836a-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="b836a-210">hostName</span><span class="sxs-lookup"><span data-stu-id="b836a-210">hostName</span></span>|<span data-ttu-id="b836a-211">String</span><span class="sxs-lookup"><span data-stu-id="b836a-211">String</span></span>|<span data-ttu-id="b836a-212">Exchange-Speicherort (URL), die die systemeigene Mail-app stellt eine Verbindung zur.</span><span class="sxs-lookup"><span data-stu-id="b836a-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="b836a-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="b836a-213">requireSsl</span></span>|<span data-ttu-id="b836a-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b836a-214">Boolean</span></span>|<span data-ttu-id="b836a-215">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="b836a-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="b836a-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="b836a-216">Response</span></span>
<span data-ttu-id="b836a-217">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b836a-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b836a-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b836a-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="b836a-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b836a-219">Request</span></span>
<span data-ttu-id="b836a-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b836a-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="b836a-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="b836a-221">Response</span></span>
<span data-ttu-id="b836a-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b836a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```




