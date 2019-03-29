---
title: AndroidForWorkNineWorkEasConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidForWorkNineWorkEasConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91979bdff1221960c5c8454787c0f55c5b275d01
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966607"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="b6953-103">AndroidForWorkNineWorkEasConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b6953-103">Update androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="b6953-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6953-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6953-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b6953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6953-106">Aktualisieren der Eigenschaften eines [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b6953-106">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6953-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b6953-107">Prerequisites</span></span>
<span data-ttu-id="b6953-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6953-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6953-110">Permission type</span></span>|<span data-ttu-id="b6953-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6953-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6953-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6953-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6953-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6953-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6953-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6953-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6953-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6953-115">Not supported.</span></span>|
|<span data-ttu-id="b6953-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6953-116">Application</span></span>|<span data-ttu-id="b6953-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6953-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6953-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6953-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b6953-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6953-119">Request headers</span></span>
|<span data-ttu-id="b6953-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b6953-120">Header</span></span>|<span data-ttu-id="b6953-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b6953-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6953-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6953-122">Authorization</span></span>|<span data-ttu-id="b6953-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b6953-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6953-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b6953-124">Accept</span></span>|<span data-ttu-id="b6953-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6953-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6953-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6953-126">Request body</span></span>
<span data-ttu-id="b6953-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b6953-127">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="b6953-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b6953-128">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="b6953-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6953-129">Property</span></span>|<span data-ttu-id="b6953-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b6953-130">Type</span></span>|<span data-ttu-id="b6953-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6953-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6953-132">id</span><span class="sxs-lookup"><span data-stu-id="b6953-132">id</span></span>|<span data-ttu-id="b6953-133">String</span><span class="sxs-lookup"><span data-stu-id="b6953-133">String</span></span>|<span data-ttu-id="b6953-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b6953-134">Key of the entity.</span></span> <span data-ttu-id="b6953-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6953-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b6953-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6953-137">DateTimeOffset</span></span>|<span data-ttu-id="b6953-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b6953-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b6953-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b6953-140">roleScopeTagIds</span></span>|<span data-ttu-id="b6953-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b6953-141">String collection</span></span>|<span data-ttu-id="b6953-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="b6953-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6953-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6953-144">supportsScopeTags</span></span>|<span data-ttu-id="b6953-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6953-145">Boolean</span></span>|<span data-ttu-id="b6953-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6953-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b6953-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="b6953-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b6953-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b6953-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b6953-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b6953-149">This property is read-only.</span></span> <span data-ttu-id="b6953-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6953-151">createdDateTime</span></span>|<span data-ttu-id="b6953-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6953-152">DateTimeOffset</span></span>|<span data-ttu-id="b6953-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b6953-153">DateTime the object was created.</span></span> <span data-ttu-id="b6953-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-155">description</span><span class="sxs-lookup"><span data-stu-id="b6953-155">description</span></span>|<span data-ttu-id="b6953-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6953-156">String</span></span>|<span data-ttu-id="b6953-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b6953-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6953-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b6953-159">displayName</span></span>|<span data-ttu-id="b6953-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6953-160">String</span></span>|<span data-ttu-id="b6953-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b6953-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6953-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-163">Version</span><span class="sxs-lookup"><span data-stu-id="b6953-163">version</span></span>|<span data-ttu-id="b6953-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b6953-164">Int32</span></span>|<span data-ttu-id="b6953-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b6953-165">Version of the device configuration.</span></span> <span data-ttu-id="b6953-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6953-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6953-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b6953-167">authenticationMethod</span></span>|[<span data-ttu-id="b6953-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b6953-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b6953-169">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="b6953-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="b6953-170">Von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b6953-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="b6953-171">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="b6953-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="b6953-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="b6953-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="b6953-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b6953-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b6953-174">Uhrzeit, zu der e-Mails synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b6953-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="b6953-175">Von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b6953-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="b6953-176">Mögliche Werte: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="b6953-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b6953-177">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="b6953-177">emailAddressSource</span></span>|[<span data-ttu-id="b6953-178">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="b6953-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b6953-179">E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b6953-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b6953-180">Von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b6953-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="b6953-181">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b6953-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b6953-182">hostName</span><span class="sxs-lookup"><span data-stu-id="b6953-182">hostName</span></span>|<span data-ttu-id="b6953-183">String</span><span class="sxs-lookup"><span data-stu-id="b6953-183">String</span></span>|<span data-ttu-id="b6953-184">Exchange-Speicherort (URL), mit dem die Mail-App eine Verbindung herstellt.</span><span class="sxs-lookup"><span data-stu-id="b6953-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="b6953-185">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b6953-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b6953-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="b6953-186">requireSsl</span></span>|<span data-ttu-id="b6953-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6953-187">Boolean</span></span>|<span data-ttu-id="b6953-188">Gibt an, ob SSL verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b6953-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="b6953-189">Geerbt von [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b6953-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b6953-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b6953-190">usernameSource</span></span>|[<span data-ttu-id="b6953-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="b6953-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="b6953-192">UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="b6953-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b6953-193">Von [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b6953-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="b6953-194">Mögliche Werte sind: `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b6953-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b6953-195">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="b6953-195">syncCalendar</span></span>|<span data-ttu-id="b6953-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6953-196">Boolean</span></span>|<span data-ttu-id="b6953-197">Schaltet die Synchronisierung des Kalenders ein.</span><span class="sxs-lookup"><span data-stu-id="b6953-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="b6953-198">Bei Festlegung auf false wird der Kalender auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="b6953-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="b6953-199">syncContacts</span><span class="sxs-lookup"><span data-stu-id="b6953-199">syncContacts</span></span>|<span data-ttu-id="b6953-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6953-200">Boolean</span></span>|<span data-ttu-id="b6953-201">Schaltet die Synchronisierungs Kontakte ein.</span><span class="sxs-lookup"><span data-stu-id="b6953-201">Toggles syncing contacts.</span></span> <span data-ttu-id="b6953-202">Bei Festlegung auf false sind Kontakte auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="b6953-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="b6953-203">syncTasks</span><span class="sxs-lookup"><span data-stu-id="b6953-203">syncTasks</span></span>|<span data-ttu-id="b6953-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6953-204">Boolean</span></span>|<span data-ttu-id="b6953-205">Schaltet Synchronisierungsaufgaben um.</span><span class="sxs-lookup"><span data-stu-id="b6953-205">Toggles syncing tasks.</span></span> <span data-ttu-id="b6953-206">Bei Festlegung auf false werden Aufgaben auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="b6953-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="b6953-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6953-207">Response</span></span>
<span data-ttu-id="b6953-208">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b6953-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6953-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6953-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6953-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6953-210">Request</span></span>
<span data-ttu-id="b6953-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6953-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 566

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="b6953-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6953-212">Response</span></span>
<span data-ttu-id="b6953-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6953-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




