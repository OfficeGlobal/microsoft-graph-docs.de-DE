---
title: Erstellen von „windows10EndpointProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10EndpointProtectionConfiguration.
ms.openlocfilehash: ba6dcb512b2a4989c8b1fe03953f810f390e2670
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064293"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="f3b65-103">Erstellen von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f3b65-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="f3b65-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3b65-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3b65-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3b65-107">Diese Methode erstellt ein neues Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3b65-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3b65-108">Prerequisites</span></span>
<span data-ttu-id="f3b65-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3b65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3b65-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3b65-111">Permission type</span></span>|<span data-ttu-id="f3b65-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3b65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3b65-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3b65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3b65-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b65-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3b65-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3b65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3b65-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3b65-116">Not supported.</span></span>|
|<span data-ttu-id="f3b65-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3b65-117">Application</span></span>|<span data-ttu-id="f3b65-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3b65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3b65-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3b65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3b65-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3b65-120">Request headers</span></span>
|<span data-ttu-id="f3b65-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3b65-121">Header</span></span>|<span data-ttu-id="f3b65-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3b65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3b65-123">Authorization</span></span>|<span data-ttu-id="f3b65-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3b65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3b65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3b65-125">Accept</span></span>|<span data-ttu-id="f3b65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3b65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3b65-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3b65-127">Request body</span></span>
<span data-ttu-id="f3b65-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EndpointProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="f3b65-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="f3b65-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EndpointProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="f3b65-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3b65-130">Property</span></span>|<span data-ttu-id="f3b65-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f3b65-131">Type</span></span>|<span data-ttu-id="f3b65-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3b65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b65-133">id</span><span class="sxs-lookup"><span data-stu-id="f3b65-133">id</span></span>|<span data-ttu-id="f3b65-134">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-134">String</span></span>|<span data-ttu-id="f3b65-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f3b65-135">Key of the entity.</span></span> <span data-ttu-id="f3b65-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3b65-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f3b65-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3b65-138">DateTimeOffset</span></span>|<span data-ttu-id="f3b65-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3b65-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f3b65-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3b65-141">roleScopeTagIds</span></span>|<span data-ttu-id="f3b65-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3b65-142">String collection</span></span>|<span data-ttu-id="f3b65-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f3b65-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f3b65-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f3b65-145">supportsScopeTags</span></span>|<span data-ttu-id="f3b65-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-146">Boolean</span></span>|<span data-ttu-id="f3b65-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f3b65-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f3b65-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f3b65-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-150">This property is read-only.</span></span> <span data-ttu-id="f3b65-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3b65-152">createdDateTime</span></span>|<span data-ttu-id="f3b65-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3b65-153">DateTimeOffset</span></span>|<span data-ttu-id="f3b65-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3b65-154">DateTime the object was created.</span></span> <span data-ttu-id="f3b65-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-156">description</span><span class="sxs-lookup"><span data-stu-id="f3b65-156">description</span></span>|<span data-ttu-id="f3b65-157">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-157">String</span></span>|<span data-ttu-id="f3b65-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f3b65-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3b65-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f3b65-160">displayName</span></span>|<span data-ttu-id="f3b65-161">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-161">String</span></span>|<span data-ttu-id="f3b65-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f3b65-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3b65-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-164">Version</span><span class="sxs-lookup"><span data-stu-id="f3b65-164">version</span></span>|<span data-ttu-id="f3b65-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b65-165">Int32</span></span>|<span data-ttu-id="f3b65-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f3b65-166">Version of the device configuration.</span></span> <span data-ttu-id="f3b65-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3b65-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3b65-168">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="f3b65-168">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="f3b65-169">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-169">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-170">Diese Berechtigung wird während der Sicherung/Wiederherstellung von Anmeldeinformations-Manager verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-170">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="f3b65-171">Gespeicherten Anmeldeinformationen der Benutzer können beeinträchtigt werden, wenn diese Berechtigung für die anderen Entitäten angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-171">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="f3b65-172">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-172">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-173">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f3b65-173">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="f3b65-174">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-174">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-175">Diese Berechtigung bestimmt, welche Benutzer und Gruppen mit dem Computer über das Netzwerk herstellen dürfen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-175">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="f3b65-176">State zugelassen wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-176">State Allowed is supported.</span></span>|
|<span data-ttu-id="f3b65-177">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f3b65-177">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="f3b65-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-179">Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Block aus eine Verbindung mit dem Computer über das Netzwerk sind.</span><span class="sxs-lookup"><span data-stu-id="f3b65-179">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="f3b65-180">State-Block wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-180">State Block is supported.</span></span>|
|<span data-ttu-id="f3b65-181">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3b65-181">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="f3b65-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-183">Diese Berechtigung ermöglicht es einem Prozess zum Identitätswechsel für alle Benutzer ohne Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="f3b65-183">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="f3b65-184">Der Prozess kann daher auf dieselben lokalen Ressourcen wie der Benutzer zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-184">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="f3b65-185">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-185">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-186">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="f3b65-186">userRightsLocalLogOn</span></span>|[<span data-ttu-id="f3b65-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-188">Dieser Benutzer Rechte bestimmt, welche Benutzer am Computer anmelden können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-188">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="f3b65-189">Status nicht konfiguriert, zugelassen und blockiert werden alle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-189">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="f3b65-190">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="f3b65-190">userRightsBackupData</span></span>|[<span data-ttu-id="f3b65-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-192">Diese Rechte Benutzer bestimmt, welche Benutzer Datei-, Verzeichnis-, Registrierung und andere beständige Objekte Berechtigungen beim Sichern der Dateien und Verzeichnisse umgehen können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-192">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="f3b65-193">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-194">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="f3b65-194">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="f3b65-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-196">Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Uhrzeit und Datum der internen Uhr des Computers ändern können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-196">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="f3b65-197">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-198">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="f3b65-198">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="f3b65-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-200">Diese Einstellung bestimmt, ob Benutzer globale Objekte erstellen können, die alle Sitzungen zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-200">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="f3b65-201">Benutzer, die globale Objekte erstellen können, können es sich um Prozesse auswirken, die unter anderer Benutzer Sitzungen, ausgeführt wird und zu Anwendung Fehler und Datenverlust führen kann.</span><span class="sxs-lookup"><span data-stu-id="f3b65-201">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="f3b65-202">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-203">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="f3b65-203">userRightsCreatePageFile</span></span>|[<span data-ttu-id="f3b65-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-205">Diese Berechtigung bestimmt, welche Benutzer und Gruppen können eine interne API zum Erstellen und Ändern der Größe der Auslagerungsdatei aufrufen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-205">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="f3b65-206">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-207">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="f3b65-207">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="f3b65-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-209">Diese Rechte Benutzer bestimmt, welche Konten von Prozessen verwendet werden können, um ein Verzeichnisobjekt mithilfe des Objekts-Manager erstellen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-209">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="f3b65-210">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-211">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="f3b65-211">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="f3b65-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-213">Dieser Benutzer Rechte bestimmt, ob der Benutzer eine symbolische Verbindung vom Computer erstellen kann, an dem sie angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="f3b65-213">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="f3b65-214">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-215">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="f3b65-215">userRightsCreateToken</span></span>|[<span data-ttu-id="f3b65-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-217">Diese Berechtigung bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token erstellen, die Zugriff auf alle lokalen Ressourcen abrufen, wenn der Prozess eine interne API verwendet, um ein Zugriffstoken erstellen verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="f3b65-217">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="f3b65-218">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-219">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="f3b65-219">userRightsDebugPrograms</span></span>|[<span data-ttu-id="f3b65-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-221">Diese Rechte Benutzer bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-221">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="f3b65-222">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3b65-223">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="f3b65-223">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="f3b65-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-225">Diese Berechtigung bestimmt, welche Benutzer und Gruppen nicht zulässig sind, als Remote Desktop Services Client anmelden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-225">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="f3b65-226">Nur die Bundesländer nicht konfiguriert und blockiert werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-226">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="f3b65-227">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="f3b65-227">userRightsDelegation</span></span>|[<span data-ttu-id="f3b65-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-229">Dieser Benutzer Rechte bestimmt, welche Benutzer die vertrauenswürdige für Delegierung Einstellung für ein Benutzer- oder Computerkonto-Objekt festlegen können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-229">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="f3b65-230">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-230">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-231">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="f3b65-231">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="f3b65-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-233">Dieser Benutzer Rechte bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen im Sicherheitsprotokoll verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-233">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="f3b65-234">Sicherheitsprotokoll wird verwendet, um autorisierter Zugriff zu verfolgen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-234">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="f3b65-235">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-235">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-236">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="f3b65-236">userRightsImpersonateClient</span></span>|[<span data-ttu-id="f3b65-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-238">Zuweisen von diesem Benutzerrecht keinem Benutzer kann für diesen Benutzer zum Annehmen der Clientidentität ausgeführte Programme.</span><span class="sxs-lookup"><span data-stu-id="f3b65-238">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="f3b65-239">Voraussetzen dieses Benutzerrecht für diese Art des Identitätswechsels verhindert, dass einen nicht autorisierten Benutzer aus überzeugende einen Client eine Verbindung zu einem Dienst, die sie erstellt haben, und klicken Sie dann Identitätswechsel bei dieser Client, dem der nicht autorisierte Benutzer Berechtigungen zu erhöhen können Administrative oder Systemebenen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-239">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="f3b65-240">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-240">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-241">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="f3b65-241">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="f3b65-242">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-242">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-243">Diese Rechte Benutzer bestimmt, welche Konten einen Prozess mit Schreibzugriff auf einen anderen Prozess verwenden können, um die Ausführungspriorität zugewiesen an den anderen Prozess zu erhöhen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-243">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="f3b65-244">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-245">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="f3b65-245">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="f3b65-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-247">Dieser Benutzer Rechte bestimmt, welche Benutzer können dynamisch laden und entladen Gerätetreiber oder anderen Code im Kernelmodus.</span><span class="sxs-lookup"><span data-stu-id="f3b65-247">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="f3b65-248">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-249">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="f3b65-249">userRightsLockMemory</span></span>|[<span data-ttu-id="f3b65-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-251">Dieser Benutzer Rechte bestimmt, welche Konten einen Prozess Speichern von Daten im physikalischen Speicher, wodurch das System verhindert, dass die Daten in den virtuellen Speicher auf dem Datenträger paging verwenden können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-251">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="f3b65-252">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-253">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="f3b65-253">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="f3b65-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-255">Diese Berechtigung bestimmt, welche Benutzer Objekt den Optionen für einzelne Ressourcen, wie Dateien, Active Directory-Objekte und Registrierungsschlüssel für die Überwachung angeben können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-255">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="f3b65-256">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-257">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="f3b65-257">userRightsManageVolumes</span></span>|[<span data-ttu-id="f3b65-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-259">Diese Rechte Benutzer bestimmt der Benutzer und Gruppen auf einem Datenträger, wie remote Defragmentierung Wartungsaufgaben ausführen können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-259">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="f3b65-260">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-261">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="f3b65-261">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="f3b65-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-263">Diese Berechtigung bestimmt, Firmware-Umgebungsvariablen geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="f3b65-263">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="f3b65-264">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-265">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="f3b65-265">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="f3b65-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-267">Dieser Benutzer Rechte bestimmt, welche Benutzerkonten die Bezeichnung Integrität von Objekten, wie Dateien, Registrierungsschlüssel oder Prozesse, die im Besitz von anderen Benutzern ändern können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-267">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="f3b65-268">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-269">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="f3b65-269">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="f3b65-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-271">Dieser Benutzer Rechte bestimmt, welche Benutzer Tools zum Überwachen der Leistung verwenden können, zur Überwachung der Leistung der Systemprozesse.</span><span class="sxs-lookup"><span data-stu-id="f3b65-271">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="f3b65-272">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-273">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="f3b65-273">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="f3b65-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-275">Dieser Benutzer Rechte bestimmt, welche Benutzer dürfen Herunterfahren eines Computers von einem Remotestandort im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="f3b65-275">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="f3b65-276">Missbrauch dieses Benutzerrechts kann ein Denial-of-Service führen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-276">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="f3b65-277">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-278">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="f3b65-278">userRightsRestoreData</span></span>|[<span data-ttu-id="f3b65-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-280">Diese Berechtigung bestimmt, welche Benutzer umgehen können Datei-, Verzeichnis-, Registrierung und andere beständige Objekte, die Berechtigungen, die beim Wiederherstellen von Dateien und Verzeichnisse gesichert und bestimmt, welche Benutzer einen beliebigen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-280">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="f3b65-281">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-282">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="f3b65-282">userRightsTakeOwnership</span></span>|[<span data-ttu-id="f3b65-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-284">Dieser Benutzer Rechte bestimmt, welche Benutzer die Besitzrechte für ein beliebiges sicherungsfähiges Objekt in das System, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads übernehmen können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-284">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="f3b65-285">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3b65-286">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="f3b65-286">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="f3b65-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3b65-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3b65-288">Diese Einstellung legt fest, welche Dienstkonten für das Registrieren von eines Prozess als Dienst gehindert werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-288">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="f3b65-289">Hinweis: Diese Einstellung gilt nicht für die Konten System, lokaler Dienst oder Netzwerkdienst.</span><span class="sxs-lookup"><span data-stu-id="f3b65-289">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="f3b65-290">Nur Status blockiert wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-290">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="f3b65-291">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="f3b65-291">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="f3b65-292">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-292">Boolean</span></span>|<span data-ttu-id="f3b65-293">Diese Einstellung bestimmt, ob Xbox Spiel speichern aktiviert (1) oder deaktiviert (0) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-293">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="f3b65-294">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3b65-294">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="f3b65-295">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f3b65-295">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3b65-296">Diese Einstellung bestimmt, ob der Verwaltungsdienst Zubehör Starttyp Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-296">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3b65-297">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="f3b65-297">Default: Manual.</span></span> <span data-ttu-id="f3b65-298">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-298">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3b65-299">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3b65-299">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="f3b65-300">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f3b65-300">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3b65-301">Diese Einstellung bestimmt, ob Starttyp Live Auth-Manager-Dienst Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-301">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3b65-302">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="f3b65-302">Default: Manual.</span></span> <span data-ttu-id="f3b65-303">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-303">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3b65-304">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3b65-304">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="f3b65-305">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f3b65-305">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3b65-306">Diese Einstellung bestimmt, ob Live Spiel Speichern des Dienstes Starttyp Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-306">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3b65-307">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="f3b65-307">Default: Manual.</span></span> <span data-ttu-id="f3b65-308">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-308">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3b65-309">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3b65-309">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="f3b65-310">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f3b65-310">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3b65-311">Diese Einstellung bestimmt, ob Starttyp Networking-Dienst Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-311">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3b65-312">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="f3b65-312">Default: Manual.</span></span> <span data-ttu-id="f3b65-313">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-313">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3b65-314">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="f3b65-314">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="f3b65-315">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-315">Boolean</span></span>|<span data-ttu-id="f3b65-316">Hindert Benutzer am Hinzufügen von neuen Microsoft-Konten auf diesem Computer.</span><span class="sxs-lookup"><span data-stu-id="f3b65-316">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="f3b65-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="f3b65-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="f3b65-318">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-318">Boolean</span></span>|<span data-ttu-id="f3b65-319">Aktivieren Sie lokale Konten, die nicht von anderen Orten als physisches Gerät anmelden, um kennwortgeschützte sind. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="f3b65-319">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="f3b65-320">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="f3b65-320">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="f3b65-321">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-321">Boolean</span></span>|<span data-ttu-id="f3b65-322">Bestimmt, ob das lokale Administratorkonto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-322">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="f3b65-323">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="f3b65-323">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="f3b65-324">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-324">String</span></span>|<span data-ttu-id="f3b65-325">Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f3b65-325">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="f3b65-326">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="f3b65-326">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="f3b65-327">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-327">Boolean</span></span>|<span data-ttu-id="f3b65-328">Bestimmt, ob das Konto Gast aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-328">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="f3b65-329">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="f3b65-329">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="f3b65-330">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-330">String</span></span>|<span data-ttu-id="f3b65-331">Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Gast" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f3b65-331">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="f3b65-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="f3b65-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="f3b65-333">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-333">Boolean</span></span>|<span data-ttu-id="f3b65-334">Verhindern Sie, dass eines portablen Computers ohne Anmeldung abgedockt werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-334">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="f3b65-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="f3b65-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="f3b65-336">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-336">Boolean</span></span>|<span data-ttu-id="f3b65-337">Installieren von Druckertreiber als Teil des Herstellens einer Verbindung zu einem freigegebenen Drucker Admins nur zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="f3b65-337">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="f3b65-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="f3b65-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="f3b65-339">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-339">Boolean</span></span>|<span data-ttu-id="f3b65-340">Aktivieren diese Einstellungen kann nur interaktiv angemeldeten Benutzer auf CD-ROM-Medien zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-340">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="f3b65-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="f3b65-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="f3b65-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="f3b65-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="f3b65-343">Definieren Sie, wer berechtigt ist, zu formatieren und NTFS-Wechselmedium ausschließen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-343">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="f3b65-344">Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-344">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f3b65-345">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="f3b65-345">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="f3b65-346">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b65-346">Int32</span></span>|<span data-ttu-id="f3b65-347">Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-347">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f3b65-348">Gültige Werte von 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="f3b65-348">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f3b65-349">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="f3b65-349">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="f3b65-350">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b65-350">Int32</span></span>|<span data-ttu-id="f3b65-351">Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-351">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f3b65-352">Gültige Werte von 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="f3b65-352">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f3b65-353">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="f3b65-353">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="f3b65-354">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-354">Boolean</span></span>|<span data-ttu-id="f3b65-355">Benötigen Sie STRG + ALT + ENTF gedrückt werden, bevor ein Benutzer anmelden kann.</span><span class="sxs-lookup"><span data-stu-id="f3b65-355">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="f3b65-356">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="f3b65-356">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="f3b65-357">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-357">Boolean</span></span>|<span data-ttu-id="f3b65-358">Der Benutzername der letzten Person ein, die Anmeldung auf dem Gerät nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-358">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="f3b65-359">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="f3b65-359">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="f3b65-360">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-360">Boolean</span></span>|<span data-ttu-id="f3b65-361">Der Benutzername der Person, die dieses Gerät anmelden, nachdem Anmeldeinformationen eingegeben wurden und bevor der Desktop des Geräts angezeigt wird nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-361">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="f3b65-362">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="f3b65-362">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="f3b65-363">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-363">String</span></span>|<span data-ttu-id="f3b65-364">Festlegen Sie Titel der Nachricht für Benutzer, die versuchen, melden Sie sich bei.</span><span class="sxs-lookup"><span data-stu-id="f3b65-364">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="f3b65-365">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="f3b65-365">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="f3b65-366">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-366">String</span></span>|<span data-ttu-id="f3b65-367">Festlegen des Nachrichtentexts für Benutzer, die sich anmelden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-367">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="f3b65-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="f3b65-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="f3b65-369">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-369">Boolean</span></span>|<span data-ttu-id="f3b65-370">Block PKU2U authentifizierungsanforderungen an dieses Gerät online-Identitäten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-370">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="f3b65-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="f3b65-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="f3b65-372">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-372">Boolean</span></span>|<span data-ttu-id="f3b65-373">UI-Hilfsprogramm für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager Entität boolean</span><span class="sxs-lookup"><span data-stu-id="f3b65-373">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="f3b65-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="f3b65-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="f3b65-375">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-375">String</span></span>|<span data-ttu-id="f3b65-376">Bearbeiten Sie die Security Descriptor Definition Language Standardzeichenfolge zum gewähren oder verweigern, Benutzer und Gruppen, um die SAM remote anzurufen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-376">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="f3b65-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="f3b65-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="f3b65-378">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f3b65-378">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f3b65-379">Diese Einstellung kann ein Client die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-379">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f3b65-380">Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-380">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f3b65-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="f3b65-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="f3b65-382">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f3b65-382">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f3b65-383">Diese Einstellung kann ein Server die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-383">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f3b65-384">Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-384">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f3b65-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f3b65-385">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="f3b65-386">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f3b65-386">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="f3b65-387">Diese Einstellung bestimmt, welche Herausforderung/Antwort-Authentifizierungsprotokoll Netzwerk Anmeldungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-387">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="f3b65-388">Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-388">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="f3b65-389">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="f3b65-389">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="f3b65-390">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-390">Boolean</span></span>|<span data-ttu-id="f3b65-391">Wenn aktiviert, wird der SMB-Client unsichere Gast Anmeldungen zulassen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-391">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="f3b65-392">Falls nicht konfiguriert, wird der SMB-Client unsichere Gast Anmeldungen abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-392">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="f3b65-393">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="f3b65-393">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="f3b65-394">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-394">Boolean</span></span>|<span data-ttu-id="f3b65-395">Diese Einstellung bestimmt, ob die Auslagerungsdatei beim Herunterfahren des Systems gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-395">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="f3b65-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="f3b65-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="f3b65-397">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-397">Boolean</span></span>|<span data-ttu-id="f3b65-398">Diese Einstellung bestimmt, ob es sich bei ein Computer beendet werden kann, ohne bei Windows anmelden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-398">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="f3b65-399">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="f3b65-399">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="f3b65-400">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-400">Boolean</span></span>|<span data-ttu-id="f3b65-401">Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop.</span><span class="sxs-lookup"><span data-stu-id="f3b65-401">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="f3b65-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="f3b65-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="f3b65-403">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-403">Boolean</span></span>|<span data-ttu-id="f3b65-404">Virtualisieren von Datei- und -Schreibvorgänge mit Fehlern an pro Benutzer Speicherorte</span><span class="sxs-lookup"><span data-stu-id="f3b65-404">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="f3b65-405">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="f3b65-405">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="f3b65-406">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-406">Boolean</span></span>|<span data-ttu-id="f3b65-407">Erzwingen Sie PKI-Zertifizierung Pfad Überprüfung für eine bestimmte ausführbare Datei, bevor er ausführen kann.</span><span class="sxs-lookup"><span data-stu-id="f3b65-407">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="f3b65-408">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f3b65-408">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="f3b65-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f3b65-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="f3b65-410">Definieren Sie das Verhalten der Aufforderung für Administratoren im Administratormodus Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="f3b65-410">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="f3b65-411">Mögliche Werte sind: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent` und `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-411">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="f3b65-412">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f3b65-412">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="f3b65-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f3b65-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="f3b65-414">Definieren Sie das Verhalten der Elevation Ansage für Standardbenutzer.</span><span class="sxs-lookup"><span data-stu-id="f3b65-414">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="f3b65-415">Mögliche Werte: sind `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-415">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="f3b65-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="f3b65-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="f3b65-417">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-417">Boolean</span></span>|<span data-ttu-id="f3b65-418">Aktivieren Sie alle Elevation-Anforderungen, fahren Sie mit dem sicheren Desktop, sondern den interaktiven Desktop des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f3b65-418">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="f3b65-419">Richtlinien für Administratoren und Standardbenutzer Prompt Verhalten dienen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-419">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="f3b65-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="f3b65-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="f3b65-421">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-421">Boolean</span></span>|<span data-ttu-id="f3b65-422">App Installationen mit erhöhte Berechtigungen werden für die Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="f3b65-422">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="f3b65-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="f3b65-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="f3b65-424">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-424">Boolean</span></span>|<span data-ttu-id="f3b65-425">Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="f3b65-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="f3b65-426">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="f3b65-426">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="f3b65-427">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-427">Boolean</span></span>|<span data-ttu-id="f3b65-428">Definiert, ob das integrierte Administratorkonto Administratormodus Genehmigung verwendet oder alle apps mit vollständigen Administratorberechtigungen ausgeführt wird. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="f3b65-428">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="f3b65-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="f3b65-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="f3b65-430">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-430">Boolean</span></span>|<span data-ttu-id="f3b65-431">Definieren Sie, ob Administratormodus Genehmigung und alle UAC-Richtlinieneinstellungen aktiviert sind, ist standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f3b65-431">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="f3b65-432">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f3b65-432">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="f3b65-433">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f3b65-433">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="f3b65-434">Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-434">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f3b65-435">Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-435">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f3b65-436">Mögliche Werte: sind `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-436">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="f3b65-437">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f3b65-437">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="f3b65-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f3b65-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="f3b65-439">Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-439">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f3b65-440">Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-440">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f3b65-441">Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-441">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f3b65-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="f3b65-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="f3b65-443">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-443">Boolean</span></span>|<span data-ttu-id="f3b65-444">Diese Einstellung bestimmt, ob der SMB-Client versucht, SMB-Paketsignatur aushandeln.</span><span class="sxs-lookup"><span data-stu-id="f3b65-444">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="f3b65-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f3b65-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f3b65-446">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-446">Boolean</span></span>|<span data-ttu-id="f3b65-447">Diese Einstellung bestimmt, ob die Clientkomponente für SMB-Paketsignatur erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-447">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="f3b65-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="f3b65-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="f3b65-449">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-449">Boolean</span></span>|<span data-ttu-id="f3b65-450">Wenn diese Einstellung aktiviert ist, kann der Server Message Block (SMB) Redirector nur-Text-Kennwörter an nicht - Microsoft SMB-Server zu senden, die keine für die Verschlüsselung von Kennwörtern während der Authentifizierung Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="f3b65-450">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="f3b65-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f3b65-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f3b65-452">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-452">Boolean</span></span>|<span data-ttu-id="f3b65-453">Diese Einstellung bestimmt, ob die SMB-Server-Komponente Paketsignatur erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-453">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="f3b65-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="f3b65-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="f3b65-455">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-455">Boolean</span></span>|<span data-ttu-id="f3b65-456">Diese Einstellung bestimmt, ob der SMB Server SMB-Paketsignatur mit Clients, die diese anfordern aushandeln kann.</span><span class="sxs-lookup"><span data-stu-id="f3b65-456">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="f3b65-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="f3b65-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="f3b65-458">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-458">Boolean</span></span>|<span data-ttu-id="f3b65-459">Diese Einstellung schränkt standardmäßig anonymen Zugriff auf Freigaben und Pipes an den Einstellungen für named Pipes, die anonym zugegriffen werden können und Freigaben, die anonym zugegriffen werden kann</span><span class="sxs-lookup"><span data-stu-id="f3b65-459">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="f3b65-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="f3b65-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="f3b65-461">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-461">Boolean</span></span>|<span data-ttu-id="f3b65-462">Diese Einstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-462">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="f3b65-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="f3b65-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="f3b65-464">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-464">Boolean</span></span>|<span data-ttu-id="f3b65-465">Diese Einstellung bestimmt, ob anonyme Benutzer zum Ausführen bestimmter Aktivitäten, beispielsweise die Namen von Domänenkonten und Netzwerkfreigaben auflisten können.</span><span class="sxs-lookup"><span data-stu-id="f3b65-465">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="f3b65-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="f3b65-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="f3b65-467">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-467">Boolean</span></span>|<span data-ttu-id="f3b65-468">Diese Einstellung bestimmt, ob, an die nächste Änderung des Kennworts, der Hashwert LAN Manager (LM) für das neue Kennwort gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-468">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="f3b65-469">Es wird nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="f3b65-469">It’s not stored by default.</span></span>|
|<span data-ttu-id="f3b65-470">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="f3b65-470">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="f3b65-471">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f3b65-471">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="f3b65-472">Diese Einstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Leser entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-472">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="f3b65-473">Mögliche Werte: sind `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-473">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="f3b65-474">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-474">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="f3b65-475">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-475">Boolean</span></span>|<span data-ttu-id="f3b65-476">So deaktivieren Sie die Anzeige des Bereichs Protection app und Browser verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-476">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="f3b65-477">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-477">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="f3b65-478">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-478">Boolean</span></span>|<span data-ttu-id="f3b65-479">Verwendet, um die Anzeige des Bereichs-Optionen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f3b65-479">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="f3b65-480">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-480">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="f3b65-481">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-481">Boolean</span></span>|<span data-ttu-id="f3b65-482">So deaktivieren Sie die Anzeige des Geräts Leistung und der Zustand Bereichs verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-482">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="f3b65-483">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-483">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="f3b65-484">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-484">Boolean</span></span>|<span data-ttu-id="f3b65-485">So deaktivieren Sie die Anzeige des Bereichs Protection Firewall und Netzwerk verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-485">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="f3b65-486">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-486">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="f3b65-487">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-487">Boolean</span></span>|<span data-ttu-id="f3b65-488">So deaktivieren Sie die Anzeige des Bereichs Protection Viren und verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-488">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="f3b65-489">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-489">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="f3b65-490">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-490">Boolean</span></span>|<span data-ttu-id="f3b65-491">So deaktivieren Sie die Anzeige des Bereichs Protection Konto verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-491">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="f3b65-492">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-492">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="f3b65-493">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-493">Boolean</span></span>|<span data-ttu-id="f3b65-494">Verwendet, um die Anzeige des Bereichs Protection Hardware zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f3b65-494">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="f3b65-495">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-495">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="f3b65-496">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-496">Boolean</span></span>|<span data-ttu-id="f3b65-497">So deaktivieren Sie die Anzeige des Bereichs Protection Ransomware verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-497">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="f3b65-498">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-498">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="f3b65-499">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-499">Boolean</span></span>|<span data-ttu-id="f3b65-500">So deaktivieren Sie die Anzeige des Bereichs sicheren Boot unter gerätesicherheit verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-500">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="f3b65-501">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="f3b65-501">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="f3b65-502">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-502">Boolean</span></span>|<span data-ttu-id="f3b65-503">So deaktivieren Sie die Anzeige des Prozesses Sicherheit unter Sicherheit Gerät Problembehandlung verwendet.</span><span class="sxs-lookup"><span data-stu-id="f3b65-503">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="f3b65-504">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f3b65-504">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="f3b65-505">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-505">String</span></span>|<span data-ttu-id="f3b65-506">Der Firmenname, der den Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-506">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="f3b65-507">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="f3b65-507">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="f3b65-508">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-508">String</span></span>|<span data-ttu-id="f3b65-509">Die e-Mail-Adresse, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-509">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="f3b65-510">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="f3b65-510">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="f3b65-511">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-511">String</span></span>|<span data-ttu-id="f3b65-512">Die angegebene Rufnummer oder Skype-ID, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-512">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="f3b65-513">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="f3b65-513">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="f3b65-514">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-514">String</span></span>|<span data-ttu-id="f3b65-515">Das Hilfeportal URL dies für Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f3b65-515">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="f3b65-516">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="f3b65-516">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="f3b65-517">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="f3b65-517">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="f3b65-518">Benachrichtigungen über die angezeigte Bereiche der app angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-518">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="f3b65-519">Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-519">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="f3b65-520">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="f3b65-520">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="f3b65-521">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="f3b65-521">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="f3b65-522">Konfigurieren Sie, wie IT-Kontakt anzeigen Informationen für Endbenutzer.</span><span class="sxs-lookup"><span data-stu-id="f3b65-522">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="f3b65-523">Mögliche Werte: sind `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-523">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="f3b65-524">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="f3b65-524">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="f3b65-525">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-525">Boolean</span></span>|<span data-ttu-id="f3b65-526">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="f3b65-526">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="f3b65-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="f3b65-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="f3b65-528">Int32</span><span class="sxs-lookup"><span data-stu-id="f3b65-528">Int32</span></span>|<span data-ttu-id="f3b65-529">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="f3b65-529">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="f3b65-530">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-530">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="f3b65-531">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="f3b65-531">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="f3b65-532">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="f3b65-532">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="f3b65-533">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="f3b65-533">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="f3b65-534">Wählen Sie den vorinstallierten Schlüssel um zu verwendende Codierung.</span><span class="sxs-lookup"><span data-stu-id="f3b65-534">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="f3b65-535">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-535">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="f3b65-536">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="f3b65-536">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="f3b65-537">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-537">Boolean</span></span>|<span data-ttu-id="f3b65-538">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f3b65-538">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f3b65-539">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="f3b65-539">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="f3b65-540">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-540">Boolean</span></span>|<span data-ttu-id="f3b65-541">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-541">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="f3b65-542">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="f3b65-542">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="f3b65-543">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-543">Boolean</span></span>|<span data-ttu-id="f3b65-544">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f3b65-544">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f3b65-545">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="f3b65-545">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="f3b65-546">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-546">Boolean</span></span>|<span data-ttu-id="f3b65-547">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-547">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="f3b65-548">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f3b65-548">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="f3b65-549">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f3b65-549">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="f3b65-550">Geben Sie an, wie die Certificate Revocation List erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-550">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="f3b65-551">Mögliche Werte: sind `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-551">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="f3b65-552">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="f3b65-552">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="f3b65-553">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-553">Boolean</span></span>|<span data-ttu-id="f3b65-554">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="f3b65-554">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="f3b65-555">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="f3b65-555">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="f3b65-556">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="f3b65-556">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="f3b65-557">Konfiguriert, wie vom Warteschlangensystem Paket im Szenario mit Tunnel Gateway angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f3b65-557">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="f3b65-558">Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-558">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="f3b65-559">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="f3b65-559">firewallProfileDomain</span></span>|[<span data-ttu-id="f3b65-560">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f3b65-560">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f3b65-561">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="f3b65-561">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="f3b65-562">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="f3b65-562">firewallProfilePublic</span></span>|[<span data-ttu-id="f3b65-563">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f3b65-563">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f3b65-564">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="f3b65-564">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="f3b65-565">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="f3b65-565">firewallProfilePrivate</span></span>|[<span data-ttu-id="f3b65-566">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f3b65-566">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f3b65-567">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="f3b65-567">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="f3b65-568">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="f3b65-568">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="f3b65-569">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3b65-569">String collection</span></span>|<span data-ttu-id="f3b65-570">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-570">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="f3b65-571">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-571">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="f3b65-572">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-572">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-573">Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-573">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="f3b65-574">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-574">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-575">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="f3b65-575">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="f3b65-576">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-576">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-577">Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-577">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="f3b65-578">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-578">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="f3b65-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="f3b65-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-581">Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte.</span><span class="sxs-lookup"><span data-stu-id="f3b65-581">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f3b65-582">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="f3b65-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="f3b65-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-585">Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte.</span><span class="sxs-lookup"><span data-stu-id="f3b65-585">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f3b65-586">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-587">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="f3b65-587">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="f3b65-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-589">Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten.</span><span class="sxs-lookup"><span data-stu-id="f3b65-589">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f3b65-590">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-591">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f3b65-591">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="f3b65-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-593">Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten.</span><span class="sxs-lookup"><span data-stu-id="f3b65-593">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f3b65-594">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-595">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="f3b65-595">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="f3b65-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-597">Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert.</span><span class="sxs-lookup"><span data-stu-id="f3b65-597">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f3b65-598">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-599">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="f3b65-599">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="f3b65-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-601">Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert.</span><span class="sxs-lookup"><span data-stu-id="f3b65-601">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f3b65-602">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-603">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="f3b65-603">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="f3b65-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-605">Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code.</span><span class="sxs-lookup"><span data-stu-id="f3b65-605">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f3b65-606">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-607">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="f3b65-607">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="f3b65-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-609">Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code.</span><span class="sxs-lookup"><span data-stu-id="f3b65-609">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f3b65-610">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-611">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-611">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="f3b65-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-613">Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-613">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f3b65-614">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-615">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="f3b65-615">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="f3b65-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-617">Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="f3b65-617">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f3b65-618">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-619">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="f3b65-619">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="f3b65-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-621">Der Wert, der angibt, wenn die Anmeldeinformationen, die vom Windows lokalen Behörde Teilsystem stehlen zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-621">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="f3b65-622">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-623">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="f3b65-623">defenderProcessCreationType</span></span>|[<span data-ttu-id="f3b65-624">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-624">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-625">Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-625">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f3b65-626">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-626">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-627">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="f3b65-627">defenderProcessCreation</span></span>|[<span data-ttu-id="f3b65-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-629">Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-629">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f3b65-630">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-631">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="f3b65-631">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="f3b65-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-633">Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-633">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f3b65-634">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-635">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="f3b65-635">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="f3b65-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-637">Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="f3b65-637">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f3b65-638">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-639">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="f3b65-639">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="f3b65-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-641">Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien.</span><span class="sxs-lookup"><span data-stu-id="f3b65-641">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f3b65-642">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-643">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="f3b65-643">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="f3b65-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-645">Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien.</span><span class="sxs-lookup"><span data-stu-id="f3b65-645">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f3b65-646">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-647">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-647">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="f3b65-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3b65-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3b65-649">Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="f3b65-649">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f3b65-650">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-651">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="f3b65-651">defenderEmailContentExecution</span></span>|[<span data-ttu-id="f3b65-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-653">Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="f3b65-653">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f3b65-654">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-655">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-655">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="f3b65-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-657">Wert, der Verwendung der erweiterte Schutz vor Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="f3b65-657">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="f3b65-658">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-659">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="f3b65-659">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="f3b65-660">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-660">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="f3b65-661">Wert, der das Verhalten der geschützte Ordner.</span><span class="sxs-lookup"><span data-stu-id="f3b65-661">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="f3b65-662">Mögliche Werte sind: `userDefined`, `enable`, `auditMode`, `blockDiskModification` und `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-662">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="f3b65-663">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="f3b65-663">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="f3b65-664">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3b65-664">String collection</span></span>|<span data-ttu-id="f3b65-665">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-665">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="f3b65-666">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="f3b65-666">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="f3b65-667">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f3b65-667">String collection</span></span>|<span data-ttu-id="f3b65-668">Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-668">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="f3b65-669">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-669">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="f3b65-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3b65-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3b65-671">Wert, der das Verhalten des NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="f3b65-671">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="f3b65-672">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3b65-673">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="f3b65-673">defenderExploitProtectionXml</span></span>|<span data-ttu-id="f3b65-674">Binär</span><span class="sxs-lookup"><span data-stu-id="f3b65-674">Binary</span></span>|<span data-ttu-id="f3b65-675">XML-Inhalte mit Details zum Exploit-Schutz.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-675">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="f3b65-676">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="f3b65-676">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="f3b65-677">String</span><span class="sxs-lookup"><span data-stu-id="f3b65-677">String</span></span>|<span data-ttu-id="f3b65-678">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-678">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="f3b65-679">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="f3b65-679">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="f3b65-680">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-680">Boolean</span></span>|<span data-ttu-id="f3b65-681">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="f3b65-681">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="f3b65-682">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="f3b65-682">appLockerApplicationControl</span></span>|[<span data-ttu-id="f3b65-683">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f3b65-683">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="f3b65-684">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="f3b65-684">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="f3b65-685">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-685">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="f3b65-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="f3b65-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="f3b65-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="f3b65-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="f3b65-688">Anmeldeinformationen Guard aktivieren Sie, wenn Sicherheit Plattformebene mit Secure Boot und Virtualisierung Sicherheit sind beide aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f3b65-688">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="f3b65-689">Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-689">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="f3b65-690">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="f3b65-690">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="f3b65-691">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-691">Boolean</span></span>|<span data-ttu-id="f3b65-692">Schaltet die Virtualisierung basierend Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="f3b65-692">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="f3b65-693">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="f3b65-693">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="f3b65-694">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-694">Boolean</span></span>|<span data-ttu-id="f3b65-695">Gibt an, ob Sicherheit Plattformebene beim nächsten Neustart aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f3b65-695">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="f3b65-696">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="f3b65-696">smartScreenEnableInShell</span></span>|<span data-ttu-id="f3b65-697">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-697">Boolean</span></span>|<span data-ttu-id="f3b65-698">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="f3b65-698">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="f3b65-699">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="f3b65-699">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="f3b65-700">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-700">Boolean</span></span>|<span data-ttu-id="f3b65-701">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-701">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="f3b65-702">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="f3b65-702">applicationGuardEnabled</span></span>|<span data-ttu-id="f3b65-703">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-703">Boolean</span></span>|<span data-ttu-id="f3b65-704">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="f3b65-704">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="f3b65-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f3b65-705">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="f3b65-706">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f3b65-706">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="f3b65-707">Aktivieren Sie Windows Defender Anwendung Guard für neuere Versionen von Windows.</span><span class="sxs-lookup"><span data-stu-id="f3b65-707">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="f3b65-708">Mögliche Werte: sind `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-708">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="f3b65-709">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f3b65-709">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="f3b65-710">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="f3b65-710">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="f3b65-711">Block Zwischenablage Übertragung Bilddatei, Textdatei oder dürfen.</span><span class="sxs-lookup"><span data-stu-id="f3b65-711">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="f3b65-712">Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-712">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="f3b65-713">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="f3b65-713">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="f3b65-714">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-714">Boolean</span></span>|<span data-ttu-id="f3b65-715">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="f3b65-715">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="f3b65-716">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="f3b65-716">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="f3b65-717">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-717">Boolean</span></span>|<span data-ttu-id="f3b65-718">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="f3b65-718">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="f3b65-719">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="f3b65-719">applicationGuardForceAuditing</span></span>|<span data-ttu-id="f3b65-720">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-720">Boolean</span></span>|<span data-ttu-id="f3b65-721">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="f3b65-721">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="f3b65-722">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="f3b65-722">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="f3b65-723">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f3b65-723">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="f3b65-724">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="f3b65-724">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="f3b65-725">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="f3b65-725">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="f3b65-726">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="f3b65-726">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="f3b65-727">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-727">Boolean</span></span>|<span data-ttu-id="f3b65-728">Erlaubt das Drucken im PDF-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-728">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="f3b65-729">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="f3b65-729">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="f3b65-730">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-730">Boolean</span></span>|<span data-ttu-id="f3b65-731">Erlaubt das Drucken im XPS-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-731">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="f3b65-732">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="f3b65-732">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="f3b65-733">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-733">Boolean</span></span>|<span data-ttu-id="f3b65-734">Erlaubt das Drucken auf lokalen Druckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-734">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="f3b65-735">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="f3b65-735">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="f3b65-736">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-736">Boolean</span></span>|<span data-ttu-id="f3b65-737">Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-737">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="f3b65-738">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="f3b65-738">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="f3b65-739">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-739">Boolean</span></span>|<span data-ttu-id="f3b65-740">Zulassen der Anwendung Guard virtuellen GPU verwenden</span><span class="sxs-lookup"><span data-stu-id="f3b65-740">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="f3b65-741">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="f3b65-741">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="f3b65-742">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f3b65-742">Boolean</span></span>|<span data-ttu-id="f3b65-743">Zulassen, dass Benutzer Dateien vom Rand im Container Guard Anwendung herunterladen und speichern Sie sie auf dem Host Dateisystem</span><span class="sxs-lookup"><span data-stu-id="f3b65-743">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="f3b65-744">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="f3b65-744">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="f3b65-745">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-745">Boolean</span></span>|<span data-ttu-id="f3b65-746">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f3b65-746">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="f3b65-747">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="f3b65-747">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="f3b65-748">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-748">Boolean</span></span>|<span data-ttu-id="f3b65-749">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-749">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="f3b65-750">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="f3b65-750">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="f3b65-751">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="f3b65-751">bitLockerEncryptDevice</span></span>|<span data-ttu-id="f3b65-752">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f3b65-752">Boolean</span></span>|<span data-ttu-id="f3b65-753">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="f3b65-753">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="f3b65-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3b65-754">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="f3b65-755">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3b65-755">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="f3b65-756">System BitLocker Drive-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="f3b65-756">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="f3b65-757">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3b65-757">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="f3b65-758">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3b65-758">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="f3b65-759">BitLocker feste Laufwerk Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="f3b65-759">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="f3b65-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3b65-760">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="f3b65-761">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3b65-761">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="f3b65-762">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="f3b65-762">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f3b65-763">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3b65-763">Response</span></span>
<span data-ttu-id="f3b65-764">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f3b65-764">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3b65-765">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3b65-765">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3b65-766">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3b65-766">Request</span></span>
<span data-ttu-id="f3b65-767">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3b65-767">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26391

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f3b65-768">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3b65-768">Response</span></span>
<span data-ttu-id="f3b65-p194">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3b65-p194">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26499

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```




