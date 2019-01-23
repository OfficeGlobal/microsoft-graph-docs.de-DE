---
title: AndroidEasEmailProfileConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidEasEmailProfileConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b1cb423ebe3cf5424151f665be3ca682aff5fb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406990"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="0d640-103">AndroidEasEmailProfileConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d640-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="0d640-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0d640-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d640-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d640-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d640-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d640-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d640-107">Aktualisieren Sie die Eigenschaften eines [AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d640-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d640-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d640-108">Prerequisites</span></span>
<span data-ttu-id="0d640-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d640-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d640-111">Permission type</span></span>|<span data-ttu-id="0d640-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d640-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d640-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d640-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d640-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d640-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d640-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d640-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d640-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d640-116">Not supported.</span></span>|
|<span data-ttu-id="0d640-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d640-117">Application</span></span>|<span data-ttu-id="0d640-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d640-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d640-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d640-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0d640-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d640-120">Request headers</span></span>
|<span data-ttu-id="0d640-121">Header</span><span class="sxs-lookup"><span data-stu-id="0d640-121">Header</span></span>|<span data-ttu-id="0d640-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0d640-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d640-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0d640-123">Authorization</span></span>|<span data-ttu-id="0d640-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d640-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d640-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d640-125">Accept</span></span>|<span data-ttu-id="0d640-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d640-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d640-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d640-127">Request body</span></span>
<span data-ttu-id="0d640-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0d640-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="0d640-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0d640-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="0d640-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d640-130">Property</span></span>|<span data-ttu-id="0d640-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0d640-131">Type</span></span>|<span data-ttu-id="0d640-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d640-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d640-133">id</span><span class="sxs-lookup"><span data-stu-id="0d640-133">id</span></span>|<span data-ttu-id="0d640-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d640-134">String</span></span>|<span data-ttu-id="0d640-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0d640-135">Key of the entity.</span></span> <span data-ttu-id="0d640-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d640-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0d640-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d640-138">DateTimeOffset</span></span>|<span data-ttu-id="0d640-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d640-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0d640-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d640-141">roleScopeTagIds</span></span>|<span data-ttu-id="0d640-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0d640-142">String collection</span></span>|<span data-ttu-id="0d640-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0d640-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0d640-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0d640-145">supportsScopeTags</span></span>|<span data-ttu-id="0d640-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-146">Boolean</span></span>|<span data-ttu-id="0d640-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d640-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0d640-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0d640-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0d640-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0d640-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0d640-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0d640-150">This property is read-only.</span></span> <span data-ttu-id="0d640-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d640-152">createdDateTime</span></span>|<span data-ttu-id="0d640-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d640-153">DateTimeOffset</span></span>|<span data-ttu-id="0d640-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d640-154">DateTime the object was created.</span></span> <span data-ttu-id="0d640-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-156">description</span><span class="sxs-lookup"><span data-stu-id="0d640-156">description</span></span>|<span data-ttu-id="0d640-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d640-157">String</span></span>|<span data-ttu-id="0d640-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0d640-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d640-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0d640-160">displayName</span></span>|<span data-ttu-id="0d640-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d640-161">String</span></span>|<span data-ttu-id="0d640-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0d640-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d640-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-164">Version</span><span class="sxs-lookup"><span data-stu-id="0d640-164">version</span></span>|<span data-ttu-id="0d640-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0d640-165">Int32</span></span>|<span data-ttu-id="0d640-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0d640-166">Version of the device configuration.</span></span> <span data-ttu-id="0d640-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d640-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d640-168">accountName</span><span class="sxs-lookup"><span data-stu-id="0d640-168">accountName</span></span>|<span data-ttu-id="0d640-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d640-169">String</span></span>|<span data-ttu-id="0d640-170">Exchange ActiveSync-Kontonamen, Benutzern als Namen des Profils EAS (this) angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0d640-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="0d640-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0d640-171">authenticationMethod</span></span>|[<span data-ttu-id="0d640-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0d640-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0d640-173">Authentifizierungsmethode für Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0d640-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="0d640-174">Mögliche Werte sind: `usernameAndPassword` und `certificate`.</span><span class="sxs-lookup"><span data-stu-id="0d640-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="0d640-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="0d640-175">syncCalendar</span></span>|<span data-ttu-id="0d640-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-176">Boolean</span></span>|<span data-ttu-id="0d640-177">Schaltet den Kalender wird synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="0d640-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="0d640-178">Bei Festlegung auf "false" Kalender auf dem Gerät deaktiviertem.</span><span class="sxs-lookup"><span data-stu-id="0d640-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="0d640-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="0d640-179">syncContacts</span></span>|<span data-ttu-id="0d640-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-180">Boolean</span></span>|<span data-ttu-id="0d640-181">Schaltet die Kontakte werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="0d640-181">Toggles syncing contacts.</span></span> <span data-ttu-id="0d640-182">Wenn es sich bei Festlegung auf "false" Kontakte auf dem Gerät deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="0d640-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="0d640-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="0d640-183">syncTasks</span></span>|<span data-ttu-id="0d640-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-184">Boolean</span></span>|<span data-ttu-id="0d640-185">Schaltet Aufgaben werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="0d640-185">Toggles syncing tasks.</span></span> <span data-ttu-id="0d640-186">Wenn es sich bei Festlegung auf "false" Aufgaben auf dem Gerät deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="0d640-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="0d640-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="0d640-187">syncNotes</span></span>|<span data-ttu-id="0d640-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-188">Boolean</span></span>|<span data-ttu-id="0d640-189">Schaltet Notizen werden synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="0d640-189">Toggles syncing notes.</span></span> <span data-ttu-id="0d640-190">Wenn es sich bei Festlegung auf "false" Notes auf dem Gerät deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="0d640-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="0d640-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0d640-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="0d640-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0d640-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0d640-193">Dauer des Zeit-e-Mail-sollte mit synchronisiert werden.</span><span class="sxs-lookup"><span data-stu-id="0d640-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="0d640-194">Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0d640-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0d640-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="0d640-195">emailAddressSource</span></span>|[<span data-ttu-id="0d640-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0d640-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0d640-197">E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="0d640-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0d640-198">Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0d640-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0d640-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="0d640-199">emailSyncSchedule</span></span>|[<span data-ttu-id="0d640-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="0d640-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="0d640-201">E-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="0d640-201">Email sync schedule.</span></span> <span data-ttu-id="0d640-202">Mögliche Werte sind: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes` und `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="0d640-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="0d640-203">hostName</span><span class="sxs-lookup"><span data-stu-id="0d640-203">hostName</span></span>|<span data-ttu-id="0d640-204">String</span><span class="sxs-lookup"><span data-stu-id="0d640-204">String</span></span>|<span data-ttu-id="0d640-205">Exchange-Speicherort (URL) die systemeigene Mail-app für die Verbindung mit.</span><span class="sxs-lookup"><span data-stu-id="0d640-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="0d640-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="0d640-206">requireSmime</span></span>|<span data-ttu-id="0d640-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-207">Boolean</span></span>|<span data-ttu-id="0d640-208">Gibt an, ob S/MIME-Zertifikat verwenden.</span><span class="sxs-lookup"><span data-stu-id="0d640-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="0d640-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0d640-209">requireSsl</span></span>|<span data-ttu-id="0d640-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d640-210">Boolean</span></span>|<span data-ttu-id="0d640-211">Gibt an, ob SSL verwendet.</span><span class="sxs-lookup"><span data-stu-id="0d640-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="0d640-212">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0d640-212">usernameSource</span></span>|[<span data-ttu-id="0d640-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="0d640-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="0d640-214">Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="0d640-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0d640-215">Mögliche Werte: sind `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0d640-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0d640-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="0d640-216">userDomainNameSource</span></span>|[<span data-ttu-id="0d640-217">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="0d640-217">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="0d640-218">UserDomainname-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="0d640-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0d640-219">Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="0d640-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="0d640-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="0d640-220">customDomainName</span></span>|<span data-ttu-id="0d640-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d640-221">String</span></span>|<span data-ttu-id="0d640-222">Benutzerdefinierte Domäne Name-Wert beim Generieren von einem e-Mail-Profil vor der Installation auf dem Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="0d640-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="0d640-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d640-223">Response</span></span>
<span data-ttu-id="0d640-224">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0d640-224">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d640-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d640-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d640-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d640-226">Request</span></span>
<span data-ttu-id="0d640-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d640-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d640-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d640-228">Response</span></span>
<span data-ttu-id="0d640-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d640-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




