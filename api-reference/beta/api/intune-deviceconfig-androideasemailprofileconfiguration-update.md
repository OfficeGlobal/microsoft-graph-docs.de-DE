---
title: AndroidEasEmailProfileConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidEasEmailProfileConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52e9f239daae0f524c9063fea5d2ac7942c1fe3c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158044"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="df3d2-103">AndroidEasEmailProfileConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="df3d2-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="df3d2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df3d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df3d2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="df3d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df3d2-106">Aktualisieren der Eigenschaften eines [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="df3d2-106">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df3d2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df3d2-107">Prerequisites</span></span>
<span data-ttu-id="df3d2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df3d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df3d2-110">Permission type</span></span>|<span data-ttu-id="df3d2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df3d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df3d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df3d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df3d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df3d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df3d2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df3d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df3d2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df3d2-115">Not supported.</span></span>|
|<span data-ttu-id="df3d2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df3d2-116">Application</span></span>|<span data-ttu-id="df3d2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df3d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df3d2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df3d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="df3d2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df3d2-119">Request headers</span></span>
|<span data-ttu-id="df3d2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="df3d2-120">Header</span></span>|<span data-ttu-id="df3d2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df3d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df3d2-122">Authorization</span></span>|<span data-ttu-id="df3d2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df3d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df3d2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df3d2-124">Accept</span></span>|<span data-ttu-id="df3d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df3d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df3d2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df3d2-126">Request body</span></span>
<span data-ttu-id="df3d2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="df3d2-127">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="df3d2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="df3d2-128">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="df3d2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df3d2-129">Property</span></span>|<span data-ttu-id="df3d2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="df3d2-130">Type</span></span>|<span data-ttu-id="df3d2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df3d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df3d2-132">id</span><span class="sxs-lookup"><span data-stu-id="df3d2-132">id</span></span>|<span data-ttu-id="df3d2-133">string</span><span class="sxs-lookup"><span data-stu-id="df3d2-133">String</span></span>|<span data-ttu-id="df3d2-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="df3d2-134">Key of the entity.</span></span> <span data-ttu-id="df3d2-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df3d2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="df3d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3d2-137">DateTimeOffset</span></span>|<span data-ttu-id="df3d2-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="df3d2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="df3d2-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="df3d2-140">roleScopeTagIds</span></span>|<span data-ttu-id="df3d2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="df3d2-141">String collection</span></span>|<span data-ttu-id="df3d2-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="df3d2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df3d2-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="df3d2-144">supportsScopeTags</span></span>|<span data-ttu-id="df3d2-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-145">Boolean</span></span>|<span data-ttu-id="df3d2-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df3d2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="df3d2-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="df3d2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="df3d2-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="df3d2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="df3d2-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="df3d2-149">This property is read-only.</span></span> <span data-ttu-id="df3d2-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df3d2-151">createdDateTime</span></span>|<span data-ttu-id="df3d2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3d2-152">DateTimeOffset</span></span>|<span data-ttu-id="df3d2-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="df3d2-153">DateTime the object was created.</span></span> <span data-ttu-id="df3d2-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-155">description</span><span class="sxs-lookup"><span data-stu-id="df3d2-155">description</span></span>|<span data-ttu-id="df3d2-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df3d2-156">String</span></span>|<span data-ttu-id="df3d2-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="df3d2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df3d2-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="df3d2-159">displayName</span></span>|<span data-ttu-id="df3d2-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df3d2-160">String</span></span>|<span data-ttu-id="df3d2-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="df3d2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df3d2-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-163">Version</span><span class="sxs-lookup"><span data-stu-id="df3d2-163">version</span></span>|<span data-ttu-id="df3d2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="df3d2-164">Int32</span></span>|<span data-ttu-id="df3d2-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="df3d2-165">Version of the device configuration.</span></span> <span data-ttu-id="df3d2-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df3d2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df3d2-167">accountName</span><span class="sxs-lookup"><span data-stu-id="df3d2-167">accountName</span></span>|<span data-ttu-id="df3d2-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df3d2-168">String</span></span>|<span data-ttu-id="df3d2-169">Exchange ActiveSync-Kontonamen, der den Benutzern als Name des EAS-Profils (dieses) angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="df3d2-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="df3d2-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="df3d2-170">authenticationMethod</span></span>|[<span data-ttu-id="df3d2-171">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="df3d2-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="df3d2-172">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="df3d2-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="df3d2-173">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="df3d2-173">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="df3d2-174">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="df3d2-174">syncCalendar</span></span>|<span data-ttu-id="df3d2-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-175">Boolean</span></span>|<span data-ttu-id="df3d2-176">Schaltet die Synchronisierung des Kalenders ein.</span><span class="sxs-lookup"><span data-stu-id="df3d2-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="df3d2-177">Wenn der Wert auf false festgelegt ist, wird der Kalender auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="df3d2-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="df3d2-178">syncContacts</span><span class="sxs-lookup"><span data-stu-id="df3d2-178">syncContacts</span></span>|<span data-ttu-id="df3d2-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-179">Boolean</span></span>|<span data-ttu-id="df3d2-180">Schaltet die Synchronisierungs Kontakte ein.</span><span class="sxs-lookup"><span data-stu-id="df3d2-180">Toggles syncing contacts.</span></span> <span data-ttu-id="df3d2-181">Bei Festlegung auf false sind Kontakte auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="df3d2-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="df3d2-182">syncTasks</span><span class="sxs-lookup"><span data-stu-id="df3d2-182">syncTasks</span></span>|<span data-ttu-id="df3d2-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-183">Boolean</span></span>|<span data-ttu-id="df3d2-184">Schaltet Synchronisierungsaufgaben um.</span><span class="sxs-lookup"><span data-stu-id="df3d2-184">Toggles syncing tasks.</span></span> <span data-ttu-id="df3d2-185">Bei Festlegung auf false werden Aufgaben auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="df3d2-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="df3d2-186">syncNotes</span><span class="sxs-lookup"><span data-stu-id="df3d2-186">syncNotes</span></span>|<span data-ttu-id="df3d2-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-187">Boolean</span></span>|<span data-ttu-id="df3d2-188">Schaltet die Synchronisierungs Notizen ein.</span><span class="sxs-lookup"><span data-stu-id="df3d2-188">Toggles syncing notes.</span></span> <span data-ttu-id="df3d2-189">Wenn der Wert auf false festgelegt ist, werden die Notizen auf dem Gerät deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="df3d2-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="df3d2-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="df3d2-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="df3d2-191">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="df3d2-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="df3d2-192">Uhrzeit, zu der e-Mails synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="df3d2-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="df3d2-193">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="df3d2-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="df3d2-194">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="df3d2-194">emailAddressSource</span></span>|[<span data-ttu-id="df3d2-195">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="df3d2-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="df3d2-196">E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="df3d2-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="df3d2-197">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="df3d2-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="df3d2-198">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="df3d2-198">emailSyncSchedule</span></span>|[<span data-ttu-id="df3d2-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="df3d2-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="df3d2-200">Zeitplan für die e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="df3d2-200">Email sync schedule.</span></span> <span data-ttu-id="df3d2-201">Mögliche Werte sind: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes` und `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="df3d2-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="df3d2-202">hostName</span><span class="sxs-lookup"><span data-stu-id="df3d2-202">hostName</span></span>|<span data-ttu-id="df3d2-203">String</span><span class="sxs-lookup"><span data-stu-id="df3d2-203">String</span></span>|<span data-ttu-id="df3d2-204">Exchange-Speicherort (URL), mit dem die systemeigene Mail-App eine Verbindung herstellt.</span><span class="sxs-lookup"><span data-stu-id="df3d2-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="df3d2-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="df3d2-205">requireSmime</span></span>|<span data-ttu-id="df3d2-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-206">Boolean</span></span>|<span data-ttu-id="df3d2-207">Gibt an, ob S/MIME-Zertifikat verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="df3d2-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="df3d2-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="df3d2-208">requireSsl</span></span>|<span data-ttu-id="df3d2-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="df3d2-209">Boolean</span></span>|<span data-ttu-id="df3d2-210">Gibt an, ob SSL verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="df3d2-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="df3d2-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="df3d2-211">usernameSource</span></span>|[<span data-ttu-id="df3d2-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="df3d2-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="df3d2-213">UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="df3d2-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="df3d2-214">Mögliche Werte: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="df3d2-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="df3d2-215">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="df3d2-215">userDomainNameSource</span></span>|[<span data-ttu-id="df3d2-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="df3d2-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="df3d2-217">UserDomainname-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="df3d2-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="df3d2-218">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="df3d2-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="df3d2-219">customDomainName</span><span class="sxs-lookup"><span data-stu-id="df3d2-219">customDomainName</span></span>|<span data-ttu-id="df3d2-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df3d2-220">String</span></span>|<span data-ttu-id="df3d2-221">Benutzerdefinierter Domänenname, der beim Generieren eines e-Mail-Profils verwendet wird, bevor es auf dem Gerät installiert wird.</span><span class="sxs-lookup"><span data-stu-id="df3d2-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="df3d2-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="df3d2-222">Response</span></span>
<span data-ttu-id="df3d2-223">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="df3d2-223">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df3d2-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df3d2-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="df3d2-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df3d2-225">Request</span></span>
<span data-ttu-id="df3d2-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df3d2-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="df3d2-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="df3d2-227">Response</span></span>
<span data-ttu-id="df3d2-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df3d2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




