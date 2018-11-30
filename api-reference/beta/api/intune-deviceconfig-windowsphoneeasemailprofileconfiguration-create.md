---
title: Erstellen von windowsPhoneEASEmailProfileConfiguration
description: Erstellen eines neuen WindowsPhoneEASEmailProfileConfiguration-Objekts.
ms.openlocfilehash: 61f260349ec29cc4b8ffa84d4f5186e2ecf711fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061077"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="d086e-103">Erstellen von windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="d086e-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="d086e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d086e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d086e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d086e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d086e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d086e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d086e-107">Erstellen eines neuen [WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d086e-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d086e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d086e-108">Prerequisites</span></span>
<span data-ttu-id="d086e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d086e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d086e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d086e-111">Permission type</span></span>|<span data-ttu-id="d086e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d086e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d086e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d086e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d086e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d086e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d086e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d086e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d086e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d086e-116">Not supported.</span></span>|
|<span data-ttu-id="d086e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d086e-117">Application</span></span>|<span data-ttu-id="d086e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d086e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d086e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d086e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d086e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d086e-120">Request headers</span></span>
|<span data-ttu-id="d086e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d086e-121">Header</span></span>|<span data-ttu-id="d086e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d086e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d086e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d086e-123">Authorization</span></span>|<span data-ttu-id="d086e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d086e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d086e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d086e-125">Accept</span></span>|<span data-ttu-id="d086e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d086e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d086e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d086e-127">Request body</span></span>
<span data-ttu-id="d086e-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsPhoneEASEmailProfileConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d086e-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="d086e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsPhoneEASEmailProfileConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="d086e-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="d086e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d086e-130">Property</span></span>|<span data-ttu-id="d086e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d086e-131">Type</span></span>|<span data-ttu-id="d086e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d086e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d086e-133">id</span><span class="sxs-lookup"><span data-stu-id="d086e-133">id</span></span>|<span data-ttu-id="d086e-134">String</span><span class="sxs-lookup"><span data-stu-id="d086e-134">String</span></span>|<span data-ttu-id="d086e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d086e-135">Key of the entity.</span></span> <span data-ttu-id="d086e-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d086e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d086e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d086e-138">DateTimeOffset</span></span>|<span data-ttu-id="d086e-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d086e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d086e-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d086e-141">roleScopeTagIds</span></span>|<span data-ttu-id="d086e-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d086e-142">String collection</span></span>|<span data-ttu-id="d086e-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="d086e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d086e-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d086e-145">supportsScopeTags</span></span>|<span data-ttu-id="d086e-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d086e-146">Boolean</span></span>|<span data-ttu-id="d086e-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d086e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d086e-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="d086e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d086e-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d086e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d086e-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d086e-150">This property is read-only.</span></span> <span data-ttu-id="d086e-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d086e-152">createdDateTime</span></span>|<span data-ttu-id="d086e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d086e-153">DateTimeOffset</span></span>|<span data-ttu-id="d086e-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d086e-154">DateTime the object was created.</span></span> <span data-ttu-id="d086e-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-156">description</span><span class="sxs-lookup"><span data-stu-id="d086e-156">description</span></span>|<span data-ttu-id="d086e-157">String</span><span class="sxs-lookup"><span data-stu-id="d086e-157">String</span></span>|<span data-ttu-id="d086e-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d086e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d086e-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d086e-160">displayName</span></span>|<span data-ttu-id="d086e-161">String</span><span class="sxs-lookup"><span data-stu-id="d086e-161">String</span></span>|<span data-ttu-id="d086e-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d086e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d086e-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-164">Version</span><span class="sxs-lookup"><span data-stu-id="d086e-164">version</span></span>|<span data-ttu-id="d086e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d086e-165">Int32</span></span>|<span data-ttu-id="d086e-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d086e-166">Version of the device configuration.</span></span> <span data-ttu-id="d086e-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d086e-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d086e-168">usernameSource</span></span>|[<span data-ttu-id="d086e-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d086e-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d086e-170">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d086e-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d086e-171">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d086e-172">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d086e-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d086e-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="d086e-173">usernameAADSource</span></span>|[<span data-ttu-id="d086e-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d086e-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="d086e-175">Name des Felds AAD, mit der Benutzername für e-Mail-Profil abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d086e-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="d086e-176">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d086e-177">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="d086e-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="d086e-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="d086e-178">userDomainNameSource</span></span>|[<span data-ttu-id="d086e-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="d086e-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="d086e-180">UserDomainname-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d086e-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d086e-181">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d086e-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d086e-182">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="d086e-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="d086e-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="d086e-183">customDomainName</span></span>|<span data-ttu-id="d086e-184">String</span><span class="sxs-lookup"><span data-stu-id="d086e-184">String</span></span>|<span data-ttu-id="d086e-185">Benutzerdefinierte Domäne Name-Wert beim Generieren von einem e-Mail-Profil vor der Installation auf dem Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="d086e-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="d086e-186">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="d086e-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="d086e-187">accountName</span><span class="sxs-lookup"><span data-stu-id="d086e-187">accountName</span></span>|<span data-ttu-id="d086e-188">String</span><span class="sxs-lookup"><span data-stu-id="d086e-188">String</span></span>|<span data-ttu-id="d086e-189">Name des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="d086e-189">Account name.</span></span>|
|<span data-ttu-id="d086e-190">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="d086e-190">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="d086e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d086e-191">Boolean</span></span>|<span data-ttu-id="d086e-192">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="d086e-192">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="d086e-193">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d086e-193">This property is read-only.</span></span>|
|<span data-ttu-id="d086e-194">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="d086e-194">syncCalendar</span></span>|<span data-ttu-id="d086e-195">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d086e-195">Boolean</span></span>|<span data-ttu-id="d086e-196">Ob den Kalender synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="d086e-196">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="d086e-197">syncContacts</span><span class="sxs-lookup"><span data-stu-id="d086e-197">syncContacts</span></span>|<span data-ttu-id="d086e-198">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d086e-198">Boolean</span></span>|<span data-ttu-id="d086e-199">Ob Kontakte synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="d086e-199">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="d086e-200">syncTasks</span><span class="sxs-lookup"><span data-stu-id="d086e-200">syncTasks</span></span>|<span data-ttu-id="d086e-201">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d086e-201">Boolean</span></span>|<span data-ttu-id="d086e-202">Ob Sie Vorgänge synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="d086e-202">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="d086e-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d086e-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="d086e-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d086e-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d086e-205">Dauer der e-Mails zu synchronisieren. Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d086e-205">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d086e-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="d086e-206">emailAddressSource</span></span>|[<span data-ttu-id="d086e-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d086e-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d086e-208">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d086e-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d086e-209">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d086e-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d086e-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="d086e-210">emailSyncSchedule</span></span>|[<span data-ttu-id="d086e-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="d086e-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="d086e-212">E-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="d086e-212">Email sync schedule.</span></span> <span data-ttu-id="d086e-213">Mögliche Werte sind: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes` und `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="d086e-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="d086e-214">hostName</span><span class="sxs-lookup"><span data-stu-id="d086e-214">hostName</span></span>|<span data-ttu-id="d086e-215">String</span><span class="sxs-lookup"><span data-stu-id="d086e-215">String</span></span>|<span data-ttu-id="d086e-216">Exchange-Speicherort (URL), die die systemeigene Mail-app stellt eine Verbindung zur.</span><span class="sxs-lookup"><span data-stu-id="d086e-216">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="d086e-217">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d086e-217">requireSsl</span></span>|<span data-ttu-id="d086e-218">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d086e-218">Boolean</span></span>|<span data-ttu-id="d086e-219">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="d086e-219">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="d086e-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="d086e-220">Response</span></span>
<span data-ttu-id="d086e-221">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d086e-221">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d086e-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d086e-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="d086e-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d086e-223">Request</span></span>
<span data-ttu-id="d086e-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d086e-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 858

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
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

### <a name="response"></a><span data-ttu-id="d086e-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="d086e-225">Response</span></span>
<span data-ttu-id="d086e-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d086e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 966

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
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





