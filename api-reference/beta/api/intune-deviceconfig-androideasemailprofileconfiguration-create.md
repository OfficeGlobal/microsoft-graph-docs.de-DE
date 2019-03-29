---
title: AndroidEasEmailProfileConfiguration erstellen
description: Erstellen eines neuen androidEasEmailProfileConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6288feb32a616a3ba0636ce3f6fb61a6585ad2f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964276"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="350df-103">AndroidEasEmailProfileConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="350df-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="350df-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="350df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="350df-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="350df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="350df-106">Erstellen eines neuen [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="350df-106">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="350df-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="350df-107">Prerequisites</span></span>
<span data-ttu-id="350df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="350df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="350df-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="350df-110">Permission type</span></span>|<span data-ttu-id="350df-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="350df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="350df-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="350df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="350df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="350df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="350df-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="350df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="350df-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="350df-115">Not supported.</span></span>|
|<span data-ttu-id="350df-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="350df-116">Application</span></span>|<span data-ttu-id="350df-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="350df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="350df-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="350df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="350df-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="350df-119">Request headers</span></span>
|<span data-ttu-id="350df-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="350df-120">Header</span></span>|<span data-ttu-id="350df-121">Wert</span><span class="sxs-lookup"><span data-stu-id="350df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="350df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="350df-122">Authorization</span></span>|<span data-ttu-id="350df-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="350df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="350df-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="350df-124">Accept</span></span>|<span data-ttu-id="350df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="350df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="350df-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="350df-126">Request body</span></span>
<span data-ttu-id="350df-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidEasEmailProfileConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="350df-127">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="350df-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidEasEmailProfileConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="350df-128">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="350df-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="350df-129">Property</span></span>|<span data-ttu-id="350df-130">Typ</span><span class="sxs-lookup"><span data-stu-id="350df-130">Type</span></span>|<span data-ttu-id="350df-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="350df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="350df-132">id</span><span class="sxs-lookup"><span data-stu-id="350df-132">id</span></span>|<span data-ttu-id="350df-133">String</span><span class="sxs-lookup"><span data-stu-id="350df-133">String</span></span>|<span data-ttu-id="350df-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="350df-134">Key of the entity.</span></span> <span data-ttu-id="350df-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="350df-136">lastModifiedDateTime</span></span>|<span data-ttu-id="350df-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350df-137">DateTimeOffset</span></span>|<span data-ttu-id="350df-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="350df-138">DateTime the object was last modified.</span></span> <span data-ttu-id="350df-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="350df-140">roleScopeTagIds</span></span>|<span data-ttu-id="350df-141">String collection</span><span class="sxs-lookup"><span data-stu-id="350df-141">String collection</span></span>|<span data-ttu-id="350df-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="350df-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="350df-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="350df-144">supportsScopeTags</span></span>|<span data-ttu-id="350df-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-145">Boolean</span></span>|<span data-ttu-id="350df-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="350df-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="350df-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="350df-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="350df-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="350df-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="350df-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="350df-149">This property is read-only.</span></span> <span data-ttu-id="350df-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="350df-151">createdDateTime</span></span>|<span data-ttu-id="350df-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350df-152">DateTimeOffset</span></span>|<span data-ttu-id="350df-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="350df-153">DateTime the object was created.</span></span> <span data-ttu-id="350df-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-155">description</span><span class="sxs-lookup"><span data-stu-id="350df-155">description</span></span>|<span data-ttu-id="350df-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="350df-156">String</span></span>|<span data-ttu-id="350df-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="350df-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="350df-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-159">displayName</span><span class="sxs-lookup"><span data-stu-id="350df-159">displayName</span></span>|<span data-ttu-id="350df-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="350df-160">String</span></span>|<span data-ttu-id="350df-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="350df-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="350df-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-163">Version</span><span class="sxs-lookup"><span data-stu-id="350df-163">version</span></span>|<span data-ttu-id="350df-164">Int32</span><span class="sxs-lookup"><span data-stu-id="350df-164">Int32</span></span>|<span data-ttu-id="350df-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="350df-165">Version of the device configuration.</span></span> <span data-ttu-id="350df-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="350df-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="350df-167">accountName</span><span class="sxs-lookup"><span data-stu-id="350df-167">accountName</span></span>|<span data-ttu-id="350df-168">String</span><span class="sxs-lookup"><span data-stu-id="350df-168">String</span></span>|<span data-ttu-id="350df-169">Exchange ActiveSync-Kontonamen, der den Benutzern als Name des EAS-Profils (dieses) angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="350df-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="350df-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="350df-170">authenticationMethod</span></span>|[<span data-ttu-id="350df-171">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="350df-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="350df-172">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="350df-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="350df-173">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="350df-173">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="350df-174">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="350df-174">syncCalendar</span></span>|<span data-ttu-id="350df-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-175">Boolean</span></span>|<span data-ttu-id="350df-176">Schaltet die Synchronisierung des Kalenders ein.</span><span class="sxs-lookup"><span data-stu-id="350df-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="350df-177">Wenn der Wert auf false festgelegt ist, wird der Kalender auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="350df-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="350df-178">syncContacts</span><span class="sxs-lookup"><span data-stu-id="350df-178">syncContacts</span></span>|<span data-ttu-id="350df-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-179">Boolean</span></span>|<span data-ttu-id="350df-180">Schaltet die Synchronisierungs Kontakte ein.</span><span class="sxs-lookup"><span data-stu-id="350df-180">Toggles syncing contacts.</span></span> <span data-ttu-id="350df-181">Bei Festlegung auf false sind Kontakte auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="350df-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="350df-182">syncTasks</span><span class="sxs-lookup"><span data-stu-id="350df-182">syncTasks</span></span>|<span data-ttu-id="350df-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-183">Boolean</span></span>|<span data-ttu-id="350df-184">Schaltet Synchronisierungsaufgaben um.</span><span class="sxs-lookup"><span data-stu-id="350df-184">Toggles syncing tasks.</span></span> <span data-ttu-id="350df-185">Bei Festlegung auf false werden Aufgaben auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="350df-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="350df-186">syncNotes</span><span class="sxs-lookup"><span data-stu-id="350df-186">syncNotes</span></span>|<span data-ttu-id="350df-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-187">Boolean</span></span>|<span data-ttu-id="350df-188">Schaltet die Synchronisierungs Notizen ein.</span><span class="sxs-lookup"><span data-stu-id="350df-188">Toggles syncing notes.</span></span> <span data-ttu-id="350df-189">Wenn der Wert auf false festgelegt ist, werden die Notizen auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="350df-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="350df-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="350df-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="350df-191">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="350df-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="350df-192">Uhrzeit, zu der e-Mails synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="350df-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="350df-193">Mögliche Werte: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="350df-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="350df-194">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="350df-194">emailAddressSource</span></span>|[<span data-ttu-id="350df-195">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="350df-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="350df-196">E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="350df-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="350df-197">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="350df-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="350df-198">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="350df-198">emailSyncSchedule</span></span>|[<span data-ttu-id="350df-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="350df-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="350df-200">Zeitplan für die e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="350df-200">Email sync schedule.</span></span> <span data-ttu-id="350df-201">Mögliche Werte: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="350df-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="350df-202">hostName</span><span class="sxs-lookup"><span data-stu-id="350df-202">hostName</span></span>|<span data-ttu-id="350df-203">String</span><span class="sxs-lookup"><span data-stu-id="350df-203">String</span></span>|<span data-ttu-id="350df-204">Exchange-Speicherort (URL), mit dem die systemeigene Mail-App eine Verbindung herstellt.</span><span class="sxs-lookup"><span data-stu-id="350df-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="350df-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="350df-205">requireSmime</span></span>|<span data-ttu-id="350df-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-206">Boolean</span></span>|<span data-ttu-id="350df-207">Gibt an, ob S/MIME-Zertifikat verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="350df-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="350df-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="350df-208">requireSsl</span></span>|<span data-ttu-id="350df-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="350df-209">Boolean</span></span>|<span data-ttu-id="350df-210">Gibt an, ob SSL verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="350df-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="350df-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="350df-211">usernameSource</span></span>|[<span data-ttu-id="350df-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="350df-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="350df-213">UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="350df-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="350df-214">Mögliche Werte sind: `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="350df-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="350df-215">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="350df-215">userDomainNameSource</span></span>|[<span data-ttu-id="350df-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="350df-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="350df-217">UserDomainname-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="350df-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="350df-218">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="350df-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="350df-219">customDomainName</span><span class="sxs-lookup"><span data-stu-id="350df-219">customDomainName</span></span>|<span data-ttu-id="350df-220">String</span><span class="sxs-lookup"><span data-stu-id="350df-220">String</span></span>|<span data-ttu-id="350df-221">Benutzerdefinierter Domänenname, der beim Generieren eines e-Mail-Profils verwendet wird, bevor es auf dem Gerät installiert wird.</span><span class="sxs-lookup"><span data-stu-id="350df-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="350df-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="350df-222">Response</span></span>
<span data-ttu-id="350df-223">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="350df-223">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="350df-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="350df-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="350df-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="350df-225">Request</span></span>
<span data-ttu-id="350df-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="350df-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 793

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="350df-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="350df-227">Response</span></span>
<span data-ttu-id="350df-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="350df-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```




