---
title: Erstellen von windowsPhoneEASEmailProfileConfiguration
description: Erstellen eines neuen WindowsPhoneEASEmailProfileConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b304c7b45ef487845a66ee6df74e74195aa46ad3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408558"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="23d6d-103">Erstellen von windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="23d6d-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="23d6d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="23d6d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23d6d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23d6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23d6d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23d6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23d6d-107">Erstellen eines neuen [WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="23d6d-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23d6d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23d6d-108">Prerequisites</span></span>
<span data-ttu-id="23d6d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23d6d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23d6d-111">Permission type</span></span>|<span data-ttu-id="23d6d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23d6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23d6d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23d6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23d6d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23d6d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23d6d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23d6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23d6d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23d6d-116">Not supported.</span></span>|
|<span data-ttu-id="23d6d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23d6d-117">Application</span></span>|<span data-ttu-id="23d6d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23d6d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23d6d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23d6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="23d6d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23d6d-120">Request headers</span></span>
|<span data-ttu-id="23d6d-121">Header</span><span class="sxs-lookup"><span data-stu-id="23d6d-121">Header</span></span>|<span data-ttu-id="23d6d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="23d6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23d6d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="23d6d-123">Authorization</span></span>|<span data-ttu-id="23d6d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23d6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23d6d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="23d6d-125">Accept</span></span>|<span data-ttu-id="23d6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23d6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23d6d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23d6d-127">Request body</span></span>
<span data-ttu-id="23d6d-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsPhoneEASEmailProfileConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="23d6d-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="23d6d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsPhoneEASEmailProfileConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="23d6d-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="23d6d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23d6d-130">Property</span></span>|<span data-ttu-id="23d6d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="23d6d-131">Type</span></span>|<span data-ttu-id="23d6d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23d6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23d6d-133">id</span><span class="sxs-lookup"><span data-stu-id="23d6d-133">id</span></span>|<span data-ttu-id="23d6d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23d6d-134">String</span></span>|<span data-ttu-id="23d6d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="23d6d-135">Key of the entity.</span></span> <span data-ttu-id="23d6d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23d6d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="23d6d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d6d-138">DateTimeOffset</span></span>|<span data-ttu-id="23d6d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="23d6d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="23d6d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23d6d-141">roleScopeTagIds</span></span>|<span data-ttu-id="23d6d-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="23d6d-142">String collection</span></span>|<span data-ttu-id="23d6d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="23d6d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23d6d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23d6d-145">supportsScopeTags</span></span>|<span data-ttu-id="23d6d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d6d-146">Boolean</span></span>|<span data-ttu-id="23d6d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23d6d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23d6d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="23d6d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23d6d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="23d6d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23d6d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="23d6d-150">This property is read-only.</span></span> <span data-ttu-id="23d6d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23d6d-152">createdDateTime</span></span>|<span data-ttu-id="23d6d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d6d-153">DateTimeOffset</span></span>|<span data-ttu-id="23d6d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="23d6d-154">DateTime the object was created.</span></span> <span data-ttu-id="23d6d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-156">description</span><span class="sxs-lookup"><span data-stu-id="23d6d-156">description</span></span>|<span data-ttu-id="23d6d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23d6d-157">String</span></span>|<span data-ttu-id="23d6d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="23d6d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23d6d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="23d6d-160">displayName</span></span>|<span data-ttu-id="23d6d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23d6d-161">String</span></span>|<span data-ttu-id="23d6d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="23d6d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23d6d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-164">Version</span><span class="sxs-lookup"><span data-stu-id="23d6d-164">version</span></span>|<span data-ttu-id="23d6d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="23d6d-165">Int32</span></span>|<span data-ttu-id="23d6d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="23d6d-166">Version of the device configuration.</span></span> <span data-ttu-id="23d6d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23d6d-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-168">usernameSource</span></span>|[<span data-ttu-id="23d6d-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="23d6d-170">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="23d6d-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="23d6d-171">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="23d6d-172">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="23d6d-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="23d6d-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-173">usernameAADSource</span></span>|[<span data-ttu-id="23d6d-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="23d6d-175">Name des Felds AAD, mit der Benutzername für e-Mail-Profil abgerufen.</span><span class="sxs-lookup"><span data-stu-id="23d6d-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="23d6d-176">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="23d6d-177">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="23d6d-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="23d6d-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-178">userDomainNameSource</span></span>|[<span data-ttu-id="23d6d-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="23d6d-180">UserDomainname-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="23d6d-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="23d6d-181">Geerbt von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="23d6d-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="23d6d-182">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="23d6d-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="23d6d-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="23d6d-183">customDomainName</span></span>|<span data-ttu-id="23d6d-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23d6d-184">String</span></span>|<span data-ttu-id="23d6d-185">Benutzerdefinierte Domäne Name-Wert beim Generieren von einem e-Mail-Profil vor der Installation auf dem Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="23d6d-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="23d6d-186">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="23d6d-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="23d6d-187">accountName</span><span class="sxs-lookup"><span data-stu-id="23d6d-187">accountName</span></span>|<span data-ttu-id="23d6d-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23d6d-188">String</span></span>|<span data-ttu-id="23d6d-189">Name des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="23d6d-189">Account name.</span></span>|
|<span data-ttu-id="23d6d-190">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="23d6d-190">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="23d6d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d6d-191">Boolean</span></span>|<span data-ttu-id="23d6d-192">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="23d6d-192">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="23d6d-193">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="23d6d-193">This property is read-only.</span></span>|
|<span data-ttu-id="23d6d-194">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="23d6d-194">syncCalendar</span></span>|<span data-ttu-id="23d6d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d6d-195">Boolean</span></span>|<span data-ttu-id="23d6d-196">Ob den Kalender synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="23d6d-196">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="23d6d-197">syncContacts</span><span class="sxs-lookup"><span data-stu-id="23d6d-197">syncContacts</span></span>|<span data-ttu-id="23d6d-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d6d-198">Boolean</span></span>|<span data-ttu-id="23d6d-199">Ob Kontakte synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="23d6d-199">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="23d6d-200">syncTasks</span><span class="sxs-lookup"><span data-stu-id="23d6d-200">syncTasks</span></span>|<span data-ttu-id="23d6d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d6d-201">Boolean</span></span>|<span data-ttu-id="23d6d-202">Ob Sie Vorgänge synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="23d6d-202">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="23d6d-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="23d6d-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="23d6d-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="23d6d-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="23d6d-205">Dauer der e-Mails zu synchronisieren. Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="23d6d-205">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="23d6d-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-206">emailAddressSource</span></span>|[<span data-ttu-id="23d6d-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="23d6d-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="23d6d-208">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="23d6d-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="23d6d-209">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="23d6d-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="23d6d-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="23d6d-210">emailSyncSchedule</span></span>|[<span data-ttu-id="23d6d-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="23d6d-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="23d6d-212">E-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="23d6d-212">Email sync schedule.</span></span> <span data-ttu-id="23d6d-213">Mögliche Werte sind: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes` und `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="23d6d-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="23d6d-214">hostName</span><span class="sxs-lookup"><span data-stu-id="23d6d-214">hostName</span></span>|<span data-ttu-id="23d6d-215">String</span><span class="sxs-lookup"><span data-stu-id="23d6d-215">String</span></span>|<span data-ttu-id="23d6d-216">Exchange-Speicherort (URL), die die systemeigene Mail-app stellt eine Verbindung zur.</span><span class="sxs-lookup"><span data-stu-id="23d6d-216">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="23d6d-217">requireSsl</span><span class="sxs-lookup"><span data-stu-id="23d6d-217">requireSsl</span></span>|<span data-ttu-id="23d6d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d6d-218">Boolean</span></span>|<span data-ttu-id="23d6d-219">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="23d6d-219">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="23d6d-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="23d6d-220">Response</span></span>
<span data-ttu-id="23d6d-221">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="23d6d-221">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23d6d-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23d6d-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="23d6d-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23d6d-223">Request</span></span>
<span data-ttu-id="23d6d-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23d6d-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 794

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="23d6d-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="23d6d-225">Response</span></span>
<span data-ttu-id="23d6d-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23d6d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




