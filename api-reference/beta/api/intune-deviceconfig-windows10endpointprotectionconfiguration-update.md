---
title: Aktualisieren von „windows10EndpointProtectionConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa50597f724be41707b0f015d89d9fb051bc9969
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571697"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="cda66-103">Aktualisieren von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="cda66-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="cda66-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cda66-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cda66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda66-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cda66-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cda66-107">Prerequisites</span></span>
<span data-ttu-id="cda66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cda66-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cda66-110">Permission type</span></span>|<span data-ttu-id="cda66-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cda66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cda66-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cda66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cda66-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda66-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cda66-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cda66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cda66-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cda66-115">Not supported.</span></span>|
|<span data-ttu-id="cda66-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cda66-116">Application</span></span>|<span data-ttu-id="cda66-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cda66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cda66-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cda66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cda66-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cda66-119">Request headers</span></span>
|<span data-ttu-id="cda66-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cda66-120">Header</span></span>|<span data-ttu-id="cda66-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cda66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cda66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cda66-122">Authorization</span></span>|<span data-ttu-id="cda66-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cda66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cda66-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cda66-124">Accept</span></span>|<span data-ttu-id="cda66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cda66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cda66-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cda66-126">Request body</span></span>
<span data-ttu-id="cda66-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="cda66-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="cda66-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="cda66-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="cda66-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cda66-129">Property</span></span>|<span data-ttu-id="cda66-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cda66-130">Type</span></span>|<span data-ttu-id="cda66-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cda66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda66-132">id</span><span class="sxs-lookup"><span data-stu-id="cda66-132">id</span></span>|<span data-ttu-id="cda66-133">String</span><span class="sxs-lookup"><span data-stu-id="cda66-133">String</span></span>|<span data-ttu-id="cda66-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cda66-134">Key of the entity.</span></span> <span data-ttu-id="cda66-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cda66-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cda66-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cda66-137">DateTimeOffset</span></span>|<span data-ttu-id="cda66-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cda66-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cda66-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="cda66-140">roleScopeTagIds</span></span>|<span data-ttu-id="cda66-141">String collection</span><span class="sxs-lookup"><span data-stu-id="cda66-141">String collection</span></span>|<span data-ttu-id="cda66-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="cda66-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cda66-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cda66-144">supportsScopeTags</span></span>|<span data-ttu-id="cda66-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-145">Boolean</span></span>|<span data-ttu-id="cda66-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cda66-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="cda66-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cda66-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cda66-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-149">This property is read-only.</span></span> <span data-ttu-id="cda66-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cda66-151">createdDateTime</span></span>|<span data-ttu-id="cda66-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cda66-152">DateTimeOffset</span></span>|<span data-ttu-id="cda66-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cda66-153">DateTime the object was created.</span></span> <span data-ttu-id="cda66-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-155">description</span><span class="sxs-lookup"><span data-stu-id="cda66-155">description</span></span>|<span data-ttu-id="cda66-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cda66-156">String</span></span>|<span data-ttu-id="cda66-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cda66-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cda66-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-159">displayName</span><span class="sxs-lookup"><span data-stu-id="cda66-159">displayName</span></span>|<span data-ttu-id="cda66-160">String</span><span class="sxs-lookup"><span data-stu-id="cda66-160">String</span></span>|<span data-ttu-id="cda66-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cda66-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cda66-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-163">Version</span><span class="sxs-lookup"><span data-stu-id="cda66-163">version</span></span>|<span data-ttu-id="cda66-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cda66-164">Int32</span></span>|<span data-ttu-id="cda66-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="cda66-165">Version of the device configuration.</span></span> <span data-ttu-id="cda66-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cda66-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cda66-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="cda66-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="cda66-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="cda66-169">Diese Richtlinie soll zusätzliche Sicherheit für externe DMA-fähige Geräte bieten.</span><span class="sxs-lookup"><span data-stu-id="cda66-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="cda66-170">Es ermöglicht eine bessere Kontrolle über die Enumeration externer DMA-Geräte, die mit der DMA-Neuzuordnung/Gerätespeicher Isolierung und Sandkasten nicht kompatibel sind.</span><span class="sxs-lookup"><span data-stu-id="cda66-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="cda66-171">Diese Richtlinie wird nur wirksam, wenn der Kernel DMA-Schutz von der System Firmware unterstützt und aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="cda66-172">Der Kernel DMA Protection ist eine Plattformfunktion, die nicht über Richtlinien oder Endbenutzer gesteuert werden kann.</span><span class="sxs-lookup"><span data-stu-id="cda66-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="cda66-173">Sie muss zum Zeitpunkt der Fertigung vom System unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="cda66-174">Um zu überprüfen, ob das System den Kernel DMA-Schutz unterstützt, aktivieren Sie auf der Zusammenfassungsseite von MSINFO32. exe das Feld Kernel DMA Protection.</span><span class="sxs-lookup"><span data-stu-id="cda66-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="cda66-175">Mögliche Werte sind: `deviceDefault`, `blockAll` und `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="cda66-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="cda66-176">firewallRules</span><span class="sxs-lookup"><span data-stu-id="cda66-176">firewallRules</span></span>|<span data-ttu-id="cda66-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="cda66-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="cda66-178">Konfiguriert die Firewall-Regeleinstellungen.</span><span class="sxs-lookup"><span data-stu-id="cda66-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="cda66-179">Diese Auflistung kann maximal 150 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="cda66-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="cda66-180">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="cda66-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="cda66-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-182">Dieses Benutzerrecht wird von Credential Manager während der Sicherung/Wiederherstellung verwendet.</span><span class="sxs-lookup"><span data-stu-id="cda66-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="cda66-183">Die gespeicherten Anmeldeinformationen der Benutzer werden möglicherweise kompromittiert, wenn diese Berechtigung anderen Entitäten erteilt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="cda66-184">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-185">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="cda66-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="cda66-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-187">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen über das Netzwerk eine Verbindung mit dem Computer herstellen dürfen.</span><span class="sxs-lookup"><span data-stu-id="cda66-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="cda66-188">Der Status Allowed wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="cda66-189">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="cda66-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="cda66-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-191">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen blockieren, eine Verbindung mit dem Computer über das Netzwerk herzustellen.</span><span class="sxs-lookup"><span data-stu-id="cda66-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="cda66-192">Status Block wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-192">State Block is supported.</span></span>|
|<span data-ttu-id="cda66-193">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cda66-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="cda66-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-195">Dieses Benutzerrecht ermöglicht es einem Prozess, einen beliebigen Benutzer ohne Authentifizierung zu imitieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="cda66-196">Der Prozess kann daher Zugriff auf die gleichen lokalen Ressourcen wie diesen Benutzer erlangen.</span><span class="sxs-lookup"><span data-stu-id="cda66-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="cda66-197">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-198">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="cda66-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="cda66-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-200">Dieses Benutzerrecht bestimmt, welche Benutzer sich am Computer anmelden können.</span><span class="sxs-lookup"><span data-stu-id="cda66-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="cda66-201">Status NotConfigured, zulässig und blockiert werden alle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="cda66-202">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="cda66-202">userRightsBackupData</span></span>|[<span data-ttu-id="cda66-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-204">Dieses Benutzerrecht bestimmt, welche Benutzer beim Sichern von Dateien und Verzeichnissen Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können.</span><span class="sxs-lookup"><span data-stu-id="cda66-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="cda66-205">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-206">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="cda66-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="cda66-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-208">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen die Uhrzeit und das Datum für die interne Uhr des Computers ändern können.</span><span class="sxs-lookup"><span data-stu-id="cda66-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="cda66-209">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-210">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="cda66-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="cda66-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-212">Diese Sicherheitseinstellung bestimmt, ob Benutzer globale Objekte erstellen können, die für alle Sitzungen zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="cda66-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="cda66-213">Benutzer, die globale Objekte erstellen können, könnten sich auf Prozesse auswirken, die in Sitzungen anderer Benutzer ausgeführt werden, was zu Anwendungsfehlern oder Datenbeschädigungen führen kann.</span><span class="sxs-lookup"><span data-stu-id="cda66-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="cda66-214">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-215">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="cda66-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="cda66-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-217">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen eine interne API aufrufen können, um die Größe einer Auslagerungsdatei zu erstellen und zu ändern.</span><span class="sxs-lookup"><span data-stu-id="cda66-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="cda66-218">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-219">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="cda66-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="cda66-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-221">Dieses Benutzerrecht bestimmt, welche Konten von Prozessen verwendet werden können, um mithilfe des Objekt-Managers ein Verzeichnisobjekt zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="cda66-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="cda66-222">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-223">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="cda66-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="cda66-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-225">Dieses Benutzerrecht bestimmt, ob der Benutzer einen symbolischen Link von dem Computer aus erstellen kann, auf dem Sie angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="cda66-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="cda66-226">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-227">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="cda66-227">userRightsCreateToken</span></span>|[<span data-ttu-id="cda66-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-229">Dieses Benutzerrecht bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token zu erstellen, das dann verwendet werden kann, um Zugriff auf lokale Ressourcen zu erhalten, wenn der Prozess eine interne API zum Erstellen eines Zugriffstokens verwendet.</span><span class="sxs-lookup"><span data-stu-id="cda66-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="cda66-230">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-231">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="cda66-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="cda66-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-233">Dieses Benutzerrecht bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können.</span><span class="sxs-lookup"><span data-stu-id="cda66-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="cda66-234">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="cda66-235">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="cda66-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="cda66-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-237">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen nicht als Remote Desktop Dienste-Client angemeldet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="cda66-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="cda66-238">Nur Status NotConfigured und blockiert werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="cda66-239">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="cda66-239">userRightsDelegation</span></span>|[<span data-ttu-id="cda66-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-241">Dieses Benutzerrecht bestimmt, welche Benutzer die Einstellung für die vertrauenswürdige deLegierung für ein Benutzer-oder Computerobjekt festlegen können.</span><span class="sxs-lookup"><span data-stu-id="cda66-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="cda66-242">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-243">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="cda66-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="cda66-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-245">Dieses Benutzerrecht bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen zum Sicherheitsprotokoll verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="cda66-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="cda66-246">Das Sicherheitsprotokoll wird verwendet, um nicht autorisierten Systemzugriff nachzuverfolgen.</span><span class="sxs-lookup"><span data-stu-id="cda66-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="cda66-247">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-248">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="cda66-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="cda66-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-250">Durch das Zuweisen dieses Benutzerrechts zu einem Benutzer können Programme, die im Auftrag dieses Benutzers laufen, die Identität eines Clients annehmen.</span><span class="sxs-lookup"><span data-stu-id="cda66-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="cda66-251">Wenn Sie dieses Benutzerrecht für diese Art von Identitätswechsel benötigen, wird verhindert, dass ein nicht autorisierter Benutzer einen Client dazu überzeugt, eine Verbindung mit einem Dienst herzustellen, den er erstellt hat, und dann die Identität dieses Clients annehmen, wodurch die Berechtigungen des nicht autorisierten Benutzers erhöht werden können administrative oder Systemebenen.</span><span class="sxs-lookup"><span data-stu-id="cda66-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="cda66-252">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-253">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="cda66-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="cda66-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-255">Dieses Benutzerrecht bestimmt, welche Konten einen Prozess mit Schreibeigenschaften Zugriff auf einen anderen Prozess verwenden können, um die dem anderen Prozess zugewiesene Ausführungspriorität zu verlängern.</span><span class="sxs-lookup"><span data-stu-id="cda66-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="cda66-256">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-257">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="cda66-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="cda66-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-259">Dieses Benutzerrecht bestimmt, welche Benutzer Gerätetreiber oder anderen Code im Kernelmodus dynamisch laden und entladen können.</span><span class="sxs-lookup"><span data-stu-id="cda66-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="cda66-260">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-261">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="cda66-261">userRightsLockMemory</span></span>|[<span data-ttu-id="cda66-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-263">Dieses Benutzerrecht bestimmt, welche Konten einen Prozess verwenden können, um Daten im physischen Arbeitsspeicher zu speichern, wodurch verhindert wird, dass das System die Daten auf dem Datenträger in den virtuellen Arbeitsspeicher eingibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="cda66-264">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-265">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="cda66-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="cda66-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-267">Dieses Benutzerrecht bestimmt, welche Benutzer die Objektzugriffs-Überwachungsoptionen für einzelne Ressourcen wie Dateien, Active Directory-Objekte und Registrierungsschlüssel angeben können.</span><span class="sxs-lookup"><span data-stu-id="cda66-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="cda66-268">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-269">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="cda66-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="cda66-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-271">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen Wartungsaufgaben auf einem Volume ausführen können, beispielsweise die Remote Defragmentierung.</span><span class="sxs-lookup"><span data-stu-id="cda66-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="cda66-272">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-273">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="cda66-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="cda66-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-275">Dieses Benutzerrecht bestimmt, wer die Werte der Firmware-Umgebung ändern kann.</span><span class="sxs-lookup"><span data-stu-id="cda66-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="cda66-276">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-277">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="cda66-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="cda66-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-279">Dieses Benutzerrecht bestimmt, welche Benutzerkonten die Integritäts Bezeichnung von Objekten wie Dateien, Registrierungsschlüssel oder Prozesse ändern können, die anderen Benutzern gehören.</span><span class="sxs-lookup"><span data-stu-id="cda66-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="cda66-280">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-281">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="cda66-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="cda66-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-283">Dieses Benutzerrecht bestimmt, welche Benutzer Leistungsüberwachungstools verwenden können, um die Leistung von Systemprozessen zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="cda66-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="cda66-284">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-285">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="cda66-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="cda66-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-287">Dieses Benutzerrecht bestimmt, welche Benutzer einen Computer von einem Remotestandort im Netzwerk Herunterfahren dürfen.</span><span class="sxs-lookup"><span data-stu-id="cda66-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="cda66-288">Missbrauch dieses Benutzerrechts kann zu einem Denial-of-Service führen.</span><span class="sxs-lookup"><span data-stu-id="cda66-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="cda66-289">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-290">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="cda66-290">userRightsRestoreData</span></span>|[<span data-ttu-id="cda66-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-292">Dieses Benutzerrecht bestimmt, welche Benutzer bei der Wiederherstellung gesicherter Dateien und Verzeichnisse Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können, und bestimmt, welche Benutzer einen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können.</span><span class="sxs-lookup"><span data-stu-id="cda66-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="cda66-293">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-294">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="cda66-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="cda66-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-296">Dieses Benutzerrecht bestimmt, welche Benutzer den Besitz eines sicherungsfähigen Objekts im System übernehmen können, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads.</span><span class="sxs-lookup"><span data-stu-id="cda66-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="cda66-297">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="cda66-298">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="cda66-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="cda66-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="cda66-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="cda66-300">Diese Sicherheitseinstellung bestimmt, welche Dienstkonten verhindert werden, einen Prozess als Dienst zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="cda66-301">Hinweis: Diese Sicherheitseinstellung gilt nicht für die System-, lokalen Dienst-oder Netzwerkdienstkonten.</span><span class="sxs-lookup"><span data-stu-id="cda66-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="cda66-302">Nur Status blockiert wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda66-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="cda66-303">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="cda66-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="cda66-304">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-304">Boolean</span></span>|<span data-ttu-id="cda66-305">Diese Einstellung bestimmt, ob Xbox Game Save (1) oder Disabled (0) aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="cda66-306">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="cda66-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="cda66-307">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="cda66-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="cda66-308">Diese Einstellung bestimmt, ob der Starttyp des Zubehör Verwaltungsdiensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="cda66-309">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="cda66-309">Default: Manual.</span></span> <span data-ttu-id="cda66-310">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cda66-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="cda66-311">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="cda66-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="cda66-312">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="cda66-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="cda66-313">Diese Einstellung bestimmt, ob der Starttyp des Live auth Manager-Diensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="cda66-314">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="cda66-314">Default: Manual.</span></span> <span data-ttu-id="cda66-315">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cda66-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="cda66-316">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="cda66-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="cda66-317">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="cda66-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="cda66-318">Diese Einstellung bestimmt, ob der Starttyp des Live Spiel-Diensts automatisch ist (2), manuell (3), deaktiviert (4).</span><span class="sxs-lookup"><span data-stu-id="cda66-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="cda66-319">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="cda66-319">Default: Manual.</span></span> <span data-ttu-id="cda66-320">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cda66-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="cda66-321">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="cda66-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="cda66-322">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="cda66-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="cda66-323">Diese Einstellung bestimmt, ob der Starttyp des Netzwerkdiensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="cda66-324">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="cda66-324">Default: Manual.</span></span> <span data-ttu-id="cda66-325">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cda66-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="cda66-326">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="cda66-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="cda66-327">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-327">Boolean</span></span>|<span data-ttu-id="cda66-328">Verhindern, dass Benutzer neue Microsoft-Konten zu diesem Computer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="cda66-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="cda66-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="cda66-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="cda66-330">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-330">Boolean</span></span>|<span data-ttu-id="cda66-331">Aktivieren Sie lokale Konten, die nicht kennwortgeschützt sind, um sich an anderen Speicherorten als dem physischen Gerät anzumelden. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="cda66-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="cda66-332">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="cda66-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="cda66-333">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-333">Boolean</span></span>|<span data-ttu-id="cda66-334">Bestimmt, ob das lokale Administrator Konto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="cda66-335">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="cda66-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="cda66-336">String</span><span class="sxs-lookup"><span data-stu-id="cda66-336">String</span></span>|<span data-ttu-id="cda66-337">Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="cda66-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="cda66-338">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="cda66-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="cda66-339">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-339">Boolean</span></span>|<span data-ttu-id="cda66-340">Bestimmt, ob das Gastkonto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="cda66-341">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="cda66-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="cda66-342">String</span><span class="sxs-lookup"><span data-stu-id="cda66-342">String</span></span>|<span data-ttu-id="cda66-343">Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Guest" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="cda66-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="cda66-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="cda66-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="cda66-345">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-345">Boolean</span></span>|<span data-ttu-id="cda66-346">Verhindern, dass ein tragbarer Computer ohne Anmeldung abdockt.</span><span class="sxs-lookup"><span data-stu-id="cda66-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="cda66-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="cda66-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="cda66-348">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-348">Boolean</span></span>|<span data-ttu-id="cda66-349">Beschränken Sie die Installation von Druckertreibern im Rahmen der Verbindung zu einem freigegebenen Drucker nur mit Administratoren.</span><span class="sxs-lookup"><span data-stu-id="cda66-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="cda66-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="cda66-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="cda66-351">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-351">Boolean</span></span>|<span data-ttu-id="cda66-352">Wenn Sie diese Einstellung aktivieren, kann nur interaktiv auf CD-ROM-Medien zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="cda66-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="cda66-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="cda66-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="cda66-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="cda66-355">Legen Sie fest, wer Wechseldatenträger formatieren und Auswerfen darf.</span><span class="sxs-lookup"><span data-stu-id="cda66-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="cda66-356">Mögliche Werte sind: `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="cda66-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="cda66-357">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="cda66-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="cda66-358">Int32</span><span class="sxs-lookup"><span data-stu-id="cda66-358">Int32</span></span>|<span data-ttu-id="cda66-359">Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="cda66-360">Gültige Werte 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="cda66-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="cda66-361">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="cda66-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="cda66-362">Int32</span><span class="sxs-lookup"><span data-stu-id="cda66-362">Int32</span></span>|<span data-ttu-id="cda66-363">Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="cda66-364">Gültige Werte 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="cda66-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="cda66-365">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="cda66-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="cda66-366">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-366">Boolean</span></span>|<span data-ttu-id="cda66-367">Die Tastenkombination STRG + ALT + ENTF muss gedrückt werden, bevor sich ein Benutzer anmelden kann.</span><span class="sxs-lookup"><span data-stu-id="cda66-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="cda66-368">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="cda66-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="cda66-369">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-369">Boolean</span></span>|<span data-ttu-id="cda66-370">Zeigen Sie nicht den Benutzernamen der letzten Person an, die sich auf diesem Gerät angemeldet hat.</span><span class="sxs-lookup"><span data-stu-id="cda66-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="cda66-371">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="cda66-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="cda66-372">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-372">Boolean</span></span>|<span data-ttu-id="cda66-373">Zeigen Sie nicht den Benutzernamen der Person an, die sich bei diesem Gerät anmeldet, nachdem Sie die Anmeldeinformationen eingegeben haben, und bevor der Desktop des Geräts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="cda66-374">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="cda66-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="cda66-375">String</span><span class="sxs-lookup"><span data-stu-id="cda66-375">String</span></span>|<span data-ttu-id="cda66-376">Festlegen des Nachrichten Titels für Benutzer, die sich anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="cda66-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="cda66-377">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="cda66-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="cda66-378">String</span><span class="sxs-lookup"><span data-stu-id="cda66-378">String</span></span>|<span data-ttu-id="cda66-379">Festlegen des Nachrichtentexts für Benutzer, die sich anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="cda66-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="cda66-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="cda66-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="cda66-381">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-381">Boolean</span></span>|<span data-ttu-id="cda66-382">Blockieren Sie PKU2U-Authentifizierungsanforderungen für dieses Gerät, um Online Identitäten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="cda66-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="cda66-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="cda66-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="cda66-384">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-384">Boolean</span></span>|<span data-ttu-id="cda66-385">UI Helper Boolean für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager-Entität</span><span class="sxs-lookup"><span data-stu-id="cda66-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="cda66-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="cda66-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="cda66-387">String</span><span class="sxs-lookup"><span data-stu-id="cda66-387">String</span></span>|<span data-ttu-id="cda66-388">Bearbeiten Sie die standardmäßige Zeichenfolge für die Sicherheitsdeskriptor-Definition, um Benutzern und Gruppen das Ausführen von Remote anrufen für SAM zu erlauben oder zu verweigern.</span><span class="sxs-lookup"><span data-stu-id="cda66-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="cda66-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="cda66-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="cda66-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="cda66-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="cda66-391">Mit dieser Sicherheitseinstellung kann ein Client die 128-Bit-Verschlüsselung und/oder die NTLMv2-Sitzungssicherheit aushandeln.</span><span class="sxs-lookup"><span data-stu-id="cda66-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="cda66-392">Mögliche Werte sind: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="cda66-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="cda66-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="cda66-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="cda66-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="cda66-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="cda66-395">Mit dieser Sicherheitseinstellung kann ein Server die Aushandlung der 128-Bit-Verschlüsselung und/oder der NTLMv2-Sitzungssicherheit erfordern.</span><span class="sxs-lookup"><span data-stu-id="cda66-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="cda66-396">Mögliche Werte sind: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="cda66-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="cda66-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="cda66-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="cda66-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="cda66-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="cda66-399">Diese Sicherheitseinstellung bestimmt, welches Abfrage-/Antwort Authentifizierungsprotokoll für Netzwerkanmeldungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="cda66-400">Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="cda66-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="cda66-401">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="cda66-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="cda66-402">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-402">Boolean</span></span>|<span data-ttu-id="cda66-403">Wenn diese Option aktiviert ist, erlaubt der SMB-Client unsichere Gastanmeldungen.</span><span class="sxs-lookup"><span data-stu-id="cda66-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="cda66-404">Wenn nicht konfiguriert, lehnt der SMB-Client unsichere Gastanmeldungen ab.</span><span class="sxs-lookup"><span data-stu-id="cda66-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="cda66-405">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="cda66-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="cda66-406">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-406">Boolean</span></span>|<span data-ttu-id="cda66-407">Diese Sicherheitseinstellung bestimmt, ob die Auslagerungsdatei des virtuellen Speichers gelöscht wird, wenn das System heruntergefahren wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="cda66-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="cda66-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="cda66-409">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-409">Boolean</span></span>|<span data-ttu-id="cda66-410">Diese Sicherheitseinstellung bestimmt, ob ein Computer heruntergefahren werden kann, ohne sich bei Windows anmelden zu müssen.</span><span class="sxs-lookup"><span data-stu-id="cda66-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="cda66-411">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="cda66-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="cda66-412">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-412">Boolean</span></span>|<span data-ttu-id="cda66-413">Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="cda66-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="cda66-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="cda66-415">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-415">Boolean</span></span>|<span data-ttu-id="cda66-416">Virtualisieren von Datei-und Registrierungs Schreibfehlern pro Benutzerspeicherorte</span><span class="sxs-lookup"><span data-stu-id="cda66-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="cda66-417">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="cda66-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="cda66-418">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-418">Boolean</span></span>|<span data-ttu-id="cda66-419">Erzwingen Sie die Validierung des PKI-Zertifizierungspfads für eine bestimmte ausführbare Datei, bevor Sie ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="cda66-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="cda66-420">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="cda66-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="cda66-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="cda66-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="cda66-422">Definieren Sie das Verhalten der Eingabeaufforderung für Administratoren im AdministratorgenehmigungsModus.</span><span class="sxs-lookup"><span data-stu-id="cda66-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="cda66-423">Mögliche Werte: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="cda66-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="cda66-424">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="cda66-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="cda66-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="cda66-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="cda66-426">Definieren Sie das Verhalten der Eingabeaufforderung für Standardbenutzer.</span><span class="sxs-lookup"><span data-stu-id="cda66-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="cda66-427">Mögliche Werte sind: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="cda66-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="cda66-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="cda66-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="cda66-429">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-429">Boolean</span></span>|<span data-ttu-id="cda66-430">Aktivieren Sie alle Elevation-Anforderungen, um anstelle des sicheren Desktops zum Desktop des interaktiven Benutzers zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="cda66-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="cda66-431">Richtlinieneinstellungen für das Ansage Verhalten für Administratoren und Standardbenutzer werden verwendet.</span><span class="sxs-lookup"><span data-stu-id="cda66-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="cda66-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="cda66-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="cda66-433">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-433">Boolean</span></span>|<span data-ttu-id="cda66-434">App-Installationen, die erhöhte Rechte erfordern, werden zur Eingabe von Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="cda66-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="cda66-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="cda66-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="cda66-436">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-436">Boolean</span></span>|<span data-ttu-id="cda66-437">Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="cda66-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="cda66-438">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="cda66-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="cda66-439">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-439">Boolean</span></span>|<span data-ttu-id="cda66-440">Definiert, ob das integrierte Administratorkonto den AdministratorgenehmigungsModus verwendet oder alle apps mit vollständigen Administratorrechten ausführt. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="cda66-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="cda66-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="cda66-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="cda66-442">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-442">Boolean</span></span>|<span data-ttu-id="cda66-443">Legen Sie fest, ob der AdministratorgenehmigungsModus und alle UAC-Richtlinieneinstellungen aktiviert sind, Standard ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="cda66-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="cda66-444">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="cda66-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="cda66-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="cda66-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="cda66-446">Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="cda66-447">Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cda66-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="cda66-448">Mögliche Werte sind: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="cda66-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="cda66-449">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="cda66-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="cda66-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="cda66-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="cda66-451">Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="cda66-452">Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cda66-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="cda66-453">Mögliche Werte sind: `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="cda66-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="cda66-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="cda66-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="cda66-455">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-455">Boolean</span></span>|<span data-ttu-id="cda66-456">Diese Sicherheitseinstellung bestimmt, ob der SMB-Client versucht, die SMB-Paketsignierung auszuhandeln.</span><span class="sxs-lookup"><span data-stu-id="cda66-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="cda66-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="cda66-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="cda66-458">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-458">Boolean</span></span>|<span data-ttu-id="cda66-459">Diese Sicherheitseinstellung bestimmt, ob die Paketsignierung für die SMB-Clientkomponente erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="cda66-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="cda66-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="cda66-461">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-461">Boolean</span></span>|<span data-ttu-id="cda66-462">Wenn diese Sicherheitseinstellung aktiviert ist, kann der SMB-Redirector (Server Message Block) Klartext-Kennwörter an nicht-Microsoft SMB-Server senden, die die Kennwortverschlüsselung während der Authentifizierung nicht unterstützen.</span><span class="sxs-lookup"><span data-stu-id="cda66-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="cda66-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="cda66-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="cda66-464">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-464">Boolean</span></span>|<span data-ttu-id="cda66-465">Diese Sicherheitseinstellung bestimmt, ob für die SMB-Serverkomponente eine Paketsignierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="cda66-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="cda66-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="cda66-467">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-467">Boolean</span></span>|<span data-ttu-id="cda66-468">Diese Sicherheitseinstellung bestimmt, ob der SMB-Server die SMB-Paketsignierung mit Clients aushandelt, die ihn anfordern.</span><span class="sxs-lookup"><span data-stu-id="cda66-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="cda66-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="cda66-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="cda66-470">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-470">Boolean</span></span>|<span data-ttu-id="cda66-471">Diese Sicherheitseinstellung beschränkt den anonymen Zugriff auf Freigaben und Pipes standardmäßig auf die Einstellungen für Named Pipes, auf die anonym zugegriffen werden kann, und auf Freigaben, auf die anonym zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="cda66-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="cda66-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="cda66-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="cda66-473">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-473">Boolean</span></span>|<span data-ttu-id="cda66-474">Diese Sicherheitseinstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="cda66-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="cda66-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="cda66-476">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-476">Boolean</span></span>|<span data-ttu-id="cda66-477">Diese Sicherheitseinstellung bestimmt, ob anonyme Benutzer bestimmte Aktivitäten ausführen können, beispielsweise das Aufzählen der Namen von Domänenkonten und Netzwerkfreigaben.</span><span class="sxs-lookup"><span data-stu-id="cda66-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="cda66-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="cda66-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="cda66-479">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-479">Boolean</span></span>|<span data-ttu-id="cda66-480">Diese Sicherheitseinstellung bestimmt, ob bei der nächsten Kennwortänderung der LAN-Manager (LM)-Hashwert für das neue Kennwort gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="cda66-481">Sie wird nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="cda66-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="cda66-482">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="cda66-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="cda66-483">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="cda66-483">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="cda66-484">Diese Sicherheitseinstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Lesegerät entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="cda66-485">Mögliche Werte sind: `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="cda66-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="cda66-486">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="cda66-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="cda66-487">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-487">Boolean</span></span>|<span data-ttu-id="cda66-488">Wird verwendet, um die Anzeige des App-und Browser Schutzbereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="cda66-489">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="cda66-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="cda66-490">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-490">Boolean</span></span>|<span data-ttu-id="cda66-491">Wird verwendet, um die Anzeige des Bereichs Familienoptionen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="cda66-492">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="cda66-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="cda66-493">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-493">Boolean</span></span>|<span data-ttu-id="cda66-494">Wird verwendet, um die Anzeige der Geräteleistung und des Integritäts Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="cda66-495">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="cda66-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="cda66-496">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-496">Boolean</span></span>|<span data-ttu-id="cda66-497">Wird verwendet, um die Anzeige des Firewall-und Netzwerkschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="cda66-498">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="cda66-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="cda66-499">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-499">Boolean</span></span>|<span data-ttu-id="cda66-500">Wird verwendet, um die Anzeige des Viren-und Bedrohungsschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="cda66-501">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="cda66-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="cda66-502">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-502">Boolean</span></span>|<span data-ttu-id="cda66-503">Wird verwendet, um die Anzeige des Kontoschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="cda66-504">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="cda66-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="cda66-505">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-505">Boolean</span></span>|<span data-ttu-id="cda66-506">Wird verwendet, um die Anzeige der Schaltfläche TPM löschen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="cda66-507">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="cda66-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="cda66-508">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-508">Boolean</span></span>|<span data-ttu-id="cda66-509">Wird verwendet, um die Anzeige des Hardwareschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="cda66-510">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="cda66-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="cda66-511">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-511">Boolean</span></span>|<span data-ttu-id="cda66-512">Wird verwendet, um die Anzeige des Benachrichtigungsbereichs-Steuerelements zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="cda66-513">Der Benutzer muss sich abmelden und sich anmelden oder den Computer neu starten, damit diese Einstellung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="cda66-514">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="cda66-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="cda66-515">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-515">Boolean</span></span>|<span data-ttu-id="cda66-516">Wird verwendet, um die Anzeige des Ransomware-Schutzbereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="cda66-517">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="cda66-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="cda66-518">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-518">Boolean</span></span>|<span data-ttu-id="cda66-519">Wird verwendet, um die Anzeige des sicheren Startbereichs unter Gerätesicherheit zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="cda66-520">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="cda66-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="cda66-521">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-521">Boolean</span></span>|<span data-ttu-id="cda66-522">Wird verwendet, um die Anzeige der Sicherheitsprozess-Problembehandlung unter Gerätesicherheit zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="cda66-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="cda66-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="cda66-524">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-524">Boolean</span></span>|<span data-ttu-id="cda66-525">Wird verwendet, um die Anzeige der TPM-Update-Firmware zu deaktivieren, wenn eine Sicherheitsanfälligkeit erkannt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="cda66-526">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="cda66-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="cda66-527">String</span><span class="sxs-lookup"><span data-stu-id="cda66-527">String</span></span>|<span data-ttu-id="cda66-528">Der Name des Unternehmens, der den Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="cda66-529">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="cda66-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="cda66-530">String</span><span class="sxs-lookup"><span data-stu-id="cda66-530">String</span></span>|<span data-ttu-id="cda66-531">Die e-Mail-Adresse, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="cda66-532">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="cda66-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="cda66-533">String</span><span class="sxs-lookup"><span data-stu-id="cda66-533">String</span></span>|<span data-ttu-id="cda66-534">Die Telefonnummer oder die Skype-ID, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="cda66-535">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="cda66-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="cda66-536">String</span><span class="sxs-lookup"><span data-stu-id="cda66-536">String</span></span>|<span data-ttu-id="cda66-537">Die URL des Hilfe Portals, die für Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="cda66-538">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="cda66-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="cda66-539">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="cda66-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="cda66-540">Benachrichtigungen, die aus den angezeigten Bereichen der App angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cda66-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="cda66-541">Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="cda66-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="cda66-542">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="cda66-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="cda66-543">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="cda66-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="cda66-544">Konfigurieren Sie, wo die IT-Kontaktinformationen Endbenutzern angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cda66-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="cda66-545">Mögliche Werte sind: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="cda66-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="cda66-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="cda66-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="cda66-547">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-547">Boolean</span></span>|<span data-ttu-id="cda66-548">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="cda66-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="cda66-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="cda66-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="cda66-550">Int32</span><span class="sxs-lookup"><span data-stu-id="cda66-550">Int32</span></span>|<span data-ttu-id="cda66-551">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="cda66-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="cda66-552">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="cda66-553">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="cda66-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="cda66-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="cda66-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="cda66-555">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="cda66-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="cda66-556">Wählen Sie die zu verwendende vorinstallierte Tasten Codierung aus.</span><span class="sxs-lookup"><span data-stu-id="cda66-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="cda66-557">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="cda66-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="cda66-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="cda66-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="cda66-559">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-559">Boolean</span></span>|<span data-ttu-id="cda66-560">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="cda66-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="cda66-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="cda66-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="cda66-562">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-562">Boolean</span></span>|<span data-ttu-id="cda66-563">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="cda66-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="cda66-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="cda66-565">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-565">Boolean</span></span>|<span data-ttu-id="cda66-566">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="cda66-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="cda66-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="cda66-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="cda66-568">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-568">Boolean</span></span>|<span data-ttu-id="cda66-569">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="cda66-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="cda66-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="cda66-571">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="cda66-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="cda66-572">Geben Sie an, wie die Zertifikatssperrliste erzwungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="cda66-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="cda66-573">Mögliche Werte sind: `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="cda66-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="cda66-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="cda66-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="cda66-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="cda66-575">Boolean</span></span>|<span data-ttu-id="cda66-576">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="cda66-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="cda66-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="cda66-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="cda66-578">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="cda66-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="cda66-579">Konfiguriert, wie Paketwarteschlangen im Tunnel Gateway-Szenario angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cda66-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="cda66-580">Mögliche Werte: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="cda66-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="cda66-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="cda66-581">firewallProfileDomain</span></span>|[<span data-ttu-id="cda66-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cda66-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="cda66-583">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="cda66-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="cda66-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="cda66-584">firewallProfilePublic</span></span>|[<span data-ttu-id="cda66-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cda66-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="cda66-586">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="cda66-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="cda66-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="cda66-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="cda66-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cda66-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="cda66-589">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="cda66-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="cda66-590">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="cda66-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="cda66-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-592">Wert, der das Verhalten von Adobe Reader beim Erstellen von untergeordneten Prozessen angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="cda66-593">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="cda66-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="cda66-595">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cda66-595">String collection</span></span>|<span data-ttu-id="cda66-596">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen</span><span class="sxs-lookup"><span data-stu-id="cda66-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="cda66-597">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="cda66-598">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-599">Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="cda66-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="cda66-600">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-601">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="cda66-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="cda66-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-603">Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="cda66-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="cda66-604">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-605">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="cda66-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="cda66-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-607">Wert, der das Verhalten von Office-Kommunikationsanwendungen, einschließlich Microsoft Outlook, zum Erstellen von untergeordneten Prozessen angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="cda66-608">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="cda66-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="cda66-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-611">Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten.</span><span class="sxs-lookup"><span data-stu-id="cda66-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="cda66-612">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="cda66-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="cda66-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-615">Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten.</span><span class="sxs-lookup"><span data-stu-id="cda66-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="cda66-616">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-617">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="cda66-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="cda66-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-619">Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse.</span><span class="sxs-lookup"><span data-stu-id="cda66-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="cda66-620">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-621">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="cda66-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="cda66-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-623">Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse.</span><span class="sxs-lookup"><span data-stu-id="cda66-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="cda66-624">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="cda66-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="cda66-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-627">Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="cda66-628">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="cda66-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="cda66-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-631">Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="cda66-632">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-633">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="cda66-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="cda66-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-635">Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="cda66-636">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-637">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="cda66-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="cda66-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-639">Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="cda66-640">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-641">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="cda66-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="cda66-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-643">Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="cda66-644">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-645">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="cda66-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="cda66-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-647">Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird.</span><span class="sxs-lookup"><span data-stu-id="cda66-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="cda66-648">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-649">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="cda66-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="cda66-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-651">Wert, der angibt, ob das unter System für die Windows Local Security Authority gestohlen werden darf.</span><span class="sxs-lookup"><span data-stu-id="cda66-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="cda66-652">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-653">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="cda66-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="cda66-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-655">Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="cda66-656">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-657">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="cda66-657">defenderProcessCreation</span></span>|[<span data-ttu-id="cda66-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-659">Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="cda66-660">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-661">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="cda66-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="cda66-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-663">Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="cda66-664">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-665">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="cda66-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="cda66-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-667">Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="cda66-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="cda66-668">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-669">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="cda66-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="cda66-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-671">Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen.</span><span class="sxs-lookup"><span data-stu-id="cda66-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="cda66-672">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-673">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="cda66-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="cda66-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-675">Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen.</span><span class="sxs-lookup"><span data-stu-id="cda66-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="cda66-676">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-677">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="cda66-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="cda66-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="cda66-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="cda66-679">Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="cda66-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="cda66-680">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-681">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="cda66-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="cda66-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-683">Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="cda66-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="cda66-684">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-685">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="cda66-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-687">Wert, der die Verwendung von erweitertem Schutz gegen ransomeware angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="cda66-688">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-689">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="cda66-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="cda66-690">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="cda66-691">Wert, der das Verhalten von geschützten Ordnern angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="cda66-692">Mögliche Werte: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="cda66-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="cda66-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="cda66-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="cda66-694">String collection</span><span class="sxs-lookup"><span data-stu-id="cda66-694">String collection</span></span>|<span data-ttu-id="cda66-695">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen</span><span class="sxs-lookup"><span data-stu-id="cda66-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="cda66-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="cda66-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="cda66-697">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cda66-697">String collection</span></span>|<span data-ttu-id="cda66-698">Liste von Ordnerpfaden, die der Liste der geschützter Ordner hinzugefügt werden sollen</span><span class="sxs-lookup"><span data-stu-id="cda66-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="cda66-699">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="cda66-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="cda66-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="cda66-701">Wert, der das Verhalten von NetworkProtection angibt.</span><span class="sxs-lookup"><span data-stu-id="cda66-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="cda66-702">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="cda66-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="cda66-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="cda66-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="cda66-704">Binär</span><span class="sxs-lookup"><span data-stu-id="cda66-704">Binary</span></span>|<span data-ttu-id="cda66-705">XML-Inhalte mit Details zum Exploit-Schutz</span><span class="sxs-lookup"><span data-stu-id="cda66-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="cda66-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="cda66-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="cda66-707">String</span><span class="sxs-lookup"><span data-stu-id="cda66-707">String</span></span>|<span data-ttu-id="cda66-708">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde</span><span class="sxs-lookup"><span data-stu-id="cda66-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="cda66-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="cda66-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="cda66-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="cda66-710">Boolean</span></span>|<span data-ttu-id="cda66-711">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="cda66-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="cda66-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="cda66-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="cda66-713">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="cda66-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="cda66-714">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="cda66-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="cda66-715">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="cda66-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="cda66-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="cda66-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="cda66-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="cda66-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="cda66-718">Aktivieren Sie die Aktivierung der Anmeldeinformationen, wenn die Platt Form sicherheitsStufe mit Secure Boot-und Virtualisierungs-basierter Sicherheit aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="cda66-719">Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="cda66-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="cda66-720">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="cda66-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="cda66-721">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-721">Boolean</span></span>|<span data-ttu-id="cda66-722">Aktiviert die Virtualisierungs-basierte Sicherheit (VBS).</span><span class="sxs-lookup"><span data-stu-id="cda66-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="cda66-723">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="cda66-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="cda66-724">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-724">Boolean</span></span>|<span data-ttu-id="cda66-725">Gibt an, ob die Platt Form sicherheitsStufe beim nächsten Neustart aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="cda66-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="cda66-726">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="cda66-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="cda66-727">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="cda66-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cda66-728">Ermöglicht es dem IT-Administrator, den Start von System Guard zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="cda66-729">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cda66-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cda66-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="cda66-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="cda66-731">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-731">Boolean</span></span>|<span data-ttu-id="cda66-732">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="cda66-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="cda66-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="cda66-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="cda66-734">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-734">Boolean</span></span>|<span data-ttu-id="cda66-735">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="cda66-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="cda66-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="cda66-736">applicationGuardEnabled</span></span>|<span data-ttu-id="cda66-737">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-737">Boolean</span></span>|<span data-ttu-id="cda66-738">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="cda66-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="cda66-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="cda66-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="cda66-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="cda66-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="cda66-741">Aktivieren Sie Windows Defender Application Guard für neuere Windows-Builds.</span><span class="sxs-lookup"><span data-stu-id="cda66-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="cda66-742">Mögliche Werte sind: `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="cda66-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="cda66-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="cda66-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="cda66-744">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="cda66-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="cda66-745">Zwischenablage zum Übertragen der Bilddatei, Textdatei oder keiner dieser Dateien blockieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="cda66-746">Mögliche Werte: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="cda66-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="cda66-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="cda66-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="cda66-748">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-748">Boolean</span></span>|<span data-ttu-id="cda66-749">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="cda66-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="cda66-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="cda66-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="cda66-751">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-751">Boolean</span></span>|<span data-ttu-id="cda66-752">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="cda66-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="cda66-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="cda66-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="cda66-754">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-754">Boolean</span></span>|<span data-ttu-id="cda66-755">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="cda66-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="cda66-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="cda66-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="cda66-757">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="cda66-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="cda66-758">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="cda66-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="cda66-759">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="cda66-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="cda66-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="cda66-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="cda66-761">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-761">Boolean</span></span>|<span data-ttu-id="cda66-762">Erlaubt das Drucken im PDF-Format über Container.</span><span class="sxs-lookup"><span data-stu-id="cda66-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="cda66-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="cda66-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="cda66-764">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-764">Boolean</span></span>|<span data-ttu-id="cda66-765">Erlaubt das Drucken im XPS-Format über Container.</span><span class="sxs-lookup"><span data-stu-id="cda66-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="cda66-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="cda66-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="cda66-767">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-767">Boolean</span></span>|<span data-ttu-id="cda66-768">Erlaubt das Drucken mit lokalen Druckern über Container.</span><span class="sxs-lookup"><span data-stu-id="cda66-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="cda66-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="cda66-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="cda66-770">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-770">Boolean</span></span>|<span data-ttu-id="cda66-771">Erlaubt das Drucken mit Netzwerkdruckern über Container.</span><span class="sxs-lookup"><span data-stu-id="cda66-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="cda66-772">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="cda66-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="cda66-773">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-773">Boolean</span></span>|<span data-ttu-id="cda66-774">Anwendungsschutz für die Verwendung virtueller GPU zulassen</span><span class="sxs-lookup"><span data-stu-id="cda66-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="cda66-775">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="cda66-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="cda66-776">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-776">Boolean</span></span>|<span data-ttu-id="cda66-777">Benutzer können Dateien von Edge im Application Guard-Container herunterladen und im Hostdateisystem speichern.</span><span class="sxs-lookup"><span data-stu-id="cda66-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="cda66-778">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="cda66-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="cda66-779">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-779">Boolean</span></span>|<span data-ttu-id="cda66-780">Ermöglicht es dem Administrator, Standardbenutzern das Aktivieren von encrpytion während des Azure AD-Joins zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="cda66-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="cda66-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="cda66-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="cda66-782">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cda66-782">Boolean</span></span>|<span data-ttu-id="cda66-783">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="cda66-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="cda66-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="cda66-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="cda66-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="cda66-785">Boolean</span></span>|<span data-ttu-id="cda66-786">Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.</span><span class="sxs-lookup"><span data-stu-id="cda66-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="cda66-787">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="cda66-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="cda66-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="cda66-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="cda66-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="cda66-789">Boolean</span></span>|<span data-ttu-id="cda66-790">Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.</span><span class="sxs-lookup"><span data-stu-id="cda66-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="cda66-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="cda66-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="cda66-793">BitLocker-System Laufwerk Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="cda66-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="cda66-794">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-794">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="cda66-795">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-795">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="cda66-796">BitLocker-Richtlinie für feste Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="cda66-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="cda66-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="cda66-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="cda66-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="cda66-799">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="cda66-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="cda66-800">Antwort</span><span class="sxs-lookup"><span data-stu-id="cda66-800">Response</span></span>
<span data-ttu-id="cda66-801">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cda66-801">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cda66-802">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cda66-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="cda66-803">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cda66-803">Request</span></span>
<span data-ttu-id="cda66-804">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cda66-804">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 27641

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
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
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
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
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
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
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

### <a name="response"></a><span data-ttu-id="cda66-805">Antwort</span><span class="sxs-lookup"><span data-stu-id="cda66-805">Response</span></span>
<span data-ttu-id="cda66-p199">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cda66-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 27813

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
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
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
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
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
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
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




