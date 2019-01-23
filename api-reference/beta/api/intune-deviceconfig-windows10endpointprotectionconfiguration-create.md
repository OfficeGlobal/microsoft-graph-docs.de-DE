---
title: Erstellen von „windows10EndpointProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10EndpointProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bdc31fed7797a448239bc7ed19ac57750692646
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402587"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="1fa44-103">Erstellen von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="1fa44-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="1fa44-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1fa44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1fa44-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fa44-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1fa44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fa44-107">Diese Methode erstellt ein neues Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fa44-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1fa44-108">Prerequisites</span></span>
<span data-ttu-id="1fa44-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1fa44-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1fa44-111">Permission type</span></span>|<span data-ttu-id="1fa44-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1fa44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fa44-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1fa44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fa44-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa44-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fa44-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1fa44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fa44-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fa44-116">Not supported.</span></span>|
|<span data-ttu-id="1fa44-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1fa44-117">Application</span></span>|<span data-ttu-id="1fa44-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fa44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fa44-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fa44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1fa44-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1fa44-120">Request headers</span></span>
|<span data-ttu-id="1fa44-121">Header</span><span class="sxs-lookup"><span data-stu-id="1fa44-121">Header</span></span>|<span data-ttu-id="1fa44-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1fa44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fa44-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1fa44-123">Authorization</span></span>|<span data-ttu-id="1fa44-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1fa44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fa44-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1fa44-125">Accept</span></span>|<span data-ttu-id="1fa44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fa44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fa44-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1fa44-127">Request body</span></span>
<span data-ttu-id="1fa44-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EndpointProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="1fa44-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="1fa44-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EndpointProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="1fa44-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1fa44-130">Property</span></span>|<span data-ttu-id="1fa44-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1fa44-131">Type</span></span>|<span data-ttu-id="1fa44-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fa44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa44-133">id</span><span class="sxs-lookup"><span data-stu-id="1fa44-133">id</span></span>|<span data-ttu-id="1fa44-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-134">String</span></span>|<span data-ttu-id="1fa44-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1fa44-135">Key of the entity.</span></span> <span data-ttu-id="1fa44-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa44-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1fa44-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa44-138">DateTimeOffset</span></span>|<span data-ttu-id="1fa44-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1fa44-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1fa44-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1fa44-141">roleScopeTagIds</span></span>|<span data-ttu-id="1fa44-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1fa44-142">String collection</span></span>|<span data-ttu-id="1fa44-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="1fa44-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1fa44-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1fa44-145">supportsScopeTags</span></span>|<span data-ttu-id="1fa44-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-146">Boolean</span></span>|<span data-ttu-id="1fa44-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1fa44-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1fa44-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1fa44-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-150">This property is read-only.</span></span> <span data-ttu-id="1fa44-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa44-152">createdDateTime</span></span>|<span data-ttu-id="1fa44-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa44-153">DateTimeOffset</span></span>|<span data-ttu-id="1fa44-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1fa44-154">DateTime the object was created.</span></span> <span data-ttu-id="1fa44-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-156">description</span><span class="sxs-lookup"><span data-stu-id="1fa44-156">description</span></span>|<span data-ttu-id="1fa44-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-157">String</span></span>|<span data-ttu-id="1fa44-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1fa44-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1fa44-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1fa44-160">displayName</span></span>|<span data-ttu-id="1fa44-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-161">String</span></span>|<span data-ttu-id="1fa44-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1fa44-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1fa44-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-164">Version</span><span class="sxs-lookup"><span data-stu-id="1fa44-164">version</span></span>|<span data-ttu-id="1fa44-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1fa44-165">Int32</span></span>|<span data-ttu-id="1fa44-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1fa44-166">Version of the device configuration.</span></span> <span data-ttu-id="1fa44-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fa44-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fa44-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="1fa44-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="1fa44-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="1fa44-170">Diese Richtlinie soll gegen externe DMA Geräten zusätzliche Sicherheit zu bieten.</span><span class="sxs-lookup"><span data-stu-id="1fa44-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="1fa44-171">Es ermöglicht den für größere Kontrolle über die Enumeration von externen DMA-Geräten mit Sandkästen und DMA Remapping/Gerät Arbeitsspeicher Isolation nicht kompatibel.</span><span class="sxs-lookup"><span data-stu-id="1fa44-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="1fa44-172">Diese Richtlinie wird nur wirksam, wenn Kernel DMA Protection unterstützt und von der Systemfirmware aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="1fa44-173">Kernel DMA Schutz ist ein Plattform-Feature, das über Gruppenrichtlinie oder durch Endbenutzer gesteuert werden kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="1fa44-174">Dies ist nur zum Zeitpunkt der Produktion vom System unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="1fa44-175">Um zu überprüfen, ob das System Kernel DMA Protection unterstützt, überprüfen Sie das Kernel DMA Protection-Feld in der Seite Zusammenfassung des MSINFO32.exe ein.</span><span class="sxs-lookup"><span data-stu-id="1fa44-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="1fa44-176">Mögliche Werte sind: `deviceDefault`, `blockAll` und `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="1fa44-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="1fa44-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="1fa44-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-179">Diese Berechtigung wird während der Sicherung/Wiederherstellung von Anmeldeinformations-Manager verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="1fa44-180">Gespeicherten Anmeldeinformationen der Benutzer können beeinträchtigt werden, wenn diese Berechtigung für die anderen Entitäten angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="1fa44-181">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="1fa44-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="1fa44-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-184">Diese Berechtigung bestimmt, welche Benutzer und Gruppen mit dem Computer über das Netzwerk herstellen dürfen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="1fa44-185">State zugelassen wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="1fa44-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="1fa44-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="1fa44-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-188">Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Block aus eine Verbindung mit dem Computer über das Netzwerk sind.</span><span class="sxs-lookup"><span data-stu-id="1fa44-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="1fa44-189">State-Block wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-189">State Block is supported.</span></span>|
|<span data-ttu-id="1fa44-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1fa44-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="1fa44-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-192">Diese Berechtigung ermöglicht es einem Prozess zum Identitätswechsel für alle Benutzer ohne Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="1fa44-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="1fa44-193">Der Prozess kann daher auf dieselben lokalen Ressourcen wie der Benutzer zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="1fa44-194">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="1fa44-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="1fa44-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-197">Dieser Benutzer Rechte bestimmt, welche Benutzer am Computer anmelden können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="1fa44-198">Status nicht konfiguriert, zugelassen und blockiert werden alle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="1fa44-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="1fa44-199">userRightsBackupData</span></span>|[<span data-ttu-id="1fa44-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-201">Diese Rechte Benutzer bestimmt, welche Benutzer Datei-, Verzeichnis-, Registrierung und andere beständige Objekte Berechtigungen beim Sichern der Dateien und Verzeichnisse umgehen können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="1fa44-202">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="1fa44-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="1fa44-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-205">Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Uhrzeit und Datum der internen Uhr des Computers ändern können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="1fa44-206">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="1fa44-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="1fa44-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-209">Diese Einstellung bestimmt, ob Benutzer globale Objekte erstellen können, die alle Sitzungen zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="1fa44-210">Benutzer, die globale Objekte erstellen können, können es sich um Prozesse auswirken, die unter anderer Benutzer Sitzungen, ausgeführt wird und zu Anwendung Fehler und Datenverlust führen kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="1fa44-211">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="1fa44-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="1fa44-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-214">Diese Berechtigung bestimmt, welche Benutzer und Gruppen können eine interne API zum Erstellen und Ändern der Größe der Auslagerungsdatei aufrufen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="1fa44-215">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="1fa44-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="1fa44-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-218">Diese Rechte Benutzer bestimmt, welche Konten von Prozessen verwendet werden können, um ein Verzeichnisobjekt mithilfe des Objekts-Manager erstellen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="1fa44-219">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="1fa44-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="1fa44-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-222">Dieser Benutzer Rechte bestimmt, ob der Benutzer eine symbolische Verbindung vom Computer erstellen kann, an dem sie angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="1fa44-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="1fa44-223">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="1fa44-224">userRightsCreateToken</span></span>|[<span data-ttu-id="1fa44-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-226">Diese Berechtigung bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token erstellen, die Zugriff auf alle lokalen Ressourcen abrufen, wenn der Prozess eine interne API verwendet, um ein Zugriffstoken erstellen verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="1fa44-227">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="1fa44-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="1fa44-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-230">Diese Rechte Benutzer bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="1fa44-231">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1fa44-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="1fa44-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="1fa44-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-234">Diese Berechtigung bestimmt, welche Benutzer und Gruppen nicht zulässig sind, als Remote Desktop Services Client anmelden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="1fa44-235">Nur die Bundesländer nicht konfiguriert und blockiert werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="1fa44-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="1fa44-236">userRightsDelegation</span></span>|[<span data-ttu-id="1fa44-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-238">Dieser Benutzer Rechte bestimmt, welche Benutzer die vertrauenswürdige für Delegierung Einstellung für ein Benutzer- oder Computerkonto-Objekt festlegen können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="1fa44-239">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="1fa44-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="1fa44-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-242">Dieser Benutzer Rechte bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen im Sicherheitsprotokoll verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="1fa44-243">Sicherheitsprotokoll wird verwendet, um autorisierter Zugriff zu verfolgen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="1fa44-244">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="1fa44-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="1fa44-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-247">Zuweisen von diesem Benutzerrecht keinem Benutzer kann für diesen Benutzer zum Annehmen der Clientidentität ausgeführte Programme.</span><span class="sxs-lookup"><span data-stu-id="1fa44-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="1fa44-248">Voraussetzen dieses Benutzerrecht für diese Art des Identitätswechsels verhindert, dass einen nicht autorisierten Benutzer aus überzeugende einen Client eine Verbindung zu einem Dienst, die sie erstellt haben, und klicken Sie dann Identitätswechsel bei dieser Client, dem der nicht autorisierte Benutzer Berechtigungen zu erhöhen können Administrative oder Systemebenen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="1fa44-249">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="1fa44-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="1fa44-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-252">Diese Rechte Benutzer bestimmt, welche Konten einen Prozess mit Schreibzugriff auf einen anderen Prozess verwenden können, um die Ausführungspriorität zugewiesen an den anderen Prozess zu erhöhen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="1fa44-253">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="1fa44-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="1fa44-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-256">Dieser Benutzer Rechte bestimmt, welche Benutzer können dynamisch laden und entladen Gerätetreiber oder anderen Code im Kernelmodus.</span><span class="sxs-lookup"><span data-stu-id="1fa44-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="1fa44-257">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="1fa44-258">userRightsLockMemory</span></span>|[<span data-ttu-id="1fa44-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-260">Dieser Benutzer Rechte bestimmt, welche Konten einen Prozess Speichern von Daten im physikalischen Speicher, wodurch das System verhindert, dass die Daten in den virtuellen Speicher auf dem Datenträger paging verwenden können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="1fa44-261">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="1fa44-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="1fa44-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-264">Diese Berechtigung bestimmt, welche Benutzer Objekt den Optionen für einzelne Ressourcen, wie Dateien, Active Directory-Objekte und Registrierungsschlüssel für die Überwachung angeben können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="1fa44-265">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="1fa44-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="1fa44-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-268">Diese Rechte Benutzer bestimmt der Benutzer und Gruppen auf einem Datenträger, wie remote Defragmentierung Wartungsaufgaben ausführen können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="1fa44-269">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="1fa44-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="1fa44-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-272">Diese Berechtigung bestimmt, Firmware-Umgebungsvariablen geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="1fa44-273">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="1fa44-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="1fa44-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-276">Dieser Benutzer Rechte bestimmt, welche Benutzerkonten die Bezeichnung Integrität von Objekten, wie Dateien, Registrierungsschlüssel oder Prozesse, die im Besitz von anderen Benutzern ändern können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="1fa44-277">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="1fa44-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="1fa44-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-280">Dieser Benutzer Rechte bestimmt, welche Benutzer Tools zum Überwachen der Leistung verwenden können, zur Überwachung der Leistung der Systemprozesse.</span><span class="sxs-lookup"><span data-stu-id="1fa44-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="1fa44-281">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="1fa44-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="1fa44-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-284">Dieser Benutzer Rechte bestimmt, welche Benutzer dürfen Herunterfahren eines Computers von einem Remotestandort im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="1fa44-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="1fa44-285">Missbrauch dieses Benutzerrechts kann ein Denial-of-Service führen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="1fa44-286">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="1fa44-287">userRightsRestoreData</span></span>|[<span data-ttu-id="1fa44-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-289">Diese Berechtigung bestimmt, welche Benutzer umgehen können Datei-, Verzeichnis-, Registrierung und andere beständige Objekte, die Berechtigungen, die beim Wiederherstellen von Dateien und Verzeichnisse gesichert und bestimmt, welche Benutzer einen beliebigen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="1fa44-290">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="1fa44-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="1fa44-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-293">Dieser Benutzer Rechte bestimmt, welche Benutzer die Besitzrechte für ein beliebiges sicherungsfähiges Objekt in das System, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads übernehmen können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="1fa44-294">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1fa44-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="1fa44-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="1fa44-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1fa44-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1fa44-297">Diese Einstellung legt fest, welche Dienstkonten für das Registrieren von eines Prozess als Dienst gehindert werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="1fa44-298">Hinweis: Diese Einstellung gilt nicht für die Konten System, lokaler Dienst oder Netzwerkdienst.</span><span class="sxs-lookup"><span data-stu-id="1fa44-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="1fa44-299">Nur Status blockiert wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="1fa44-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="1fa44-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="1fa44-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-301">Boolean</span></span>|<span data-ttu-id="1fa44-302">Diese Einstellung bestimmt, ob Xbox Spiel speichern aktiviert (1) oder deaktiviert (0) ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="1fa44-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1fa44-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="1fa44-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1fa44-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1fa44-305">Diese Einstellung bestimmt, ob der Verwaltungsdienst Zubehör Starttyp Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1fa44-306">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="1fa44-306">Default: Manual.</span></span> <span data-ttu-id="1fa44-307">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1fa44-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1fa44-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="1fa44-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1fa44-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1fa44-310">Diese Einstellung bestimmt, ob Starttyp Live Auth-Manager-Dienst Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1fa44-311">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="1fa44-311">Default: Manual.</span></span> <span data-ttu-id="1fa44-312">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1fa44-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1fa44-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="1fa44-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1fa44-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1fa44-315">Diese Einstellung bestimmt, ob Live Spiel Speichern des Dienstes Starttyp Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1fa44-316">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="1fa44-316">Default: Manual.</span></span> <span data-ttu-id="1fa44-317">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1fa44-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1fa44-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="1fa44-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1fa44-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1fa44-320">Diese Einstellung bestimmt, ob Starttyp Networking-Dienst Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1fa44-321">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="1fa44-321">Default: Manual.</span></span> <span data-ttu-id="1fa44-322">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1fa44-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="1fa44-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="1fa44-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-324">Boolean</span></span>|<span data-ttu-id="1fa44-325">Hindert Benutzer am Hinzufügen von neuen Microsoft-Konten auf diesem Computer.</span><span class="sxs-lookup"><span data-stu-id="1fa44-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="1fa44-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="1fa44-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="1fa44-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-327">Boolean</span></span>|<span data-ttu-id="1fa44-328">Aktivieren Sie lokale Konten, die nicht von anderen Orten als physisches Gerät anmelden, um kennwortgeschützte sind. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="1fa44-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="1fa44-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="1fa44-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="1fa44-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-330">Boolean</span></span>|<span data-ttu-id="1fa44-331">Bestimmt, ob das lokale Administratorkonto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="1fa44-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="1fa44-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="1fa44-333">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-333">String</span></span>|<span data-ttu-id="1fa44-334">Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1fa44-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="1fa44-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="1fa44-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="1fa44-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-336">Boolean</span></span>|<span data-ttu-id="1fa44-337">Bestimmt, ob das Konto Gast aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="1fa44-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="1fa44-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="1fa44-339">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-339">String</span></span>|<span data-ttu-id="1fa44-340">Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Gast" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1fa44-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="1fa44-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="1fa44-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="1fa44-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-342">Boolean</span></span>|<span data-ttu-id="1fa44-343">Verhindern Sie, dass eines portablen Computers ohne Anmeldung abgedockt werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="1fa44-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="1fa44-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="1fa44-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-345">Boolean</span></span>|<span data-ttu-id="1fa44-346">Installieren von Druckertreiber als Teil des Herstellens einer Verbindung zu einem freigegebenen Drucker Admins nur zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="1fa44-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="1fa44-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="1fa44-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="1fa44-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-348">Boolean</span></span>|<span data-ttu-id="1fa44-349">Aktivieren diese Einstellungen kann nur interaktiv angemeldeten Benutzer auf CD-ROM-Medien zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="1fa44-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="1fa44-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="1fa44-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="1fa44-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="1fa44-352">Definieren Sie, wer berechtigt ist, zu formatieren und NTFS-Wechselmedium ausschließen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="1fa44-353">Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="1fa44-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="1fa44-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="1fa44-355">Int32</span><span class="sxs-lookup"><span data-stu-id="1fa44-355">Int32</span></span>|<span data-ttu-id="1fa44-356">Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="1fa44-357">Gültige Werte von 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="1fa44-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="1fa44-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="1fa44-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="1fa44-359">Int32</span><span class="sxs-lookup"><span data-stu-id="1fa44-359">Int32</span></span>|<span data-ttu-id="1fa44-360">Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="1fa44-361">Gültige Werte von 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="1fa44-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="1fa44-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="1fa44-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="1fa44-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-363">Boolean</span></span>|<span data-ttu-id="1fa44-364">Benötigen Sie STRG + ALT + ENTF gedrückt werden, bevor ein Benutzer anmelden kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="1fa44-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="1fa44-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="1fa44-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-366">Boolean</span></span>|<span data-ttu-id="1fa44-367">Der Benutzername der letzten Person ein, die Anmeldung auf dem Gerät nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="1fa44-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="1fa44-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="1fa44-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-369">Boolean</span></span>|<span data-ttu-id="1fa44-370">Der Benutzername der Person, die dieses Gerät anmelden, nachdem Anmeldeinformationen eingegeben wurden und bevor der Desktop des Geräts angezeigt wird nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="1fa44-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="1fa44-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="1fa44-372">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-372">String</span></span>|<span data-ttu-id="1fa44-373">Festlegen Sie Titel der Nachricht für Benutzer, die versuchen, melden Sie sich bei.</span><span class="sxs-lookup"><span data-stu-id="1fa44-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="1fa44-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="1fa44-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="1fa44-375">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-375">String</span></span>|<span data-ttu-id="1fa44-376">Festlegen des Nachrichtentexts für Benutzer, die sich anmelden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="1fa44-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="1fa44-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="1fa44-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-378">Boolean</span></span>|<span data-ttu-id="1fa44-379">Block PKU2U authentifizierungsanforderungen an dieses Gerät online-Identitäten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="1fa44-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="1fa44-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="1fa44-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-381">Boolean</span></span>|<span data-ttu-id="1fa44-382">UI-Hilfsprogramm für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager Entität boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="1fa44-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="1fa44-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="1fa44-384">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-384">String</span></span>|<span data-ttu-id="1fa44-385">Bearbeiten Sie die Security Descriptor Definition Language Standardzeichenfolge zum gewähren oder verweigern, Benutzer und Gruppen, um die SAM remote anzurufen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="1fa44-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="1fa44-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="1fa44-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1fa44-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="1fa44-388">Diese Einstellung kann ein Client die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="1fa44-389">Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="1fa44-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="1fa44-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="1fa44-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1fa44-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="1fa44-392">Diese Einstellung kann ein Server die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="1fa44-393">Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="1fa44-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1fa44-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="1fa44-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1fa44-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="1fa44-396">Diese Einstellung bestimmt, welche Herausforderung/Antwort-Authentifizierungsprotokoll Netzwerk Anmeldungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="1fa44-397">Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="1fa44-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="1fa44-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="1fa44-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-399">Boolean</span></span>|<span data-ttu-id="1fa44-400">Wenn aktiviert, wird der SMB-Client unsichere Gast Anmeldungen zulassen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="1fa44-401">Falls nicht konfiguriert, wird der SMB-Client unsichere Gast Anmeldungen abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="1fa44-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="1fa44-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="1fa44-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-403">Boolean</span></span>|<span data-ttu-id="1fa44-404">Diese Einstellung bestimmt, ob die Auslagerungsdatei beim Herunterfahren des Systems gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="1fa44-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="1fa44-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="1fa44-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-406">Boolean</span></span>|<span data-ttu-id="1fa44-407">Diese Einstellung bestimmt, ob es sich bei ein Computer beendet werden kann, ohne bei Windows anmelden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="1fa44-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="1fa44-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="1fa44-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-409">Boolean</span></span>|<span data-ttu-id="1fa44-410">Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop.</span><span class="sxs-lookup"><span data-stu-id="1fa44-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="1fa44-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="1fa44-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="1fa44-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-412">Boolean</span></span>|<span data-ttu-id="1fa44-413">Virtualisieren von Datei- und -Schreibvorgänge mit Fehlern an pro Benutzer Speicherorte</span><span class="sxs-lookup"><span data-stu-id="1fa44-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="1fa44-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="1fa44-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="1fa44-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-415">Boolean</span></span>|<span data-ttu-id="1fa44-416">Erzwingen Sie PKI-Zertifizierung Pfad Überprüfung für eine bestimmte ausführbare Datei, bevor er ausführen kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="1fa44-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1fa44-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="1fa44-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1fa44-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="1fa44-419">Definieren Sie das Verhalten der Aufforderung für Administratoren im Administratormodus Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="1fa44-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="1fa44-420">Mögliche Werte sind: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent` und `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="1fa44-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1fa44-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="1fa44-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1fa44-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="1fa44-423">Definieren Sie das Verhalten der Elevation Ansage für Standardbenutzer.</span><span class="sxs-lookup"><span data-stu-id="1fa44-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="1fa44-424">Mögliche Werte: sind `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="1fa44-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="1fa44-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="1fa44-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-426">Boolean</span></span>|<span data-ttu-id="1fa44-427">Aktivieren Sie alle Elevation-Anforderungen, fahren Sie mit dem sicheren Desktop, sondern den interaktiven Desktop des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="1fa44-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="1fa44-428">Richtlinien für Administratoren und Standardbenutzer Prompt Verhalten dienen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="1fa44-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="1fa44-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="1fa44-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-430">Boolean</span></span>|<span data-ttu-id="1fa44-431">App Installationen mit erhöhte Berechtigungen werden für die Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="1fa44-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="1fa44-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="1fa44-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="1fa44-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-433">Boolean</span></span>|<span data-ttu-id="1fa44-434">Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="1fa44-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="1fa44-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="1fa44-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="1fa44-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-436">Boolean</span></span>|<span data-ttu-id="1fa44-437">Definiert, ob das integrierte Administratorkonto Administratormodus Genehmigung verwendet oder alle apps mit vollständigen Administratorberechtigungen ausgeführt wird. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="1fa44-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="1fa44-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="1fa44-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="1fa44-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-439">Boolean</span></span>|<span data-ttu-id="1fa44-440">Definieren Sie, ob Administratormodus Genehmigung und alle UAC-Richtlinieneinstellungen aktiviert sind, ist standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1fa44-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="1fa44-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1fa44-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="1fa44-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="1fa44-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="1fa44-443">Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="1fa44-444">Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="1fa44-445">Mögliche Werte: sind `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="1fa44-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1fa44-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="1fa44-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="1fa44-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="1fa44-448">Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="1fa44-449">Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="1fa44-450">Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="1fa44-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="1fa44-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="1fa44-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-452">Boolean</span></span>|<span data-ttu-id="1fa44-453">Diese Einstellung bestimmt, ob der SMB-Client versucht, SMB-Paketsignatur aushandeln.</span><span class="sxs-lookup"><span data-stu-id="1fa44-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="1fa44-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="1fa44-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="1fa44-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-455">Boolean</span></span>|<span data-ttu-id="1fa44-456">Diese Einstellung bestimmt, ob die Clientkomponente für SMB-Paketsignatur erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="1fa44-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="1fa44-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="1fa44-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-458">Boolean</span></span>|<span data-ttu-id="1fa44-459">Wenn diese Einstellung aktiviert ist, kann der Server Message Block (SMB) Redirector nur-Text-Kennwörter an nicht - Microsoft SMB-Server zu senden, die keine für die Verschlüsselung von Kennwörtern während der Authentifizierung Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="1fa44-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="1fa44-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="1fa44-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="1fa44-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-461">Boolean</span></span>|<span data-ttu-id="1fa44-462">Diese Einstellung bestimmt, ob die SMB-Server-Komponente Paketsignatur erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="1fa44-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="1fa44-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="1fa44-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-464">Boolean</span></span>|<span data-ttu-id="1fa44-465">Diese Einstellung bestimmt, ob der SMB Server SMB-Paketsignatur mit Clients, die diese anfordern aushandeln kann.</span><span class="sxs-lookup"><span data-stu-id="1fa44-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="1fa44-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="1fa44-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="1fa44-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-467">Boolean</span></span>|<span data-ttu-id="1fa44-468">Diese Einstellung schränkt standardmäßig anonymen Zugriff auf Freigaben und Pipes an den Einstellungen für named Pipes, die anonym zugegriffen werden können und Freigaben, die anonym zugegriffen werden kann</span><span class="sxs-lookup"><span data-stu-id="1fa44-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="1fa44-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="1fa44-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="1fa44-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-470">Boolean</span></span>|<span data-ttu-id="1fa44-471">Diese Einstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="1fa44-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="1fa44-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="1fa44-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-473">Boolean</span></span>|<span data-ttu-id="1fa44-474">Diese Einstellung bestimmt, ob anonyme Benutzer zum Ausführen bestimmter Aktivitäten, beispielsweise die Namen von Domänenkonten und Netzwerkfreigaben auflisten können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="1fa44-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="1fa44-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="1fa44-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-476">Boolean</span></span>|<span data-ttu-id="1fa44-477">Diese Einstellung bestimmt, ob, an die nächste Änderung des Kennworts, der Hashwert LAN Manager (LM) für das neue Kennwort gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="1fa44-478">Es wird nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="1fa44-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="1fa44-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="1fa44-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="1fa44-480">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1fa44-480">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="1fa44-481">Diese Einstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Leser entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="1fa44-482">Mögliche Werte: sind `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="1fa44-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="1fa44-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-484">Boolean</span></span>|<span data-ttu-id="1fa44-485">So deaktivieren Sie die Anzeige des Bereichs Protection app und Browser verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="1fa44-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="1fa44-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-487">Boolean</span></span>|<span data-ttu-id="1fa44-488">Verwendet, um die Anzeige des Bereichs-Optionen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1fa44-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="1fa44-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="1fa44-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-490">Boolean</span></span>|<span data-ttu-id="1fa44-491">So deaktivieren Sie die Anzeige des Geräts Leistung und der Zustand Bereichs verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="1fa44-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="1fa44-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-493">Boolean</span></span>|<span data-ttu-id="1fa44-494">So deaktivieren Sie die Anzeige des Bereichs Protection Firewall und Netzwerk verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="1fa44-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="1fa44-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-496">Boolean</span></span>|<span data-ttu-id="1fa44-497">So deaktivieren Sie die Anzeige des Bereichs Protection Viren und verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="1fa44-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="1fa44-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-499">Boolean</span></span>|<span data-ttu-id="1fa44-500">So deaktivieren Sie die Anzeige des Bereichs Protection Konto verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="1fa44-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="1fa44-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-502">Boolean</span></span>|<span data-ttu-id="1fa44-503">Verwendet, um die Anzeige des Bereichs Protection Hardware zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1fa44-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="1fa44-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="1fa44-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-505">Boolean</span></span>|<span data-ttu-id="1fa44-506">So deaktivieren Sie die Anzeige des Bereichs Protection Ransomware verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="1fa44-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="1fa44-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-508">Boolean</span></span>|<span data-ttu-id="1fa44-509">So deaktivieren Sie die Anzeige des Bereichs sicheren Boot unter gerätesicherheit verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="1fa44-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="1fa44-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="1fa44-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-511">Boolean</span></span>|<span data-ttu-id="1fa44-512">So deaktivieren Sie die Anzeige des Prozesses Sicherheit unter Sicherheit Gerät Problembehandlung verwendet.</span><span class="sxs-lookup"><span data-stu-id="1fa44-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="1fa44-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fa44-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="1fa44-514">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-514">String</span></span>|<span data-ttu-id="1fa44-515">Der Firmenname, der den Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="1fa44-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="1fa44-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="1fa44-517">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-517">String</span></span>|<span data-ttu-id="1fa44-518">Die e-Mail-Adresse, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="1fa44-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="1fa44-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="1fa44-520">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-520">String</span></span>|<span data-ttu-id="1fa44-521">Die angegebene Rufnummer oder Skype-ID, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="1fa44-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="1fa44-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="1fa44-523">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-523">String</span></span>|<span data-ttu-id="1fa44-524">Das Hilfeportal URL dies für Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="1fa44-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="1fa44-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="1fa44-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="1fa44-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="1fa44-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="1fa44-527">Benachrichtigungen über die angezeigte Bereiche der app angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="1fa44-528">Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="1fa44-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="1fa44-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="1fa44-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="1fa44-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="1fa44-531">Konfigurieren Sie, wie IT-Kontakt anzeigen Informationen für Endbenutzer.</span><span class="sxs-lookup"><span data-stu-id="1fa44-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="1fa44-532">Mögliche Werte: sind `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="1fa44-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="1fa44-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="1fa44-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-534">Boolean</span></span>|<span data-ttu-id="1fa44-535">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="1fa44-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="1fa44-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="1fa44-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="1fa44-537">Int32</span><span class="sxs-lookup"><span data-stu-id="1fa44-537">Int32</span></span>|<span data-ttu-id="1fa44-538">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="1fa44-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="1fa44-539">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="1fa44-540">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="1fa44-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="1fa44-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="1fa44-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="1fa44-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="1fa44-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="1fa44-543">Wählen Sie den vorinstallierten Schlüssel um zu verwendende Codierung.</span><span class="sxs-lookup"><span data-stu-id="1fa44-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="1fa44-544">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="1fa44-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="1fa44-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="1fa44-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-546">Boolean</span></span>|<span data-ttu-id="1fa44-547">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="1fa44-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="1fa44-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="1fa44-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="1fa44-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-549">Boolean</span></span>|<span data-ttu-id="1fa44-550">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="1fa44-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="1fa44-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="1fa44-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-552">Boolean</span></span>|<span data-ttu-id="1fa44-553">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="1fa44-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="1fa44-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="1fa44-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="1fa44-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-555">Boolean</span></span>|<span data-ttu-id="1fa44-556">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="1fa44-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="1fa44-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="1fa44-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="1fa44-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="1fa44-559">Geben Sie an, wie die Certificate Revocation List erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="1fa44-560">Mögliche Werte: sind `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="1fa44-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="1fa44-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="1fa44-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-562">Boolean</span></span>|<span data-ttu-id="1fa44-563">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="1fa44-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="1fa44-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1fa44-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="1fa44-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1fa44-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="1fa44-566">Konfiguriert, wie vom Warteschlangensystem Paket im Szenario mit Tunnel Gateway angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1fa44-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="1fa44-567">Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="1fa44-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="1fa44-568">firewallProfileDomain</span></span>|[<span data-ttu-id="1fa44-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1fa44-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1fa44-570">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="1fa44-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="1fa44-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="1fa44-571">firewallProfilePublic</span></span>|[<span data-ttu-id="1fa44-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1fa44-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1fa44-573">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="1fa44-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="1fa44-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="1fa44-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="1fa44-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1fa44-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1fa44-576">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="1fa44-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="1fa44-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="1fa44-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="1fa44-578">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1fa44-578">String collection</span></span>|<span data-ttu-id="1fa44-579">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="1fa44-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="1fa44-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-582">Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="1fa44-583">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="1fa44-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="1fa44-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-586">Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="1fa44-587">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="1fa44-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="1fa44-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-590">Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte.</span><span class="sxs-lookup"><span data-stu-id="1fa44-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="1fa44-591">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="1fa44-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="1fa44-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-594">Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte.</span><span class="sxs-lookup"><span data-stu-id="1fa44-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="1fa44-595">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="1fa44-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="1fa44-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-598">Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten.</span><span class="sxs-lookup"><span data-stu-id="1fa44-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="1fa44-599">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="1fa44-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="1fa44-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-602">Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten.</span><span class="sxs-lookup"><span data-stu-id="1fa44-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="1fa44-603">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="1fa44-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="1fa44-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-606">Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert.</span><span class="sxs-lookup"><span data-stu-id="1fa44-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="1fa44-607">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="1fa44-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="1fa44-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-610">Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert.</span><span class="sxs-lookup"><span data-stu-id="1fa44-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="1fa44-611">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="1fa44-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="1fa44-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-614">Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code.</span><span class="sxs-lookup"><span data-stu-id="1fa44-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="1fa44-615">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="1fa44-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="1fa44-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-618">Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code.</span><span class="sxs-lookup"><span data-stu-id="1fa44-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="1fa44-619">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="1fa44-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-622">Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="1fa44-623">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="1fa44-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="1fa44-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-626">Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="1fa44-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="1fa44-627">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="1fa44-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="1fa44-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-630">Der Wert, der angibt, wenn die Anmeldeinformationen, die vom Windows lokalen Behörde Teilsystem stehlen zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="1fa44-631">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="1fa44-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="1fa44-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-634">Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="1fa44-635">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="1fa44-636">defenderProcessCreation</span></span>|[<span data-ttu-id="1fa44-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-638">Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="1fa44-639">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="1fa44-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="1fa44-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-642">Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="1fa44-643">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="1fa44-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="1fa44-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-646">Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1fa44-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="1fa44-647">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="1fa44-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="1fa44-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-650">Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien.</span><span class="sxs-lookup"><span data-stu-id="1fa44-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="1fa44-651">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="1fa44-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="1fa44-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-654">Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien.</span><span class="sxs-lookup"><span data-stu-id="1fa44-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="1fa44-655">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="1fa44-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1fa44-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1fa44-658">Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="1fa44-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="1fa44-659">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="1fa44-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="1fa44-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-662">Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="1fa44-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="1fa44-663">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="1fa44-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-666">Wert, der Verwendung der erweiterte Schutz vor Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="1fa44-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="1fa44-667">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="1fa44-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="1fa44-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="1fa44-670">Wert, der das Verhalten der geschützte Ordner.</span><span class="sxs-lookup"><span data-stu-id="1fa44-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="1fa44-671">Mögliche Werte sind: `userDefined`, `enable`, `auditMode`, `blockDiskModification` und `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="1fa44-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="1fa44-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="1fa44-673">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1fa44-673">String collection</span></span>|<span data-ttu-id="1fa44-674">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="1fa44-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="1fa44-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="1fa44-676">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1fa44-676">String collection</span></span>|<span data-ttu-id="1fa44-677">Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="1fa44-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="1fa44-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1fa44-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1fa44-680">Wert, der das Verhalten des NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="1fa44-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="1fa44-681">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1fa44-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="1fa44-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="1fa44-683">Binär</span><span class="sxs-lookup"><span data-stu-id="1fa44-683">Binary</span></span>|<span data-ttu-id="1fa44-684">XML-Inhalte mit Details zum Exploit-Schutz.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="1fa44-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="1fa44-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="1fa44-686">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1fa44-686">String</span></span>|<span data-ttu-id="1fa44-687">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="1fa44-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="1fa44-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="1fa44-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-689">Boolean</span></span>|<span data-ttu-id="1fa44-690">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="1fa44-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="1fa44-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="1fa44-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="1fa44-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="1fa44-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="1fa44-693">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="1fa44-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="1fa44-694">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="1fa44-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="1fa44-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="1fa44-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="1fa44-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="1fa44-697">Anmeldeinformationen Guard aktivieren Sie, wenn Sicherheit Plattformebene mit Secure Boot und Virtualisierung Sicherheit sind beide aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1fa44-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="1fa44-698">Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="1fa44-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="1fa44-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="1fa44-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-700">Boolean</span></span>|<span data-ttu-id="1fa44-701">Schaltet die Virtualisierung basierend Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="1fa44-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="1fa44-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="1fa44-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="1fa44-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-703">Boolean</span></span>|<span data-ttu-id="1fa44-704">Gibt an, ob Sicherheit Plattformebene beim nächsten Neustart aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1fa44-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="1fa44-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="1fa44-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="1fa44-706">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="1fa44-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="1fa44-707">.MD)</span><span class="sxs-lookup"><span data-stu-id="1fa44-707">.md)</span></span>|<span data-ttu-id="1fa44-708">Ermöglicht der IT-Administrator die Einführung von Guard System zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="1fa44-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="1fa44-709">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1fa44-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="1fa44-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="1fa44-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-711">Boolean</span></span>|<span data-ttu-id="1fa44-712">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="1fa44-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="1fa44-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="1fa44-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="1fa44-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-714">Boolean</span></span>|<span data-ttu-id="1fa44-715">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="1fa44-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="1fa44-716">applicationGuardEnabled</span></span>|<span data-ttu-id="1fa44-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-717">Boolean</span></span>|<span data-ttu-id="1fa44-718">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="1fa44-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="1fa44-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="1fa44-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="1fa44-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="1fa44-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="1fa44-721">Aktivieren Sie Windows Defender Anwendung Guard für neuere Versionen von Windows.</span><span class="sxs-lookup"><span data-stu-id="1fa44-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="1fa44-722">Mögliche Werte: sind `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="1fa44-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="1fa44-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="1fa44-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="1fa44-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="1fa44-725">Block Zwischenablage Übertragung Bilddatei, Textdatei oder dürfen.</span><span class="sxs-lookup"><span data-stu-id="1fa44-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="1fa44-726">Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="1fa44-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="1fa44-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="1fa44-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-728">Boolean</span></span>|<span data-ttu-id="1fa44-729">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="1fa44-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="1fa44-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="1fa44-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="1fa44-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-731">Boolean</span></span>|<span data-ttu-id="1fa44-732">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="1fa44-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="1fa44-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="1fa44-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="1fa44-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-734">Boolean</span></span>|<span data-ttu-id="1fa44-735">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="1fa44-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="1fa44-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="1fa44-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="1fa44-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="1fa44-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="1fa44-738">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="1fa44-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="1fa44-739">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="1fa44-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="1fa44-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="1fa44-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="1fa44-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-741">Boolean</span></span>|<span data-ttu-id="1fa44-742">Erlaubt das Drucken im PDF-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="1fa44-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="1fa44-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="1fa44-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-744">Boolean</span></span>|<span data-ttu-id="1fa44-745">Erlaubt das Drucken im XPS-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="1fa44-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="1fa44-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="1fa44-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-747">Boolean</span></span>|<span data-ttu-id="1fa44-748">Erlaubt das Drucken auf lokalen Druckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="1fa44-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="1fa44-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="1fa44-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-750">Boolean</span></span>|<span data-ttu-id="1fa44-751">Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="1fa44-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="1fa44-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="1fa44-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-753">Boolean</span></span>|<span data-ttu-id="1fa44-754">Zulassen der Anwendung Guard virtuellen GPU verwenden</span><span class="sxs-lookup"><span data-stu-id="1fa44-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="1fa44-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="1fa44-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="1fa44-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-756">Boolean</span></span>|<span data-ttu-id="1fa44-757">Zulassen, dass Benutzer Dateien vom Rand im Container Guard Anwendung herunterladen und speichern Sie sie auf dem Host Dateisystem</span><span class="sxs-lookup"><span data-stu-id="1fa44-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="1fa44-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="1fa44-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="1fa44-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-759">Boolean</span></span>|<span data-ttu-id="1fa44-760">Ermöglicht die Admin standard Benutzer während der Teilnahme von Azure AD Encrpytion aktivieren können.</span><span class="sxs-lookup"><span data-stu-id="1fa44-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="1fa44-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="1fa44-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="1fa44-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-762">Boolean</span></span>|<span data-ttu-id="1fa44-763">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1fa44-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="1fa44-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="1fa44-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="1fa44-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-765">Boolean</span></span>|<span data-ttu-id="1fa44-766">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="1fa44-767">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="1fa44-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="1fa44-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="1fa44-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="1fa44-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa44-769">Boolean</span></span>|<span data-ttu-id="1fa44-770">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="1fa44-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="1fa44-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="1fa44-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="1fa44-773">System BitLocker Drive-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="1fa44-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="1fa44-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-774">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="1fa44-775">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-775">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="1fa44-776">BitLocker feste Laufwerk Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="1fa44-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="1fa44-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="1fa44-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1fa44-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="1fa44-779">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="1fa44-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1fa44-780">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fa44-780">Response</span></span>
<span data-ttu-id="1fa44-781">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1fa44-781">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fa44-782">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1fa44-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fa44-783">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fa44-783">Request</span></span>
<span data-ttu-id="1fa44-784">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1fa44-784">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26475

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
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
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
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
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
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
  "deviceGuardLaunchSystemGuard": "enabled",
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
  "bitLockerAllowStandardUserEncryption": true,
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

### <a name="response"></a><span data-ttu-id="1fa44-785">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fa44-785">Response</span></span>
<span data-ttu-id="1fa44-p196">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fa44-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26647

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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
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
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
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
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
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
  "deviceGuardLaunchSystemGuard": "enabled",
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
  "bitLockerAllowStandardUserEncryption": true,
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




