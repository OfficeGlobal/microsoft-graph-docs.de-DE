---
title: WindowsPhoneEASEmailProfileConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windowsPhoneEASEmailProfileConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5933cbe72f84a1675dd8979134ccadcfa08192a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988126"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="c9795-103">WindowsPhoneEASEmailProfileConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c9795-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="c9795-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9795-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9795-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c9795-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9795-106">Aktualisieren der Eigenschaften eines [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9795-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9795-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9795-107">Prerequisites</span></span>
<span data-ttu-id="c9795-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9795-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9795-110">Permission type</span></span>|<span data-ttu-id="c9795-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9795-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9795-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9795-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9795-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9795-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9795-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9795-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9795-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9795-115">Not supported.</span></span>|
|<span data-ttu-id="c9795-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9795-116">Application</span></span>|<span data-ttu-id="c9795-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9795-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9795-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9795-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c9795-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9795-119">Request headers</span></span>
|<span data-ttu-id="c9795-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9795-120">Header</span></span>|<span data-ttu-id="c9795-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c9795-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9795-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9795-122">Authorization</span></span>|<span data-ttu-id="c9795-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9795-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9795-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9795-124">Accept</span></span>|<span data-ttu-id="c9795-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9795-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9795-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9795-126">Request body</span></span>
<span data-ttu-id="c9795-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c9795-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="c9795-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c9795-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="c9795-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9795-129">Property</span></span>|<span data-ttu-id="c9795-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c9795-130">Type</span></span>|<span data-ttu-id="c9795-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9795-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9795-132">id</span><span class="sxs-lookup"><span data-stu-id="c9795-132">id</span></span>|<span data-ttu-id="c9795-133">String</span><span class="sxs-lookup"><span data-stu-id="c9795-133">String</span></span>|<span data-ttu-id="c9795-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c9795-134">Key of the entity.</span></span> <span data-ttu-id="c9795-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9795-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9795-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9795-137">DateTimeOffset</span></span>|<span data-ttu-id="c9795-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9795-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c9795-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c9795-140">roleScopeTagIds</span></span>|<span data-ttu-id="c9795-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c9795-141">String collection</span></span>|<span data-ttu-id="c9795-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c9795-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9795-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9795-144">supportsScopeTags</span></span>|<span data-ttu-id="c9795-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c9795-145">Boolean</span></span>|<span data-ttu-id="c9795-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9795-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9795-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="c9795-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9795-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c9795-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9795-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c9795-149">This property is read-only.</span></span> <span data-ttu-id="c9795-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9795-151">createdDateTime</span></span>|<span data-ttu-id="c9795-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9795-152">DateTimeOffset</span></span>|<span data-ttu-id="c9795-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9795-153">DateTime the object was created.</span></span> <span data-ttu-id="c9795-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-155">description</span><span class="sxs-lookup"><span data-stu-id="c9795-155">description</span></span>|<span data-ttu-id="c9795-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9795-156">String</span></span>|<span data-ttu-id="c9795-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c9795-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9795-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c9795-159">displayName</span></span>|<span data-ttu-id="c9795-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9795-160">String</span></span>|<span data-ttu-id="c9795-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c9795-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9795-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-163">Version</span><span class="sxs-lookup"><span data-stu-id="c9795-163">version</span></span>|<span data-ttu-id="c9795-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c9795-164">Int32</span></span>|<span data-ttu-id="c9795-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c9795-165">Version of the device configuration.</span></span> <span data-ttu-id="c9795-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9795-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9795-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c9795-167">usernameSource</span></span>|[<span data-ttu-id="c9795-168">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c9795-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c9795-169">UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="c9795-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9795-170">Von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c9795-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c9795-171">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c9795-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c9795-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="c9795-172">usernameAADSource</span></span>|[<span data-ttu-id="c9795-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c9795-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="c9795-174">Name des AAD-Felds, das zum Abrufen des Benutzernamens für das e-Mail-Profil verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c9795-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c9795-175">Von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c9795-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c9795-176">Mögliche Werte sind: `userPrincipalName`, `primarySmtpAddress` und `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="c9795-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c9795-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="c9795-177">userDomainNameSource</span></span>|[<span data-ttu-id="c9795-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="c9795-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="c9795-179">UserDomainname-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="c9795-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9795-180">Von [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c9795-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c9795-181">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="c9795-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c9795-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="c9795-182">customDomainName</span></span>|<span data-ttu-id="c9795-183">String</span><span class="sxs-lookup"><span data-stu-id="c9795-183">String</span></span>|<span data-ttu-id="c9795-184">Benutzerdefinierter Domänenname, der beim Generieren eines e-Mail-Profils verwendet wird, bevor es auf dem Gerät installiert wird.</span><span class="sxs-lookup"><span data-stu-id="c9795-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c9795-185">Geerbt von [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c9795-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c9795-186">accountName</span><span class="sxs-lookup"><span data-stu-id="c9795-186">accountName</span></span>|<span data-ttu-id="c9795-187">String</span><span class="sxs-lookup"><span data-stu-id="c9795-187">String</span></span>|<span data-ttu-id="c9795-188">Kontoname.</span><span class="sxs-lookup"><span data-stu-id="c9795-188">Account name.</span></span>|
|<span data-ttu-id="c9795-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="c9795-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="c9795-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9795-190">Boolean</span></span>|<span data-ttu-id="c9795-191">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="c9795-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c9795-192">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c9795-192">This property is read-only.</span></span>|
|<span data-ttu-id="c9795-193">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="c9795-193">syncCalendar</span></span>|<span data-ttu-id="c9795-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c9795-194">Boolean</span></span>|<span data-ttu-id="c9795-195">Gibt an, ob der Kalender synchronisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c9795-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="c9795-196">syncContacts</span><span class="sxs-lookup"><span data-stu-id="c9795-196">syncContacts</span></span>|<span data-ttu-id="c9795-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c9795-197">Boolean</span></span>|<span data-ttu-id="c9795-198">Gibt an, ob Kontakte synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c9795-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="c9795-199">syncTasks</span><span class="sxs-lookup"><span data-stu-id="c9795-199">syncTasks</span></span>|<span data-ttu-id="c9795-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c9795-200">Boolean</span></span>|<span data-ttu-id="c9795-201">Gibt an, ob Aufgaben synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c9795-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="c9795-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c9795-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="c9795-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c9795-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c9795-204">Dauer der zu synchronisierenden e-Mail. Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="c9795-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c9795-205">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="c9795-205">emailAddressSource</span></span>|[<span data-ttu-id="c9795-206">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c9795-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c9795-207">E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="c9795-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9795-208">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c9795-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c9795-209">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c9795-209">emailSyncSchedule</span></span>|[<span data-ttu-id="c9795-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c9795-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="c9795-211">Zeitplan für die e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="c9795-211">Email sync schedule.</span></span> <span data-ttu-id="c9795-212">Mögliche Werte: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="c9795-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="c9795-213">hostName</span><span class="sxs-lookup"><span data-stu-id="c9795-213">hostName</span></span>|<span data-ttu-id="c9795-214">String</span><span class="sxs-lookup"><span data-stu-id="c9795-214">String</span></span>|<span data-ttu-id="c9795-215">Exchange-Speicherort (URL), mit dem die systemeigene Mail-App eine Verbindung herstellt.</span><span class="sxs-lookup"><span data-stu-id="c9795-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c9795-216">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c9795-216">requireSsl</span></span>|<span data-ttu-id="c9795-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c9795-217">Boolean</span></span>|<span data-ttu-id="c9795-218">Gibt an, ob SSL verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c9795-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="c9795-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9795-219">Response</span></span>
<span data-ttu-id="c9795-220">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c9795-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9795-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9795-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9795-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9795-222">Request</span></span>
<span data-ttu-id="c9795-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9795-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c9795-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9795-224">Response</span></span>
<span data-ttu-id="c9795-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9795-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




