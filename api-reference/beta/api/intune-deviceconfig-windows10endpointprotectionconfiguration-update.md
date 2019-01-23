---
title: Aktualisieren von „windows10EndpointProtectionConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10EndpointProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bb398da325f6895eee7dd5e53938f8dafc5d5f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393620"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="34a69-103">Aktualisieren von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="34a69-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="34a69-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="34a69-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34a69-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34a69-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="34a69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a69-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34a69-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34a69-108">Prerequisites</span></span>
<span data-ttu-id="34a69-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34a69-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34a69-111">Permission type</span></span>|<span data-ttu-id="34a69-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34a69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34a69-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34a69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34a69-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a69-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34a69-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34a69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a69-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34a69-116">Not supported.</span></span>|
|<span data-ttu-id="34a69-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34a69-117">Application</span></span>|<span data-ttu-id="34a69-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34a69-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34a69-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34a69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="34a69-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34a69-120">Request headers</span></span>
|<span data-ttu-id="34a69-121">Header</span><span class="sxs-lookup"><span data-stu-id="34a69-121">Header</span></span>|<span data-ttu-id="34a69-122">Wert</span><span class="sxs-lookup"><span data-stu-id="34a69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34a69-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="34a69-123">Authorization</span></span>|<span data-ttu-id="34a69-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34a69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34a69-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="34a69-125">Accept</span></span>|<span data-ttu-id="34a69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34a69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a69-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34a69-127">Request body</span></span>
<span data-ttu-id="34a69-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="34a69-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="34a69-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="34a69-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="34a69-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34a69-130">Property</span></span>|<span data-ttu-id="34a69-131">Typ</span><span class="sxs-lookup"><span data-stu-id="34a69-131">Type</span></span>|<span data-ttu-id="34a69-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34a69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a69-133">id</span><span class="sxs-lookup"><span data-stu-id="34a69-133">id</span></span>|<span data-ttu-id="34a69-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-134">String</span></span>|<span data-ttu-id="34a69-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="34a69-135">Key of the entity.</span></span> <span data-ttu-id="34a69-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34a69-137">lastModifiedDateTime</span></span>|<span data-ttu-id="34a69-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a69-138">DateTimeOffset</span></span>|<span data-ttu-id="34a69-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="34a69-139">DateTime the object was last modified.</span></span> <span data-ttu-id="34a69-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34a69-141">roleScopeTagIds</span></span>|<span data-ttu-id="34a69-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="34a69-142">String collection</span></span>|<span data-ttu-id="34a69-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="34a69-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34a69-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34a69-145">supportsScopeTags</span></span>|<span data-ttu-id="34a69-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-146">Boolean</span></span>|<span data-ttu-id="34a69-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34a69-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34a69-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34a69-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-150">This property is read-only.</span></span> <span data-ttu-id="34a69-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34a69-152">createdDateTime</span></span>|<span data-ttu-id="34a69-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a69-153">DateTimeOffset</span></span>|<span data-ttu-id="34a69-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="34a69-154">DateTime the object was created.</span></span> <span data-ttu-id="34a69-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-156">description</span><span class="sxs-lookup"><span data-stu-id="34a69-156">description</span></span>|<span data-ttu-id="34a69-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-157">String</span></span>|<span data-ttu-id="34a69-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="34a69-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34a69-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-160">displayName</span><span class="sxs-lookup"><span data-stu-id="34a69-160">displayName</span></span>|<span data-ttu-id="34a69-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-161">String</span></span>|<span data-ttu-id="34a69-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="34a69-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34a69-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-164">Version</span><span class="sxs-lookup"><span data-stu-id="34a69-164">version</span></span>|<span data-ttu-id="34a69-165">Int32</span><span class="sxs-lookup"><span data-stu-id="34a69-165">Int32</span></span>|<span data-ttu-id="34a69-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="34a69-166">Version of the device configuration.</span></span> <span data-ttu-id="34a69-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a69-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a69-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="34a69-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="34a69-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="34a69-170">Diese Richtlinie soll gegen externe DMA Geräten zusätzliche Sicherheit zu bieten.</span><span class="sxs-lookup"><span data-stu-id="34a69-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="34a69-171">Es ermöglicht den für größere Kontrolle über die Enumeration von externen DMA-Geräten mit Sandkästen und DMA Remapping/Gerät Arbeitsspeicher Isolation nicht kompatibel.</span><span class="sxs-lookup"><span data-stu-id="34a69-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="34a69-172">Diese Richtlinie wird nur wirksam, wenn Kernel DMA Protection unterstützt und von der Systemfirmware aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="34a69-173">Kernel DMA Schutz ist ein Plattform-Feature, das über Gruppenrichtlinie oder durch Endbenutzer gesteuert werden kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="34a69-174">Dies ist nur zum Zeitpunkt der Produktion vom System unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="34a69-175">Um zu überprüfen, ob das System Kernel DMA Protection unterstützt, überprüfen Sie das Kernel DMA Protection-Feld in der Seite Zusammenfassung des MSINFO32.exe ein.</span><span class="sxs-lookup"><span data-stu-id="34a69-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="34a69-176">Mögliche Werte sind: `deviceDefault`, `blockAll` und `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="34a69-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="34a69-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="34a69-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="34a69-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-179">Diese Berechtigung wird während der Sicherung/Wiederherstellung von Anmeldeinformations-Manager verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="34a69-180">Gespeicherten Anmeldeinformationen der Benutzer können beeinträchtigt werden, wenn diese Berechtigung für die anderen Entitäten angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="34a69-181">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="34a69-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="34a69-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-184">Diese Berechtigung bestimmt, welche Benutzer und Gruppen mit dem Computer über das Netzwerk herstellen dürfen.</span><span class="sxs-lookup"><span data-stu-id="34a69-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="34a69-185">State zugelassen wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="34a69-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="34a69-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="34a69-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-188">Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Block aus eine Verbindung mit dem Computer über das Netzwerk sind.</span><span class="sxs-lookup"><span data-stu-id="34a69-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="34a69-189">State-Block wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-189">State Block is supported.</span></span>|
|<span data-ttu-id="34a69-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="34a69-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="34a69-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-192">Diese Berechtigung ermöglicht es einem Prozess zum Identitätswechsel für alle Benutzer ohne Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="34a69-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="34a69-193">Der Prozess kann daher auf dieselben lokalen Ressourcen wie der Benutzer zugreifen.</span><span class="sxs-lookup"><span data-stu-id="34a69-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="34a69-194">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="34a69-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="34a69-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-197">Dieser Benutzer Rechte bestimmt, welche Benutzer am Computer anmelden können.</span><span class="sxs-lookup"><span data-stu-id="34a69-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="34a69-198">Status nicht konfiguriert, zugelassen und blockiert werden alle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="34a69-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="34a69-199">userRightsBackupData</span></span>|[<span data-ttu-id="34a69-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-201">Diese Rechte Benutzer bestimmt, welche Benutzer Datei-, Verzeichnis-, Registrierung und andere beständige Objekte Berechtigungen beim Sichern der Dateien und Verzeichnisse umgehen können.</span><span class="sxs-lookup"><span data-stu-id="34a69-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="34a69-202">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="34a69-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="34a69-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-205">Dieser Benutzer Rechte bestimmt, welche Benutzer und Gruppen Uhrzeit und Datum der internen Uhr des Computers ändern können.</span><span class="sxs-lookup"><span data-stu-id="34a69-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="34a69-206">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="34a69-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="34a69-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-209">Diese Einstellung bestimmt, ob Benutzer globale Objekte erstellen können, die alle Sitzungen zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="34a69-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="34a69-210">Benutzer, die globale Objekte erstellen können, können es sich um Prozesse auswirken, die unter anderer Benutzer Sitzungen, ausgeführt wird und zu Anwendung Fehler und Datenverlust führen kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="34a69-211">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="34a69-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="34a69-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-214">Diese Berechtigung bestimmt, welche Benutzer und Gruppen können eine interne API zum Erstellen und Ändern der Größe der Auslagerungsdatei aufrufen.</span><span class="sxs-lookup"><span data-stu-id="34a69-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="34a69-215">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="34a69-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="34a69-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-218">Diese Rechte Benutzer bestimmt, welche Konten von Prozessen verwendet werden können, um ein Verzeichnisobjekt mithilfe des Objekts-Manager erstellen.</span><span class="sxs-lookup"><span data-stu-id="34a69-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="34a69-219">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="34a69-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="34a69-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-222">Dieser Benutzer Rechte bestimmt, ob der Benutzer eine symbolische Verbindung vom Computer erstellen kann, an dem sie angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="34a69-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="34a69-223">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="34a69-224">userRightsCreateToken</span></span>|[<span data-ttu-id="34a69-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-226">Diese Berechtigung bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token erstellen, die Zugriff auf alle lokalen Ressourcen abrufen, wenn der Prozess eine interne API verwendet, um ein Zugriffstoken erstellen verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="34a69-227">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="34a69-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="34a69-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-230">Diese Rechte Benutzer bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können.</span><span class="sxs-lookup"><span data-stu-id="34a69-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="34a69-231">Nur die Bundesländer nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="34a69-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="34a69-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="34a69-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-234">Diese Berechtigung bestimmt, welche Benutzer und Gruppen nicht zulässig sind, als Remote Desktop Services Client anmelden.</span><span class="sxs-lookup"><span data-stu-id="34a69-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="34a69-235">Nur die Bundesländer nicht konfiguriert und blockiert werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="34a69-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="34a69-236">userRightsDelegation</span></span>|[<span data-ttu-id="34a69-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-238">Dieser Benutzer Rechte bestimmt, welche Benutzer die vertrauenswürdige für Delegierung Einstellung für ein Benutzer- oder Computerkonto-Objekt festlegen können.</span><span class="sxs-lookup"><span data-stu-id="34a69-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="34a69-239">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="34a69-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="34a69-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-242">Dieser Benutzer Rechte bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen im Sicherheitsprotokoll verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="34a69-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="34a69-243">Sicherheitsprotokoll wird verwendet, um autorisierter Zugriff zu verfolgen.</span><span class="sxs-lookup"><span data-stu-id="34a69-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="34a69-244">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="34a69-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="34a69-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-247">Zuweisen von diesem Benutzerrecht keinem Benutzer kann für diesen Benutzer zum Annehmen der Clientidentität ausgeführte Programme.</span><span class="sxs-lookup"><span data-stu-id="34a69-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="34a69-248">Voraussetzen dieses Benutzerrecht für diese Art des Identitätswechsels verhindert, dass einen nicht autorisierten Benutzer aus überzeugende einen Client eine Verbindung zu einem Dienst, die sie erstellt haben, und klicken Sie dann Identitätswechsel bei dieser Client, dem der nicht autorisierte Benutzer Berechtigungen zu erhöhen können Administrative oder Systemebenen.</span><span class="sxs-lookup"><span data-stu-id="34a69-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="34a69-249">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="34a69-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="34a69-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-252">Diese Rechte Benutzer bestimmt, welche Konten einen Prozess mit Schreibzugriff auf einen anderen Prozess verwenden können, um die Ausführungspriorität zugewiesen an den anderen Prozess zu erhöhen.</span><span class="sxs-lookup"><span data-stu-id="34a69-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="34a69-253">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="34a69-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="34a69-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-256">Dieser Benutzer Rechte bestimmt, welche Benutzer können dynamisch laden und entladen Gerätetreiber oder anderen Code im Kernelmodus.</span><span class="sxs-lookup"><span data-stu-id="34a69-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="34a69-257">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="34a69-258">userRightsLockMemory</span></span>|[<span data-ttu-id="34a69-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-260">Dieser Benutzer Rechte bestimmt, welche Konten einen Prozess Speichern von Daten im physikalischen Speicher, wodurch das System verhindert, dass die Daten in den virtuellen Speicher auf dem Datenträger paging verwenden können.</span><span class="sxs-lookup"><span data-stu-id="34a69-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="34a69-261">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="34a69-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="34a69-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-264">Diese Berechtigung bestimmt, welche Benutzer Objekt den Optionen für einzelne Ressourcen, wie Dateien, Active Directory-Objekte und Registrierungsschlüssel für die Überwachung angeben können.</span><span class="sxs-lookup"><span data-stu-id="34a69-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="34a69-265">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="34a69-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="34a69-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-268">Diese Rechte Benutzer bestimmt der Benutzer und Gruppen auf einem Datenträger, wie remote Defragmentierung Wartungsaufgaben ausführen können.</span><span class="sxs-lookup"><span data-stu-id="34a69-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="34a69-269">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="34a69-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="34a69-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-272">Diese Berechtigung bestimmt, Firmware-Umgebungsvariablen geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="34a69-273">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="34a69-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="34a69-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-276">Dieser Benutzer Rechte bestimmt, welche Benutzerkonten die Bezeichnung Integrität von Objekten, wie Dateien, Registrierungsschlüssel oder Prozesse, die im Besitz von anderen Benutzern ändern können.</span><span class="sxs-lookup"><span data-stu-id="34a69-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="34a69-277">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="34a69-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="34a69-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-280">Dieser Benutzer Rechte bestimmt, welche Benutzer Tools zum Überwachen der Leistung verwenden können, zur Überwachung der Leistung der Systemprozesse.</span><span class="sxs-lookup"><span data-stu-id="34a69-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="34a69-281">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="34a69-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="34a69-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-284">Dieser Benutzer Rechte bestimmt, welche Benutzer dürfen Herunterfahren eines Computers von einem Remotestandort im Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="34a69-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="34a69-285">Missbrauch dieses Benutzerrechts kann ein Denial-of-Service führen.</span><span class="sxs-lookup"><span data-stu-id="34a69-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="34a69-286">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="34a69-287">userRightsRestoreData</span></span>|[<span data-ttu-id="34a69-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-289">Diese Berechtigung bestimmt, welche Benutzer umgehen können Datei-, Verzeichnis-, Registrierung und andere beständige Objekte, die Berechtigungen, die beim Wiederherstellen von Dateien und Verzeichnisse gesichert und bestimmt, welche Benutzer einen beliebigen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können.</span><span class="sxs-lookup"><span data-stu-id="34a69-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="34a69-290">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="34a69-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="34a69-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-293">Dieser Benutzer Rechte bestimmt, welche Benutzer die Besitzrechte für ein beliebiges sicherungsfähiges Objekt in das System, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads übernehmen können.</span><span class="sxs-lookup"><span data-stu-id="34a69-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="34a69-294">Nur Zustände nicht konfiguriert und zugelassen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="34a69-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="34a69-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="34a69-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="34a69-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="34a69-297">Diese Einstellung legt fest, welche Dienstkonten für das Registrieren von eines Prozess als Dienst gehindert werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="34a69-298">Hinweis: Diese Einstellung gilt nicht für die Konten System, lokaler Dienst oder Netzwerkdienst.</span><span class="sxs-lookup"><span data-stu-id="34a69-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="34a69-299">Nur Status blockiert wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a69-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="34a69-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="34a69-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="34a69-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-301">Boolean</span></span>|<span data-ttu-id="34a69-302">Diese Einstellung bestimmt, ob Xbox Spiel speichern aktiviert (1) oder deaktiviert (0) ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="34a69-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="34a69-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="34a69-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="34a69-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="34a69-305">Diese Einstellung bestimmt, ob der Verwaltungsdienst Zubehör Starttyp Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="34a69-306">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="34a69-306">Default: Manual.</span></span> <span data-ttu-id="34a69-307">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="34a69-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="34a69-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="34a69-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="34a69-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="34a69-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="34a69-310">Diese Einstellung bestimmt, ob Starttyp Live Auth-Manager-Dienst Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="34a69-311">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="34a69-311">Default: Manual.</span></span> <span data-ttu-id="34a69-312">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="34a69-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="34a69-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="34a69-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="34a69-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="34a69-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="34a69-315">Diese Einstellung bestimmt, ob Live Spiel Speichern des Dienstes Starttyp Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="34a69-316">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="34a69-316">Default: Manual.</span></span> <span data-ttu-id="34a69-317">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="34a69-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="34a69-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="34a69-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="34a69-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="34a69-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="34a69-320">Diese Einstellung bestimmt, ob Starttyp Networking-Dienst Automatic(2), Manual(3), Disabled(4) ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="34a69-321">Standard: manuell.</span><span class="sxs-lookup"><span data-stu-id="34a69-321">Default: Manual.</span></span> <span data-ttu-id="34a69-322">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="34a69-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="34a69-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="34a69-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="34a69-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-324">Boolean</span></span>|<span data-ttu-id="34a69-325">Hindert Benutzer am Hinzufügen von neuen Microsoft-Konten auf diesem Computer.</span><span class="sxs-lookup"><span data-stu-id="34a69-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="34a69-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="34a69-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="34a69-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-327">Boolean</span></span>|<span data-ttu-id="34a69-328">Aktivieren Sie lokale Konten, die nicht von anderen Orten als physisches Gerät anmelden, um kennwortgeschützte sind. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="34a69-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="34a69-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="34a69-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="34a69-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-330">Boolean</span></span>|<span data-ttu-id="34a69-331">Bestimmt, ob das lokale Administratorkonto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="34a69-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="34a69-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="34a69-333">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-333">String</span></span>|<span data-ttu-id="34a69-334">Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="34a69-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="34a69-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="34a69-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="34a69-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-336">Boolean</span></span>|<span data-ttu-id="34a69-337">Bestimmt, ob das Konto Gast aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="34a69-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="34a69-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="34a69-339">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-339">String</span></span>|<span data-ttu-id="34a69-340">Definieren Sie einen anderen Kontonamen an, die Sicherheits-ID (SID) für das Konto "Gast" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="34a69-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="34a69-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="34a69-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="34a69-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-342">Boolean</span></span>|<span data-ttu-id="34a69-343">Verhindern Sie, dass eines portablen Computers ohne Anmeldung abgedockt werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="34a69-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="34a69-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="34a69-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-345">Boolean</span></span>|<span data-ttu-id="34a69-346">Installieren von Druckertreiber als Teil des Herstellens einer Verbindung zu einem freigegebenen Drucker Admins nur zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="34a69-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="34a69-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="34a69-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="34a69-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-348">Boolean</span></span>|<span data-ttu-id="34a69-349">Aktivieren diese Einstellungen kann nur interaktiv angemeldeten Benutzer auf CD-ROM-Medien zugreifen.</span><span class="sxs-lookup"><span data-stu-id="34a69-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="34a69-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="34a69-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="34a69-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="34a69-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="34a69-352">Definieren Sie, wer berechtigt ist, zu formatieren und NTFS-Wechselmedium ausschließen.</span><span class="sxs-lookup"><span data-stu-id="34a69-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="34a69-353">Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="34a69-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="34a69-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="34a69-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="34a69-355">Int32</span><span class="sxs-lookup"><span data-stu-id="34a69-355">Int32</span></span>|<span data-ttu-id="34a69-356">Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="34a69-357">Gültige Werte von 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="34a69-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="34a69-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="34a69-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="34a69-359">Int32</span><span class="sxs-lookup"><span data-stu-id="34a69-359">Int32</span></span>|<span data-ttu-id="34a69-360">Definieren Sie maximale Minuten der Inaktivität auf dem interaktiven Desktop Anmeldebildschirm, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="34a69-361">Gültige Werte von 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="34a69-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="34a69-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="34a69-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="34a69-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-363">Boolean</span></span>|<span data-ttu-id="34a69-364">Benötigen Sie STRG + ALT + ENTF gedrückt werden, bevor ein Benutzer anmelden kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="34a69-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="34a69-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="34a69-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-366">Boolean</span></span>|<span data-ttu-id="34a69-367">Der Benutzername der letzten Person ein, die Anmeldung auf dem Gerät nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34a69-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="34a69-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="34a69-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="34a69-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-369">Boolean</span></span>|<span data-ttu-id="34a69-370">Der Benutzername der Person, die dieses Gerät anmelden, nachdem Anmeldeinformationen eingegeben wurden und bevor der Desktop des Geräts angezeigt wird nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34a69-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="34a69-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="34a69-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="34a69-372">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-372">String</span></span>|<span data-ttu-id="34a69-373">Festlegen Sie Titel der Nachricht für Benutzer, die versuchen, melden Sie sich bei.</span><span class="sxs-lookup"><span data-stu-id="34a69-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="34a69-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="34a69-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="34a69-375">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-375">String</span></span>|<span data-ttu-id="34a69-376">Festlegen des Nachrichtentexts für Benutzer, die sich anmelden.</span><span class="sxs-lookup"><span data-stu-id="34a69-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="34a69-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="34a69-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="34a69-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-378">Boolean</span></span>|<span data-ttu-id="34a69-379">Block PKU2U authentifizierungsanforderungen an dieses Gerät online-Identitäten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="34a69-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="34a69-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="34a69-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="34a69-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-381">Boolean</span></span>|<span data-ttu-id="34a69-382">UI-Hilfsprogramm für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager Entität boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="34a69-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="34a69-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="34a69-384">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-384">String</span></span>|<span data-ttu-id="34a69-385">Bearbeiten Sie die Security Descriptor Definition Language Standardzeichenfolge zum gewähren oder verweigern, Benutzer und Gruppen, um die SAM remote anzurufen.</span><span class="sxs-lookup"><span data-stu-id="34a69-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="34a69-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="34a69-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="34a69-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="34a69-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="34a69-388">Diese Einstellung kann ein Client die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="34a69-389">Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="34a69-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="34a69-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="34a69-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="34a69-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="34a69-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="34a69-392">Diese Einstellung kann ein Server die Aushandlung von 128-Bit-Verschlüsselung und/oder sitzungssicherheit NTLMv2 erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="34a69-393">Mögliche Werte: sind `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="34a69-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="34a69-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="34a69-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="34a69-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="34a69-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="34a69-396">Diese Einstellung bestimmt, welche Herausforderung/Antwort-Authentifizierungsprotokoll Netzwerk Anmeldungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="34a69-397">Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="34a69-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="34a69-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="34a69-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="34a69-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-399">Boolean</span></span>|<span data-ttu-id="34a69-400">Wenn aktiviert, wird der SMB-Client unsichere Gast Anmeldungen zulassen.</span><span class="sxs-lookup"><span data-stu-id="34a69-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="34a69-401">Falls nicht konfiguriert, wird der SMB-Client unsichere Gast Anmeldungen abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="34a69-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="34a69-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="34a69-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="34a69-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-403">Boolean</span></span>|<span data-ttu-id="34a69-404">Diese Einstellung bestimmt, ob die Auslagerungsdatei beim Herunterfahren des Systems gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="34a69-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="34a69-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="34a69-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-406">Boolean</span></span>|<span data-ttu-id="34a69-407">Diese Einstellung bestimmt, ob es sich bei ein Computer beendet werden kann, ohne bei Windows anmelden.</span><span class="sxs-lookup"><span data-stu-id="34a69-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="34a69-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="34a69-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="34a69-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-409">Boolean</span></span>|<span data-ttu-id="34a69-410">Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop.</span><span class="sxs-lookup"><span data-stu-id="34a69-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="34a69-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="34a69-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="34a69-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-412">Boolean</span></span>|<span data-ttu-id="34a69-413">Virtualisieren von Datei- und -Schreibvorgänge mit Fehlern an pro Benutzer Speicherorte</span><span class="sxs-lookup"><span data-stu-id="34a69-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="34a69-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="34a69-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="34a69-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-415">Boolean</span></span>|<span data-ttu-id="34a69-416">Erzwingen Sie PKI-Zertifizierung Pfad Überprüfung für eine bestimmte ausführbare Datei, bevor er ausführen kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="34a69-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="34a69-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="34a69-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="34a69-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="34a69-419">Definieren Sie das Verhalten der Aufforderung für Administratoren im Administratormodus Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="34a69-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="34a69-420">Mögliche Werte sind: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent` und `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="34a69-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="34a69-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="34a69-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="34a69-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="34a69-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="34a69-423">Definieren Sie das Verhalten der Elevation Ansage für Standardbenutzer.</span><span class="sxs-lookup"><span data-stu-id="34a69-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="34a69-424">Mögliche Werte: sind `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="34a69-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="34a69-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="34a69-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="34a69-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-426">Boolean</span></span>|<span data-ttu-id="34a69-427">Aktivieren Sie alle Elevation-Anforderungen, fahren Sie mit dem sicheren Desktop, sondern den interaktiven Desktop des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="34a69-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="34a69-428">Richtlinien für Administratoren und Standardbenutzer Prompt Verhalten dienen.</span><span class="sxs-lookup"><span data-stu-id="34a69-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="34a69-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="34a69-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="34a69-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-430">Boolean</span></span>|<span data-ttu-id="34a69-431">App Installationen mit erhöhte Berechtigungen werden für die Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="34a69-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="34a69-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="34a69-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="34a69-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-433">Boolean</span></span>|<span data-ttu-id="34a69-434">Ermöglichen Sie UIAccess apps Elevation einzugeben, mit dem sicheren Desktop. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="34a69-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="34a69-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="34a69-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="34a69-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-436">Boolean</span></span>|<span data-ttu-id="34a69-437">Definiert, ob das integrierte Administratorkonto Administratormodus Genehmigung verwendet oder alle apps mit vollständigen Administratorberechtigungen ausgeführt wird. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="34a69-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="34a69-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="34a69-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="34a69-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-439">Boolean</span></span>|<span data-ttu-id="34a69-440">Definieren Sie, ob Administratormodus Genehmigung und alle UAC-Richtlinieneinstellungen aktiviert sind, ist standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="34a69-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="34a69-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="34a69-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="34a69-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="34a69-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="34a69-443">Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="34a69-444">Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34a69-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="34a69-445">Mögliche Werte: sind `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="34a69-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="34a69-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="34a69-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="34a69-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="34a69-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="34a69-448">Konfigurieren Sie die Benutzerinformationen, die angezeigt wird, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="34a69-449">Falls nicht konfiguriert, werden Anzeigename des Benutzers, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34a69-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="34a69-450">Mögliche Werte: sind `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="34a69-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="34a69-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="34a69-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="34a69-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-452">Boolean</span></span>|<span data-ttu-id="34a69-453">Diese Einstellung bestimmt, ob der SMB-Client versucht, SMB-Paketsignatur aushandeln.</span><span class="sxs-lookup"><span data-stu-id="34a69-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="34a69-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="34a69-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="34a69-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-455">Boolean</span></span>|<span data-ttu-id="34a69-456">Diese Einstellung bestimmt, ob die Clientkomponente für SMB-Paketsignatur erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="34a69-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="34a69-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="34a69-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-458">Boolean</span></span>|<span data-ttu-id="34a69-459">Wenn diese Einstellung aktiviert ist, kann der Server Message Block (SMB) Redirector nur-Text-Kennwörter an nicht - Microsoft SMB-Server zu senden, die keine für die Verschlüsselung von Kennwörtern während der Authentifizierung Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="34a69-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="34a69-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="34a69-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="34a69-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-461">Boolean</span></span>|<span data-ttu-id="34a69-462">Diese Einstellung bestimmt, ob die SMB-Server-Komponente Paketsignatur erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="34a69-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="34a69-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="34a69-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-464">Boolean</span></span>|<span data-ttu-id="34a69-465">Diese Einstellung bestimmt, ob der SMB Server SMB-Paketsignatur mit Clients, die diese anfordern aushandeln kann.</span><span class="sxs-lookup"><span data-stu-id="34a69-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="34a69-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="34a69-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="34a69-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-467">Boolean</span></span>|<span data-ttu-id="34a69-468">Diese Einstellung schränkt standardmäßig anonymen Zugriff auf Freigaben und Pipes an den Einstellungen für named Pipes, die anonym zugegriffen werden können und Freigaben, die anonym zugegriffen werden kann</span><span class="sxs-lookup"><span data-stu-id="34a69-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="34a69-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="34a69-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="34a69-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-470">Boolean</span></span>|<span data-ttu-id="34a69-471">Diese Einstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="34a69-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="34a69-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="34a69-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="34a69-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-473">Boolean</span></span>|<span data-ttu-id="34a69-474">Diese Einstellung bestimmt, ob anonyme Benutzer zum Ausführen bestimmter Aktivitäten, beispielsweise die Namen von Domänenkonten und Netzwerkfreigaben auflisten können.</span><span class="sxs-lookup"><span data-stu-id="34a69-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="34a69-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="34a69-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="34a69-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-476">Boolean</span></span>|<span data-ttu-id="34a69-477">Diese Einstellung bestimmt, ob, an die nächste Änderung des Kennworts, der Hashwert LAN Manager (LM) für das neue Kennwort gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="34a69-478">Es wird nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="34a69-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="34a69-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="34a69-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="34a69-480">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="34a69-480">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="34a69-481">Diese Einstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Leser entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="34a69-482">Mögliche Werte: sind `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="34a69-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="34a69-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="34a69-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="34a69-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-484">Boolean</span></span>|<span data-ttu-id="34a69-485">So deaktivieren Sie die Anzeige des Bereichs Protection app und Browser verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="34a69-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="34a69-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="34a69-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-487">Boolean</span></span>|<span data-ttu-id="34a69-488">Verwendet, um die Anzeige des Bereichs-Optionen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="34a69-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="34a69-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="34a69-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="34a69-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-490">Boolean</span></span>|<span data-ttu-id="34a69-491">So deaktivieren Sie die Anzeige des Geräts Leistung und der Zustand Bereichs verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="34a69-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="34a69-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="34a69-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-493">Boolean</span></span>|<span data-ttu-id="34a69-494">So deaktivieren Sie die Anzeige des Bereichs Protection Firewall und Netzwerk verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="34a69-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="34a69-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="34a69-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-496">Boolean</span></span>|<span data-ttu-id="34a69-497">So deaktivieren Sie die Anzeige des Bereichs Protection Viren und verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="34a69-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="34a69-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="34a69-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-499">Boolean</span></span>|<span data-ttu-id="34a69-500">So deaktivieren Sie die Anzeige des Bereichs Protection Konto verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="34a69-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="34a69-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="34a69-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-502">Boolean</span></span>|<span data-ttu-id="34a69-503">Verwendet, um die Anzeige des Bereichs Protection Hardware zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="34a69-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="34a69-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="34a69-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="34a69-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-505">Boolean</span></span>|<span data-ttu-id="34a69-506">So deaktivieren Sie die Anzeige des Bereichs Protection Ransomware verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="34a69-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="34a69-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="34a69-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-508">Boolean</span></span>|<span data-ttu-id="34a69-509">So deaktivieren Sie die Anzeige des Bereichs sicheren Boot unter gerätesicherheit verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="34a69-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="34a69-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="34a69-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-511">Boolean</span></span>|<span data-ttu-id="34a69-512">So deaktivieren Sie die Anzeige des Prozesses Sicherheit unter Sicherheit Gerät Problembehandlung verwendet.</span><span class="sxs-lookup"><span data-stu-id="34a69-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="34a69-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="34a69-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="34a69-514">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-514">String</span></span>|<span data-ttu-id="34a69-515">Der Firmenname, der den Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="34a69-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="34a69-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="34a69-517">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-517">String</span></span>|<span data-ttu-id="34a69-518">Die e-Mail-Adresse, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="34a69-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="34a69-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="34a69-520">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-520">String</span></span>|<span data-ttu-id="34a69-521">Die angegebene Rufnummer oder Skype-ID, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="34a69-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="34a69-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="34a69-523">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-523">String</span></span>|<span data-ttu-id="34a69-524">Das Hilfeportal URL dies für Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="34a69-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="34a69-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="34a69-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="34a69-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="34a69-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="34a69-527">Benachrichtigungen über die angezeigte Bereiche der app angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34a69-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="34a69-528">Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="34a69-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="34a69-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="34a69-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="34a69-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="34a69-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="34a69-531">Konfigurieren Sie, wie IT-Kontakt anzeigen Informationen für Endbenutzer.</span><span class="sxs-lookup"><span data-stu-id="34a69-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="34a69-532">Mögliche Werte: sind `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="34a69-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="34a69-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="34a69-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="34a69-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-534">Boolean</span></span>|<span data-ttu-id="34a69-535">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="34a69-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="34a69-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="34a69-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="34a69-537">Int32</span><span class="sxs-lookup"><span data-stu-id="34a69-537">Int32</span></span>|<span data-ttu-id="34a69-538">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="34a69-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="34a69-539">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="34a69-540">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="34a69-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="34a69-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="34a69-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="34a69-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="34a69-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="34a69-543">Wählen Sie den vorinstallierten Schlüssel um zu verwendende Codierung.</span><span class="sxs-lookup"><span data-stu-id="34a69-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="34a69-544">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="34a69-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="34a69-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="34a69-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="34a69-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-546">Boolean</span></span>|<span data-ttu-id="34a69-547">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="34a69-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="34a69-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="34a69-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="34a69-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-549">Boolean</span></span>|<span data-ttu-id="34a69-550">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="34a69-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="34a69-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="34a69-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-552">Boolean</span></span>|<span data-ttu-id="34a69-553">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="34a69-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="34a69-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="34a69-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="34a69-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-555">Boolean</span></span>|<span data-ttu-id="34a69-556">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="34a69-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="34a69-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="34a69-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="34a69-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="34a69-559">Geben Sie an, wie die Certificate Revocation List erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="34a69-560">Mögliche Werte: sind `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="34a69-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="34a69-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="34a69-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="34a69-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-562">Boolean</span></span>|<span data-ttu-id="34a69-563">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="34a69-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="34a69-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="34a69-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="34a69-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="34a69-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="34a69-566">Konfiguriert, wie vom Warteschlangensystem Paket im Szenario mit Tunnel Gateway angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="34a69-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="34a69-567">Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="34a69-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="34a69-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="34a69-568">firewallProfileDomain</span></span>|[<span data-ttu-id="34a69-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="34a69-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="34a69-570">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="34a69-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="34a69-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="34a69-571">firewallProfilePublic</span></span>|[<span data-ttu-id="34a69-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="34a69-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="34a69-573">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="34a69-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="34a69-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="34a69-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="34a69-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="34a69-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="34a69-576">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="34a69-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="34a69-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="34a69-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="34a69-578">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="34a69-578">String collection</span></span>|<span data-ttu-id="34a69-579">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="34a69-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="34a69-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="34a69-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-582">Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="34a69-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="34a69-583">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="34a69-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="34a69-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-586">Wert, der das Verhalten des Office-Clientanwendungen, die er in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="34a69-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="34a69-587">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="34a69-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="34a69-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-590">Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte.</span><span class="sxs-lookup"><span data-stu-id="34a69-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="34a69-591">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="34a69-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="34a69-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-594">Wert, der das Verhalten von Office-Anwendungen/Makros erstellen, oder starten die ausführbare Inhalte.</span><span class="sxs-lookup"><span data-stu-id="34a69-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="34a69-595">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="34a69-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="34a69-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-598">Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten.</span><span class="sxs-lookup"><span data-stu-id="34a69-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="34a69-599">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="34a69-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="34a69-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-602">Wert, der das Verhalten des Office-Anwendung, die untergeordnete Prozesse starten.</span><span class="sxs-lookup"><span data-stu-id="34a69-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="34a69-603">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="34a69-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="34a69-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-606">Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert.</span><span class="sxs-lookup"><span data-stu-id="34a69-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="34a69-607">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="34a69-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="34a69-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-610">Der Wert, der angibt, dass das Verhalten der Win32 aus Code der Makros in Office importiert.</span><span class="sxs-lookup"><span data-stu-id="34a69-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="34a69-611">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="34a69-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="34a69-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-614">Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code.</span><span class="sxs-lookup"><span data-stu-id="34a69-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="34a69-615">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="34a69-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="34a69-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-618">Wert, der das Verhalten von verschleierte Js, Vbs/Ps-/ Makro Code.</span><span class="sxs-lookup"><span data-stu-id="34a69-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="34a69-619">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="34a69-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="34a69-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-622">Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="34a69-623">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="34a69-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="34a69-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-626">Wert, der das Verhalten des Js/Vbs Nutzlast ausführen, die vom Internet heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="34a69-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="34a69-627">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="34a69-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="34a69-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-630">Der Wert, der angibt, wenn die Anmeldeinformationen, die vom Windows lokalen Behörde Teilsystem stehlen zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="34a69-631">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="34a69-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="34a69-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-634">Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt.</span><span class="sxs-lookup"><span data-stu-id="34a69-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="34a69-635">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="34a69-636">defenderProcessCreation</span></span>|[<span data-ttu-id="34a69-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-638">Wert, der angibt, Reaktion auf Prozess Kreationen PSExec und WMI-Befehle stammt.</span><span class="sxs-lookup"><span data-stu-id="34a69-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="34a69-639">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="34a69-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="34a69-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-642">Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="34a69-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="34a69-643">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="34a69-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="34a69-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-646">Wert, der als Antwort auf nicht vertrauenswürdigen und nicht signierte Prozesse, die über USB ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="34a69-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="34a69-647">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="34a69-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="34a69-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-650">Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien.</span><span class="sxs-lookup"><span data-stu-id="34a69-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="34a69-651">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="34a69-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="34a69-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-654">Wert, der als Antwort auf ausführbare Dateien, die keiner Verbreitung, Alter oder Liste der vertrauenswürdigen erfüllen Kriterien.</span><span class="sxs-lookup"><span data-stu-id="34a69-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="34a69-655">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="34a69-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="34a69-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="34a69-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="34a69-658">Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="34a69-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="34a69-659">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="34a69-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="34a69-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-662">Der Wert, der angibt, wenn die Ausführung der ausführbaren Inhalt (Exe, Dll, Ps, Js, Vbs usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="34a69-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="34a69-663">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="34a69-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-666">Wert, der Verwendung der erweiterte Schutz vor Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="34a69-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="34a69-667">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="34a69-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="34a69-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="34a69-670">Wert, der das Verhalten der geschützte Ordner.</span><span class="sxs-lookup"><span data-stu-id="34a69-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="34a69-671">Mögliche Werte sind: `userDefined`, `enable`, `auditMode`, `blockDiskModification` und `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="34a69-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="34a69-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="34a69-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="34a69-673">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="34a69-673">String collection</span></span>|<span data-ttu-id="34a69-674">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
</span><span class="sxs-lookup"><span data-stu-id="34a69-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="34a69-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="34a69-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="34a69-676">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="34a69-676">String collection</span></span>|<span data-ttu-id="34a69-677">Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="34a69-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="34a69-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="34a69-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="34a69-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="34a69-680">Wert, der das Verhalten des NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="34a69-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="34a69-681">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="34a69-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="34a69-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="34a69-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="34a69-683">Binär</span><span class="sxs-lookup"><span data-stu-id="34a69-683">Binary</span></span>|<span data-ttu-id="34a69-684">XML-Inhalte mit Details zum Exploit-Schutz.
</span><span class="sxs-lookup"><span data-stu-id="34a69-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="34a69-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="34a69-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="34a69-686">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a69-686">String</span></span>|<span data-ttu-id="34a69-687">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
</span><span class="sxs-lookup"><span data-stu-id="34a69-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="34a69-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="34a69-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="34a69-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-689">Boolean</span></span>|<span data-ttu-id="34a69-690">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="34a69-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="34a69-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="34a69-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="34a69-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="34a69-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="34a69-693">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="34a69-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="34a69-694">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="34a69-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="34a69-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="34a69-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="34a69-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="34a69-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="34a69-697">Anmeldeinformationen Guard aktivieren Sie, wenn Sicherheit Plattformebene mit Secure Boot und Virtualisierung Sicherheit sind beide aktiviert.</span><span class="sxs-lookup"><span data-stu-id="34a69-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="34a69-698">Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="34a69-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="34a69-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="34a69-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="34a69-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-700">Boolean</span></span>|<span data-ttu-id="34a69-701">Schaltet die Virtualisierung basierend Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="34a69-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="34a69-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="34a69-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="34a69-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-703">Boolean</span></span>|<span data-ttu-id="34a69-704">Gibt an, ob Sicherheit Plattformebene beim nächsten Neustart aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="34a69-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="34a69-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="34a69-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="34a69-706">[Aktivierung] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="34a69-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="34a69-707">.MD)</span><span class="sxs-lookup"><span data-stu-id="34a69-707">.md)</span></span>|<span data-ttu-id="34a69-708">Ermöglicht der IT-Administrator die Einführung von Guard System zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="34a69-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="34a69-709">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="34a69-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="34a69-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="34a69-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="34a69-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-711">Boolean</span></span>|<span data-ttu-id="34a69-712">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="34a69-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="34a69-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="34a69-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="34a69-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-714">Boolean</span></span>|<span data-ttu-id="34a69-715">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="34a69-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="34a69-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="34a69-716">applicationGuardEnabled</span></span>|<span data-ttu-id="34a69-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-717">Boolean</span></span>|<span data-ttu-id="34a69-718">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="34a69-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="34a69-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="34a69-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="34a69-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="34a69-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="34a69-721">Aktivieren Sie Windows Defender Anwendung Guard für neuere Versionen von Windows.</span><span class="sxs-lookup"><span data-stu-id="34a69-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="34a69-722">Mögliche Werte: sind `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="34a69-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="34a69-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="34a69-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="34a69-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="34a69-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="34a69-725">Block Zwischenablage Übertragung Bilddatei, Textdatei oder dürfen.</span><span class="sxs-lookup"><span data-stu-id="34a69-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="34a69-726">Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="34a69-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="34a69-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="34a69-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="34a69-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-728">Boolean</span></span>|<span data-ttu-id="34a69-729">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="34a69-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="34a69-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="34a69-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="34a69-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-731">Boolean</span></span>|<span data-ttu-id="34a69-732">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="34a69-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="34a69-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="34a69-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="34a69-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-734">Boolean</span></span>|<span data-ttu-id="34a69-735">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="34a69-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="34a69-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="34a69-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="34a69-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="34a69-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="34a69-738">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="34a69-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="34a69-739">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="34a69-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="34a69-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="34a69-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="34a69-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-741">Boolean</span></span>|<span data-ttu-id="34a69-742">Erlaubt das Drucken im PDF-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="34a69-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="34a69-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="34a69-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="34a69-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-744">Boolean</span></span>|<span data-ttu-id="34a69-745">Erlaubt das Drucken im XPS-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="34a69-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="34a69-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="34a69-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="34a69-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-747">Boolean</span></span>|<span data-ttu-id="34a69-748">Erlaubt das Drucken auf lokalen Druckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="34a69-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="34a69-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="34a69-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="34a69-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-750">Boolean</span></span>|<span data-ttu-id="34a69-751">Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="34a69-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="34a69-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="34a69-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="34a69-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-753">Boolean</span></span>|<span data-ttu-id="34a69-754">Zulassen der Anwendung Guard virtuellen GPU verwenden</span><span class="sxs-lookup"><span data-stu-id="34a69-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="34a69-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="34a69-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="34a69-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-756">Boolean</span></span>|<span data-ttu-id="34a69-757">Zulassen, dass Benutzer Dateien vom Rand im Container Guard Anwendung herunterladen und speichern Sie sie auf dem Host Dateisystem</span><span class="sxs-lookup"><span data-stu-id="34a69-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="34a69-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="34a69-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="34a69-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-759">Boolean</span></span>|<span data-ttu-id="34a69-760">Ermöglicht die Admin standard Benutzer während der Teilnahme von Azure AD Encrpytion aktivieren können.</span><span class="sxs-lookup"><span data-stu-id="34a69-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="34a69-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="34a69-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="34a69-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-762">Boolean</span></span>|<span data-ttu-id="34a69-763">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="34a69-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="34a69-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="34a69-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="34a69-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-765">Boolean</span></span>|<span data-ttu-id="34a69-766">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="34a69-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="34a69-767">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="34a69-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="34a69-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="34a69-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="34a69-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="34a69-769">Boolean</span></span>|<span data-ttu-id="34a69-770">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="34a69-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="34a69-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="34a69-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="34a69-773">System BitLocker Drive-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="34a69-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="34a69-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-774">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="34a69-775">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-775">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="34a69-776">BitLocker feste Laufwerk Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="34a69-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="34a69-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="34a69-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="34a69-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="34a69-779">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="34a69-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="34a69-780">Antwort</span><span class="sxs-lookup"><span data-stu-id="34a69-780">Response</span></span>
<span data-ttu-id="34a69-781">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="34a69-781">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a69-782">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34a69-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a69-783">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34a69-783">Request</span></span>
<span data-ttu-id="34a69-784">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34a69-784">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="34a69-785">Antwort</span><span class="sxs-lookup"><span data-stu-id="34a69-785">Response</span></span>
<span data-ttu-id="34a69-p196">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34a69-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




