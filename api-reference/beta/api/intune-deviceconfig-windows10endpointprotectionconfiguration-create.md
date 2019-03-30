---
title: Erstellen von „windows10EndpointProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1fc2745ffe0a9c3274b23d424401f19f76cc50b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987237"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="3c85a-103">Erstellen von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3c85a-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="3c85a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c85a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c85a-106">Diese Methode erstellt ein neues Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c85a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3c85a-107">Prerequisites</span></span>
<span data-ttu-id="3c85a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c85a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c85a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c85a-110">Permission type</span></span>|<span data-ttu-id="3c85a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c85a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c85a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c85a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c85a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c85a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c85a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c85a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c85a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c85a-115">Not supported.</span></span>|
|<span data-ttu-id="3c85a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c85a-116">Application</span></span>|<span data-ttu-id="3c85a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c85a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c85a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c85a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c85a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c85a-119">Request headers</span></span>
|<span data-ttu-id="3c85a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3c85a-120">Header</span></span>|<span data-ttu-id="3c85a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c85a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c85a-122">Authorization</span></span>|<span data-ttu-id="3c85a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3c85a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c85a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3c85a-124">Accept</span></span>|<span data-ttu-id="3c85a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c85a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c85a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c85a-126">Request body</span></span>
<span data-ttu-id="3c85a-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EndpointProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="3c85a-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="3c85a-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EndpointProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="3c85a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c85a-129">Property</span></span>|<span data-ttu-id="3c85a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3c85a-130">Type</span></span>|<span data-ttu-id="3c85a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c85a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c85a-132">id</span><span class="sxs-lookup"><span data-stu-id="3c85a-132">id</span></span>|<span data-ttu-id="3c85a-133">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-133">String</span></span>|<span data-ttu-id="3c85a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3c85a-134">Key of the entity.</span></span> <span data-ttu-id="3c85a-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c85a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3c85a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c85a-137">DateTimeOffset</span></span>|<span data-ttu-id="3c85a-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3c85a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3c85a-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="3c85a-140">roleScopeTagIds</span></span>|<span data-ttu-id="3c85a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3c85a-141">String collection</span></span>|<span data-ttu-id="3c85a-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="3c85a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3c85a-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3c85a-144">supportsScopeTags</span></span>|<span data-ttu-id="3c85a-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-145">Boolean</span></span>|<span data-ttu-id="3c85a-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3c85a-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="3c85a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3c85a-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3c85a-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-149">This property is read-only.</span></span> <span data-ttu-id="3c85a-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c85a-151">createdDateTime</span></span>|<span data-ttu-id="3c85a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c85a-152">DateTimeOffset</span></span>|<span data-ttu-id="3c85a-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3c85a-153">DateTime the object was created.</span></span> <span data-ttu-id="3c85a-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-155">description</span><span class="sxs-lookup"><span data-stu-id="3c85a-155">description</span></span>|<span data-ttu-id="3c85a-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c85a-156">String</span></span>|<span data-ttu-id="3c85a-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3c85a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c85a-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3c85a-159">displayName</span></span>|<span data-ttu-id="3c85a-160">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-160">String</span></span>|<span data-ttu-id="3c85a-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3c85a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c85a-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-163">Version</span><span class="sxs-lookup"><span data-stu-id="3c85a-163">version</span></span>|<span data-ttu-id="3c85a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3c85a-164">Int32</span></span>|<span data-ttu-id="3c85a-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c85a-165">Version of the device configuration.</span></span> <span data-ttu-id="3c85a-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c85a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c85a-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="3c85a-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="3c85a-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="3c85a-169">Diese Richtlinie soll zusätzliche Sicherheit für externe DMA-fähige Geräte bieten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="3c85a-170">Es ermöglicht eine bessere Kontrolle über die Enumeration externer DMA-Geräte, die mit der DMA-Neuzuordnung/Gerätespeicher Isolierung und Sandkasten nicht kompatibel sind.</span><span class="sxs-lookup"><span data-stu-id="3c85a-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="3c85a-171">Diese Richtlinie wird nur wirksam, wenn der Kernel DMA-Schutz von der System Firmware unterstützt und aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="3c85a-172">Der Kernel DMA Protection ist eine Plattformfunktion, die nicht über Richtlinien oder Endbenutzer gesteuert werden kann.</span><span class="sxs-lookup"><span data-stu-id="3c85a-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="3c85a-173">Sie muss zum Zeitpunkt der Fertigung vom System unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="3c85a-174">Um zu überprüfen, ob das System den Kernel DMA-Schutz unterstützt, aktivieren Sie auf der Zusammenfassungsseite von MSINFO32. exe das Feld Kernel DMA Protection.</span><span class="sxs-lookup"><span data-stu-id="3c85a-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="3c85a-175">Mögliche Werte sind: `deviceDefault`, `blockAll` und `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="3c85a-176">firewallRules</span><span class="sxs-lookup"><span data-stu-id="3c85a-176">firewallRules</span></span>|<span data-ttu-id="3c85a-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="3c85a-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="3c85a-178">Konfiguriert die Firewall-Regeleinstellungen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="3c85a-179">Diese Auflistung kann maximal 150 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="3c85a-180">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="3c85a-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="3c85a-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-182">Dieses Benutzerrecht wird von Credential Manager während der Sicherung/Wiederherstellung verwendet.</span><span class="sxs-lookup"><span data-stu-id="3c85a-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="3c85a-183">Die gespeicherten Anmeldeinformationen der Benutzer werden möglicherweise kompromittiert, wenn diese Berechtigung anderen Entitäten erteilt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="3c85a-184">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-185">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="3c85a-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="3c85a-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-187">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen über das Netzwerk eine Verbindung mit dem Computer herstellen dürfen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="3c85a-188">Der Status Allowed wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="3c85a-189">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="3c85a-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="3c85a-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-191">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen blockieren, eine Verbindung mit dem Computer über das Netzwerk herzustellen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="3c85a-192">Status Block wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-192">State Block is supported.</span></span>|
|<span data-ttu-id="3c85a-193">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3c85a-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="3c85a-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-195">Dieses Benutzerrecht ermöglicht es einem Prozess, einen beliebigen Benutzer ohne Authentifizierung zu imitieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="3c85a-196">Der Prozess kann daher Zugriff auf die gleichen lokalen Ressourcen wie diesen Benutzer erlangen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="3c85a-197">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-198">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="3c85a-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="3c85a-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-200">Dieses Benutzerrecht bestimmt, welche Benutzer sich am Computer anmelden können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="3c85a-201">Status NotConfigured, zulässig und blockiert werden alle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="3c85a-202">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="3c85a-202">userRightsBackupData</span></span>|[<span data-ttu-id="3c85a-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-204">Dieses Benutzerrecht bestimmt, welche Benutzer beim Sichern von Dateien und Verzeichnissen Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="3c85a-205">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-206">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="3c85a-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="3c85a-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-208">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen die Uhrzeit und das Datum für die interne Uhr des Computers ändern können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="3c85a-209">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-210">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="3c85a-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="3c85a-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-212">Diese Sicherheitseinstellung bestimmt, ob Benutzer globale Objekte erstellen können, die für alle Sitzungen zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="3c85a-213">Benutzer, die globale Objekte erstellen können, könnten sich auf Prozesse auswirken, die in Sitzungen anderer Benutzer ausgeführt werden, was zu Anwendungsfehlern oder Datenbeschädigungen führen kann.</span><span class="sxs-lookup"><span data-stu-id="3c85a-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="3c85a-214">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-215">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="3c85a-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="3c85a-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-217">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen eine interne API aufrufen können, um die Größe einer Auslagerungsdatei zu erstellen und zu ändern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="3c85a-218">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-219">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="3c85a-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="3c85a-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-221">Dieses Benutzerrecht bestimmt, welche Konten von Prozessen verwendet werden können, um mithilfe des Objekt-Managers ein Verzeichnisobjekt zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="3c85a-222">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-223">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="3c85a-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="3c85a-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-225">Dieses Benutzerrecht bestimmt, ob der Benutzer einen symbolischen Link von dem Computer aus erstellen kann, auf dem Sie angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="3c85a-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="3c85a-226">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-227">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="3c85a-227">userRightsCreateToken</span></span>|[<span data-ttu-id="3c85a-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-229">Dieses Benutzerrecht bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token zu erstellen, das dann verwendet werden kann, um Zugriff auf lokale Ressourcen zu erhalten, wenn der Prozess eine interne API zum Erstellen eines Zugriffstokens verwendet.</span><span class="sxs-lookup"><span data-stu-id="3c85a-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="3c85a-230">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-231">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="3c85a-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="3c85a-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-233">Dieses Benutzerrecht bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="3c85a-234">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="3c85a-235">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="3c85a-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="3c85a-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-237">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen nicht als Remote Desktop Dienste-Client angemeldet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="3c85a-238">Nur Status NotConfigured und blockiert werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="3c85a-239">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="3c85a-239">userRightsDelegation</span></span>|[<span data-ttu-id="3c85a-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-241">Dieses Benutzerrecht bestimmt, welche Benutzer die Einstellung für die vertrauenswürdige deLegierung für ein Benutzer-oder Computerobjekt festlegen können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="3c85a-242">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-243">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="3c85a-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="3c85a-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-245">Dieses Benutzerrecht bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen zum Sicherheitsprotokoll verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="3c85a-246">Das Sicherheitsprotokoll wird verwendet, um nicht autorisierten Systemzugriff nachzuverfolgen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="3c85a-247">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-248">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="3c85a-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="3c85a-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-250">Durch das Zuweisen dieses Benutzerrechts zu einem Benutzer können Programme, die im Auftrag dieses Benutzers laufen, die Identität eines Clients annehmen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="3c85a-251">Wenn Sie dieses Benutzerrecht für diese Art von Identitätswechsel benötigen, wird verhindert, dass ein nicht autorisierter Benutzer einen Client dazu überzeugt, eine Verbindung mit einem Dienst herzustellen, den er erstellt hat, und dann die Identität dieses Clients annehmen, wodurch die Berechtigungen des nicht autorisierten Benutzers erhöht werden können administrative oder Systemebenen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="3c85a-252">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-253">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="3c85a-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="3c85a-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-255">Dieses Benutzerrecht bestimmt, welche Konten einen Prozess mit Schreibeigenschaften Zugriff auf einen anderen Prozess verwenden können, um die dem anderen Prozess zugewiesene Ausführungspriorität zu verlängern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="3c85a-256">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-257">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="3c85a-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="3c85a-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-259">Dieses Benutzerrecht bestimmt, welche Benutzer Gerätetreiber oder anderen Code im Kernelmodus dynamisch laden und entladen können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="3c85a-260">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-261">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="3c85a-261">userRightsLockMemory</span></span>|[<span data-ttu-id="3c85a-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-263">Dieses Benutzerrecht bestimmt, welche Konten einen Prozess verwenden können, um Daten im physischen Arbeitsspeicher zu speichern, wodurch verhindert wird, dass das System die Daten auf dem Datenträger in den virtuellen Arbeitsspeicher eingibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="3c85a-264">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-265">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="3c85a-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="3c85a-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-267">Dieses Benutzerrecht bestimmt, welche Benutzer die Objektzugriffs-Überwachungsoptionen für einzelne Ressourcen wie Dateien, Active Directory-Objekte und Registrierungsschlüssel angeben können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="3c85a-268">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-269">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="3c85a-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="3c85a-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-271">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen Wartungsaufgaben auf einem Volume ausführen können, beispielsweise die Remote Defragmentierung.</span><span class="sxs-lookup"><span data-stu-id="3c85a-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="3c85a-272">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-273">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="3c85a-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="3c85a-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-275">Dieses Benutzerrecht bestimmt, wer die Werte der Firmware-Umgebung ändern kann.</span><span class="sxs-lookup"><span data-stu-id="3c85a-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="3c85a-276">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-277">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="3c85a-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="3c85a-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-279">Dieses Benutzerrecht bestimmt, welche Benutzerkonten die Integritäts Bezeichnung von Objekten wie Dateien, Registrierungsschlüssel oder Prozesse ändern können, die anderen Benutzern gehören.</span><span class="sxs-lookup"><span data-stu-id="3c85a-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="3c85a-280">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-281">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="3c85a-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="3c85a-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-283">Dieses Benutzerrecht bestimmt, welche Benutzer Leistungsüberwachungstools verwenden können, um die Leistung von Systemprozessen zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="3c85a-284">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-285">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="3c85a-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="3c85a-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-287">Dieses Benutzerrecht bestimmt, welche Benutzer einen Computer von einem Remotestandort im Netzwerk Herunterfahren dürfen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="3c85a-288">Missbrauch dieses Benutzerrechts kann zu einem Denial-of-Service führen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="3c85a-289">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-290">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="3c85a-290">userRightsRestoreData</span></span>|[<span data-ttu-id="3c85a-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-292">Dieses Benutzerrecht bestimmt, welche Benutzer bei der Wiederherstellung gesicherter Dateien und Verzeichnisse Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können, und bestimmt, welche Benutzer einen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können.</span><span class="sxs-lookup"><span data-stu-id="3c85a-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="3c85a-293">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-294">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="3c85a-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="3c85a-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-296">Dieses Benutzerrecht bestimmt, welche Benutzer den Besitz eines sicherungsfähigen Objekts im System übernehmen können, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads.</span><span class="sxs-lookup"><span data-stu-id="3c85a-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="3c85a-297">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="3c85a-298">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="3c85a-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="3c85a-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="3c85a-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="3c85a-300">Diese Sicherheitseinstellung bestimmt, welche Dienstkonten verhindert werden, einen Prozess als Dienst zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="3c85a-301">Hinweis: Diese Sicherheitseinstellung gilt nicht für die System-, lokalen Dienst-oder Netzwerkdienstkonten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="3c85a-302">Nur Status blockiert wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="3c85a-303">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="3c85a-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="3c85a-304">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-304">Boolean</span></span>|<span data-ttu-id="3c85a-305">Diese Einstellung bestimmt, ob Xbox Game Save (1) oder Disabled (0) aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="3c85a-306">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="3c85a-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="3c85a-307">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="3c85a-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="3c85a-308">Diese Einstellung bestimmt, ob der Starttyp des Zubehör Verwaltungsdiensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="3c85a-309">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="3c85a-309">Default: Manual.</span></span> <span data-ttu-id="3c85a-310">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="3c85a-311">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="3c85a-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="3c85a-312">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="3c85a-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="3c85a-313">Diese Einstellung bestimmt, ob der Starttyp des Live auth Manager-Diensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="3c85a-314">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="3c85a-314">Default: Manual.</span></span> <span data-ttu-id="3c85a-315">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="3c85a-316">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="3c85a-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="3c85a-317">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="3c85a-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="3c85a-318">Diese Einstellung bestimmt, ob der Starttyp des Live Spiel-Diensts automatisch ist (2), manuell (3), deaktiviert (4).</span><span class="sxs-lookup"><span data-stu-id="3c85a-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="3c85a-319">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="3c85a-319">Default: Manual.</span></span> <span data-ttu-id="3c85a-320">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="3c85a-321">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="3c85a-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="3c85a-322">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="3c85a-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="3c85a-323">Diese Einstellung bestimmt, ob der Starttyp des Netzwerkdiensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="3c85a-324">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="3c85a-324">Default: Manual.</span></span> <span data-ttu-id="3c85a-325">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="3c85a-326">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="3c85a-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="3c85a-327">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-327">Boolean</span></span>|<span data-ttu-id="3c85a-328">Verhindern, dass Benutzer neue Microsoft-Konten zu diesem Computer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="3c85a-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="3c85a-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="3c85a-330">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-330">Boolean</span></span>|<span data-ttu-id="3c85a-331">Aktivieren Sie lokale Konten, die nicht kennwortgeschützt sind, um sich an anderen Speicherorten als dem physischen Gerät anzumelden. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="3c85a-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="3c85a-332">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="3c85a-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="3c85a-333">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-333">Boolean</span></span>|<span data-ttu-id="3c85a-334">Bestimmt, ob das lokale Administrator Konto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="3c85a-335">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="3c85a-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="3c85a-336">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-336">String</span></span>|<span data-ttu-id="3c85a-337">Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3c85a-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="3c85a-338">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="3c85a-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="3c85a-339">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-339">Boolean</span></span>|<span data-ttu-id="3c85a-340">Bestimmt, ob das Gastkonto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="3c85a-341">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="3c85a-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="3c85a-342">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-342">String</span></span>|<span data-ttu-id="3c85a-343">Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Guest" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3c85a-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="3c85a-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="3c85a-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="3c85a-345">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-345">Boolean</span></span>|<span data-ttu-id="3c85a-346">Verhindern, dass ein tragbarer Computer ohne Anmeldung abdockt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="3c85a-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="3c85a-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="3c85a-348">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-348">Boolean</span></span>|<span data-ttu-id="3c85a-349">Beschränken Sie die Installation von Druckertreibern im Rahmen der Verbindung zu einem freigegebenen Drucker nur mit Administratoren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="3c85a-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="3c85a-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="3c85a-351">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-351">Boolean</span></span>|<span data-ttu-id="3c85a-352">Wenn Sie diese Einstellung aktivieren, kann nur interaktiv auf CD-ROM-Medien zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="3c85a-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="3c85a-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="3c85a-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="3c85a-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="3c85a-355">Legen Sie fest, wer Wechseldatenträger formatieren und Auswerfen darf.</span><span class="sxs-lookup"><span data-stu-id="3c85a-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="3c85a-356">Mögliche Werte sind: `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="3c85a-357">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="3c85a-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="3c85a-358">Int32</span><span class="sxs-lookup"><span data-stu-id="3c85a-358">Int32</span></span>|<span data-ttu-id="3c85a-359">Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="3c85a-360">Gültige Werte 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="3c85a-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="3c85a-361">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="3c85a-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="3c85a-362">Int32</span><span class="sxs-lookup"><span data-stu-id="3c85a-362">Int32</span></span>|<span data-ttu-id="3c85a-363">Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="3c85a-364">Gültige Werte 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="3c85a-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="3c85a-365">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="3c85a-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="3c85a-366">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-366">Boolean</span></span>|<span data-ttu-id="3c85a-367">Die Tastenkombination STRG + ALT + ENTF muss gedrückt werden, bevor sich ein Benutzer anmelden kann.</span><span class="sxs-lookup"><span data-stu-id="3c85a-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="3c85a-368">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="3c85a-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="3c85a-369">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-369">Boolean</span></span>|<span data-ttu-id="3c85a-370">Zeigen Sie nicht den Benutzernamen der letzten Person an, die sich auf diesem Gerät angemeldet hat.</span><span class="sxs-lookup"><span data-stu-id="3c85a-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="3c85a-371">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="3c85a-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="3c85a-372">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-372">Boolean</span></span>|<span data-ttu-id="3c85a-373">Zeigen Sie nicht den Benutzernamen der Person an, die sich bei diesem Gerät anmeldet, nachdem Sie die Anmeldeinformationen eingegeben haben, und bevor der Desktop des Geräts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="3c85a-374">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="3c85a-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="3c85a-375">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-375">String</span></span>|<span data-ttu-id="3c85a-376">Festlegen des Nachrichten Titels für Benutzer, die sich anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="3c85a-377">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="3c85a-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="3c85a-378">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-378">String</span></span>|<span data-ttu-id="3c85a-379">Festlegen des Nachrichtentexts für Benutzer, die sich anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="3c85a-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="3c85a-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="3c85a-381">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-381">Boolean</span></span>|<span data-ttu-id="3c85a-382">Blockieren Sie PKU2U-Authentifizierungsanforderungen für dieses Gerät, um Online Identitäten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="3c85a-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="3c85a-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="3c85a-384">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-384">Boolean</span></span>|<span data-ttu-id="3c85a-385">UI Helper Boolean für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager-Entität</span><span class="sxs-lookup"><span data-stu-id="3c85a-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="3c85a-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="3c85a-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="3c85a-387">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-387">String</span></span>|<span data-ttu-id="3c85a-388">Bearbeiten Sie die standardmäßige Zeichenfolge für die Sicherheitsdeskriptor-Definition, um Benutzern und Gruppen das Ausführen von Remote anrufen für SAM zu erlauben oder zu verweigern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="3c85a-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="3c85a-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="3c85a-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="3c85a-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="3c85a-391">Mit dieser Sicherheitseinstellung kann ein Client die 128-Bit-Verschlüsselung und/oder die NTLMv2-Sitzungssicherheit aushandeln.</span><span class="sxs-lookup"><span data-stu-id="3c85a-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="3c85a-392">Mögliche Werte sind: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="3c85a-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="3c85a-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="3c85a-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="3c85a-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="3c85a-395">Mit dieser Sicherheitseinstellung kann ein Server die Aushandlung der 128-Bit-Verschlüsselung und/oder der NTLMv2-Sitzungssicherheit erfordern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="3c85a-396">Mögliche Werte sind: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption` und `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="3c85a-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="3c85a-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="3c85a-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="3c85a-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="3c85a-399">Diese Sicherheitseinstellung bestimmt, welches Abfrage-/Antwort Authentifizierungsprotokoll für Netzwerkanmeldungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="3c85a-400">Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="3c85a-401">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="3c85a-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="3c85a-402">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-402">Boolean</span></span>|<span data-ttu-id="3c85a-403">Wenn diese Option aktiviert ist, erlaubt der SMB-Client unsichere Gastanmeldungen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="3c85a-404">Wenn nicht konfiguriert, lehnt der SMB-Client unsichere Gastanmeldungen ab.</span><span class="sxs-lookup"><span data-stu-id="3c85a-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="3c85a-405">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="3c85a-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="3c85a-406">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-406">Boolean</span></span>|<span data-ttu-id="3c85a-407">Diese Sicherheitseinstellung bestimmt, ob die Auslagerungsdatei des virtuellen Speichers gelöscht wird, wenn das System heruntergefahren wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="3c85a-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="3c85a-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="3c85a-409">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-409">Boolean</span></span>|<span data-ttu-id="3c85a-410">Diese Sicherheitseinstellung bestimmt, ob ein Computer heruntergefahren werden kann, ohne sich bei Windows anmelden zu müssen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="3c85a-411">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="3c85a-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="3c85a-412">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-412">Boolean</span></span>|<span data-ttu-id="3c85a-413">Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="3c85a-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="3c85a-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="3c85a-415">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-415">Boolean</span></span>|<span data-ttu-id="3c85a-416">Virtualisieren von Datei-und Registrierungs Schreibfehlern pro Benutzerspeicherorte</span><span class="sxs-lookup"><span data-stu-id="3c85a-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="3c85a-417">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="3c85a-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="3c85a-418">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-418">Boolean</span></span>|<span data-ttu-id="3c85a-419">Erzwingen Sie die Validierung des PKI-Zertifizierungspfads für eine bestimmte ausführbare Datei, bevor Sie ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="3c85a-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="3c85a-420">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="3c85a-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="3c85a-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="3c85a-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="3c85a-422">Definieren Sie das Verhalten der Eingabeaufforderung für Administratoren im AdministratorgenehmigungsModus.</span><span class="sxs-lookup"><span data-stu-id="3c85a-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="3c85a-423">Mögliche Werte: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="3c85a-424">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="3c85a-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="3c85a-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="3c85a-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="3c85a-426">Definieren Sie das Verhalten der Eingabeaufforderung für Standardbenutzer.</span><span class="sxs-lookup"><span data-stu-id="3c85a-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="3c85a-427">Mögliche Werte sind: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop` und `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="3c85a-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="3c85a-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="3c85a-429">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-429">Boolean</span></span>|<span data-ttu-id="3c85a-430">Aktivieren Sie alle Elevation-Anforderungen, um anstelle des sicheren Desktops zum Desktop des interaktiven Benutzers zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="3c85a-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="3c85a-431">Richtlinieneinstellungen für das Ansage Verhalten für Administratoren und Standardbenutzer werden verwendet.</span><span class="sxs-lookup"><span data-stu-id="3c85a-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="3c85a-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="3c85a-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="3c85a-433">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-433">Boolean</span></span>|<span data-ttu-id="3c85a-434">App-Installationen, die erhöhte Rechte erfordern, werden zur Eingabe von Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="3c85a-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="3c85a-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="3c85a-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="3c85a-436">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-436">Boolean</span></span>|<span data-ttu-id="3c85a-437">Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="3c85a-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="3c85a-438">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="3c85a-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="3c85a-439">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-439">Boolean</span></span>|<span data-ttu-id="3c85a-440">Definiert, ob das integrierte Administratorkonto den AdministratorgenehmigungsModus verwendet oder alle apps mit vollständigen Administratorrechten ausführt. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="3c85a-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="3c85a-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="3c85a-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="3c85a-442">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-442">Boolean</span></span>|<span data-ttu-id="3c85a-443">Legen Sie fest, ob der AdministratorgenehmigungsModus und alle UAC-Richtlinieneinstellungen aktiviert sind, Standard ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3c85a-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="3c85a-444">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="3c85a-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="3c85a-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="3c85a-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="3c85a-446">Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="3c85a-447">Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="3c85a-448">Mögliche Werte sind: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly` und `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="3c85a-449">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="3c85a-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="3c85a-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="3c85a-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="3c85a-451">Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="3c85a-452">Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="3c85a-453">Mögliche Werte sind: `notConfigured`, `administrators`, `administratorsAndPowerUsers` und `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="3c85a-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="3c85a-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="3c85a-455">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-455">Boolean</span></span>|<span data-ttu-id="3c85a-456">Diese Sicherheitseinstellung bestimmt, ob der SMB-Client versucht, die SMB-Paketsignierung auszuhandeln.</span><span class="sxs-lookup"><span data-stu-id="3c85a-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="3c85a-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="3c85a-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="3c85a-458">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-458">Boolean</span></span>|<span data-ttu-id="3c85a-459">Diese Sicherheitseinstellung bestimmt, ob die Paketsignierung für die SMB-Clientkomponente erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="3c85a-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="3c85a-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="3c85a-461">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-461">Boolean</span></span>|<span data-ttu-id="3c85a-462">Wenn diese Sicherheitseinstellung aktiviert ist, kann der SMB-Redirector (Server Message Block) Klartext-Kennwörter an nicht-Microsoft SMB-Server senden, die die Kennwortverschlüsselung während der Authentifizierung nicht unterstützen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="3c85a-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="3c85a-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="3c85a-464">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-464">Boolean</span></span>|<span data-ttu-id="3c85a-465">Diese Sicherheitseinstellung bestimmt, ob für die SMB-Serverkomponente eine Paketsignierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="3c85a-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="3c85a-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="3c85a-467">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-467">Boolean</span></span>|<span data-ttu-id="3c85a-468">Diese Sicherheitseinstellung bestimmt, ob der SMB-Server die SMB-Paketsignierung mit Clients aushandelt, die ihn anfordern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="3c85a-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="3c85a-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="3c85a-470">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-470">Boolean</span></span>|<span data-ttu-id="3c85a-471">Diese Sicherheitseinstellung beschränkt den anonymen Zugriff auf Freigaben und Pipes standardmäßig auf die Einstellungen für Named Pipes, auf die anonym zugegriffen werden kann, und auf Freigaben, auf die anonym zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="3c85a-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="3c85a-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="3c85a-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="3c85a-473">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-473">Boolean</span></span>|<span data-ttu-id="3c85a-474">Diese Sicherheitseinstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="3c85a-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="3c85a-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="3c85a-476">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-476">Boolean</span></span>|<span data-ttu-id="3c85a-477">Diese Sicherheitseinstellung bestimmt, ob anonyme Benutzer bestimmte Aktivitäten ausführen können, beispielsweise das Aufzählen der Namen von Domänenkonten und Netzwerkfreigaben.</span><span class="sxs-lookup"><span data-stu-id="3c85a-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="3c85a-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="3c85a-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="3c85a-479">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-479">Boolean</span></span>|<span data-ttu-id="3c85a-480">Diese Sicherheitseinstellung bestimmt, ob bei der nächsten Kennwortänderung der LAN-Manager (LM)-Hashwert für das neue Kennwort gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="3c85a-481">Sie wird nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3c85a-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="3c85a-482">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="3c85a-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="3c85a-483">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="3c85a-483">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="3c85a-484">Diese Sicherheitseinstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Lesegerät entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="3c85a-485">Mögliche Werte sind: `lockWorkstation`, `noAction`, `forceLogoff` und `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="3c85a-486">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="3c85a-487">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-487">Boolean</span></span>|<span data-ttu-id="3c85a-488">Wird verwendet, um die Anzeige des App-und Browser Schutzbereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="3c85a-489">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="3c85a-490">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-490">Boolean</span></span>|<span data-ttu-id="3c85a-491">Wird verwendet, um die Anzeige des Bereichs Familienoptionen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="3c85a-492">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="3c85a-493">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-493">Boolean</span></span>|<span data-ttu-id="3c85a-494">Wird verwendet, um die Anzeige der Geräteleistung und des Integritäts Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="3c85a-495">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="3c85a-496">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-496">Boolean</span></span>|<span data-ttu-id="3c85a-497">Wird verwendet, um die Anzeige des Firewall-und Netzwerkschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="3c85a-498">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="3c85a-499">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-499">Boolean</span></span>|<span data-ttu-id="3c85a-500">Wird verwendet, um die Anzeige des Viren-und Bedrohungsschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="3c85a-501">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="3c85a-502">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-502">Boolean</span></span>|<span data-ttu-id="3c85a-503">Wird verwendet, um die Anzeige des Kontoschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="3c85a-504">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="3c85a-505">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-505">Boolean</span></span>|<span data-ttu-id="3c85a-506">Wird verwendet, um die Anzeige der Schaltfläche TPM löschen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="3c85a-507">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="3c85a-508">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-508">Boolean</span></span>|<span data-ttu-id="3c85a-509">Wird verwendet, um die Anzeige des Hardwareschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="3c85a-510">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="3c85a-511">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-511">Boolean</span></span>|<span data-ttu-id="3c85a-512">Wird verwendet, um die Anzeige des Benachrichtigungsbereichs-Steuerelements zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="3c85a-513">Der Benutzer muss sich abmelden und sich anmelden oder den Computer neu starten, damit diese Einstellung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="3c85a-514">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="3c85a-515">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-515">Boolean</span></span>|<span data-ttu-id="3c85a-516">Wird verwendet, um die Anzeige des Ransomware-Schutzbereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="3c85a-517">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="3c85a-518">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-518">Boolean</span></span>|<span data-ttu-id="3c85a-519">Wird verwendet, um die Anzeige des sicheren Startbereichs unter Gerätesicherheit zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="3c85a-520">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="3c85a-521">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-521">Boolean</span></span>|<span data-ttu-id="3c85a-522">Wird verwendet, um die Anzeige der Sicherheitsprozess-Problembehandlung unter Gerätesicherheit zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="3c85a-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="3c85a-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="3c85a-524">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-524">Boolean</span></span>|<span data-ttu-id="3c85a-525">Wird verwendet, um die Anzeige der TPM-Update-Firmware zu deaktivieren, wenn eine Sicherheitsanfälligkeit erkannt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="3c85a-526">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c85a-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="3c85a-527">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-527">String</span></span>|<span data-ttu-id="3c85a-528">Der Name des Unternehmens, der den Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="3c85a-529">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="3c85a-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="3c85a-530">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-530">String</span></span>|<span data-ttu-id="3c85a-531">Die e-Mail-Adresse, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="3c85a-532">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="3c85a-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="3c85a-533">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-533">String</span></span>|<span data-ttu-id="3c85a-534">Die Telefonnummer oder die Skype-ID, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="3c85a-535">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="3c85a-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="3c85a-536">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-536">String</span></span>|<span data-ttu-id="3c85a-537">Die URL des Hilfe Portals, die für Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="3c85a-538">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="3c85a-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="3c85a-539">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="3c85a-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="3c85a-540">Benachrichtigungen, die aus den angezeigten Bereichen der App angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="3c85a-541">Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="3c85a-542">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="3c85a-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="3c85a-543">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="3c85a-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="3c85a-544">Konfigurieren Sie, wo die IT-Kontaktinformationen Endbenutzern angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="3c85a-545">Mögliche Werte sind: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp` und `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="3c85a-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="3c85a-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="3c85a-547">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-547">Boolean</span></span>|<span data-ttu-id="3c85a-548">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="3c85a-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="3c85a-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="3c85a-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="3c85a-550">Int32</span><span class="sxs-lookup"><span data-stu-id="3c85a-550">Int32</span></span>|<span data-ttu-id="3c85a-551">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="3c85a-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="3c85a-552">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="3c85a-553">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="3c85a-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="3c85a-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="3c85a-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="3c85a-555">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="3c85a-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="3c85a-556">Wählen Sie die zu verwendende vorinstallierte Tasten Codierung aus.</span><span class="sxs-lookup"><span data-stu-id="3c85a-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="3c85a-557">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="3c85a-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="3c85a-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="3c85a-559">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-559">Boolean</span></span>|<span data-ttu-id="3c85a-560">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="3c85a-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="3c85a-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="3c85a-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="3c85a-562">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-562">Boolean</span></span>|<span data-ttu-id="3c85a-563">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="3c85a-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="3c85a-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="3c85a-565">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-565">Boolean</span></span>|<span data-ttu-id="3c85a-566">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="3c85a-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="3c85a-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="3c85a-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="3c85a-568">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-568">Boolean</span></span>|<span data-ttu-id="3c85a-569">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="3c85a-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="3c85a-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="3c85a-571">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="3c85a-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="3c85a-572">Geben Sie an, wie die Zertifikatssperrliste erzwungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="3c85a-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="3c85a-573">Mögliche Werte sind: `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="3c85a-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="3c85a-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="3c85a-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c85a-575">Boolean</span></span>|<span data-ttu-id="3c85a-576">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="3c85a-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="3c85a-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="3c85a-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="3c85a-578">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="3c85a-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="3c85a-579">Konfiguriert, wie Paketwarteschlangen im Tunnel Gateway-Szenario angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="3c85a-580">Mögliche Werte: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="3c85a-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="3c85a-581">firewallProfileDomain</span></span>|[<span data-ttu-id="3c85a-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3c85a-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="3c85a-583">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="3c85a-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="3c85a-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="3c85a-584">firewallProfilePublic</span></span>|[<span data-ttu-id="3c85a-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3c85a-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="3c85a-586">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="3c85a-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="3c85a-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="3c85a-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="3c85a-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3c85a-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="3c85a-589">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="3c85a-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="3c85a-590">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="3c85a-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="3c85a-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-592">Wert, der das Verhalten von Adobe Reader beim Erstellen von untergeordneten Prozessen angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="3c85a-593">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="3c85a-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="3c85a-595">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3c85a-595">String collection</span></span>|<span data-ttu-id="3c85a-596">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen</span><span class="sxs-lookup"><span data-stu-id="3c85a-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="3c85a-597">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="3c85a-598">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-599">Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="3c85a-600">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-601">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="3c85a-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="3c85a-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-603">Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="3c85a-604">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-605">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="3c85a-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="3c85a-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-607">Wert, der das Verhalten von Office-Kommunikationsanwendungen, einschließlich Microsoft Outlook, zum Erstellen von untergeordneten Prozessen angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="3c85a-608">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="3c85a-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="3c85a-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-611">Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="3c85a-612">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="3c85a-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="3c85a-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-615">Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten.</span><span class="sxs-lookup"><span data-stu-id="3c85a-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="3c85a-616">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-617">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="3c85a-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="3c85a-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-619">Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse.</span><span class="sxs-lookup"><span data-stu-id="3c85a-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="3c85a-620">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-621">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="3c85a-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="3c85a-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-623">Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse.</span><span class="sxs-lookup"><span data-stu-id="3c85a-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="3c85a-624">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="3c85a-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="3c85a-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-627">Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="3c85a-628">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="3c85a-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="3c85a-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-631">Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="3c85a-632">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-633">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="3c85a-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="3c85a-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-635">Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="3c85a-636">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-637">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="3c85a-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="3c85a-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-639">Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="3c85a-640">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-641">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="3c85a-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-643">Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="3c85a-644">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-645">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="3c85a-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="3c85a-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-647">Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird.</span><span class="sxs-lookup"><span data-stu-id="3c85a-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="3c85a-648">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-649">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="3c85a-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="3c85a-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-651">Wert, der angibt, ob das unter System für die Windows Local Security Authority gestohlen werden darf.</span><span class="sxs-lookup"><span data-stu-id="3c85a-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="3c85a-652">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-653">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="3c85a-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="3c85a-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-655">Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="3c85a-656">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-657">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="3c85a-657">defenderProcessCreation</span></span>|[<span data-ttu-id="3c85a-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-659">Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="3c85a-660">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-661">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="3c85a-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="3c85a-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-663">Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="3c85a-664">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-665">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="3c85a-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="3c85a-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-667">Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="3c85a-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="3c85a-668">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-669">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="3c85a-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="3c85a-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-671">Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="3c85a-672">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-673">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="3c85a-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="3c85a-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-675">Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="3c85a-676">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-677">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="3c85a-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="3c85a-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="3c85a-679">Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="3c85a-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="3c85a-680">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-681">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="3c85a-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="3c85a-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-683">Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="3c85a-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="3c85a-684">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-685">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="3c85a-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-687">Wert, der die Verwendung von erweitertem Schutz gegen ransomeware angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="3c85a-688">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-689">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="3c85a-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="3c85a-690">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="3c85a-691">Wert, der das Verhalten von geschützten Ordnern angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="3c85a-692">Mögliche Werte: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="3c85a-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="3c85a-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="3c85a-694">String collection</span><span class="sxs-lookup"><span data-stu-id="3c85a-694">String collection</span></span>|<span data-ttu-id="3c85a-695">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen</span><span class="sxs-lookup"><span data-stu-id="3c85a-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="3c85a-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="3c85a-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="3c85a-697">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3c85a-697">String collection</span></span>|<span data-ttu-id="3c85a-698">Liste von Ordnerpfaden, die der Liste der geschützter Ordner hinzugefügt werden sollen</span><span class="sxs-lookup"><span data-stu-id="3c85a-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="3c85a-699">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="3c85a-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3c85a-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3c85a-701">Wert, der das Verhalten von NetworkProtection angibt.</span><span class="sxs-lookup"><span data-stu-id="3c85a-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="3c85a-702">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3c85a-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="3c85a-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="3c85a-704">Binär</span><span class="sxs-lookup"><span data-stu-id="3c85a-704">Binary</span></span>|<span data-ttu-id="3c85a-705">XML-Inhalte mit Details zum Exploit-Schutz</span><span class="sxs-lookup"><span data-stu-id="3c85a-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="3c85a-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="3c85a-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="3c85a-707">String</span><span class="sxs-lookup"><span data-stu-id="3c85a-707">String</span></span>|<span data-ttu-id="3c85a-708">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde</span><span class="sxs-lookup"><span data-stu-id="3c85a-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="3c85a-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="3c85a-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="3c85a-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c85a-710">Boolean</span></span>|<span data-ttu-id="3c85a-711">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="3c85a-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="3c85a-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="3c85a-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="3c85a-713">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="3c85a-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="3c85a-714">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="3c85a-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="3c85a-715">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="3c85a-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="3c85a-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="3c85a-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="3c85a-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="3c85a-718">Aktivieren Sie die Aktivierung der Anmeldeinformationen, wenn die Platt Form sicherheitsStufe mit Secure Boot-und Virtualisierungs-basierter Sicherheit aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="3c85a-719">Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="3c85a-720">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="3c85a-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="3c85a-721">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-721">Boolean</span></span>|<span data-ttu-id="3c85a-722">Aktiviert die Virtualisierungs-basierte Sicherheit (VBS).</span><span class="sxs-lookup"><span data-stu-id="3c85a-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="3c85a-723">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="3c85a-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="3c85a-724">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-724">Boolean</span></span>|<span data-ttu-id="3c85a-725">Gibt an, ob die Platt Form sicherheitsStufe beim nächsten Neustart aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3c85a-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="3c85a-726">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="3c85a-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="3c85a-727">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="3c85a-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="3c85a-728">Ermöglicht es dem IT-Administrator, den Start von System Guard zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="3c85a-729">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3c85a-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="3c85a-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="3c85a-731">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-731">Boolean</span></span>|<span data-ttu-id="3c85a-732">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="3c85a-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="3c85a-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="3c85a-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="3c85a-734">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-734">Boolean</span></span>|<span data-ttu-id="3c85a-735">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="3c85a-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="3c85a-736">applicationGuardEnabled</span></span>|<span data-ttu-id="3c85a-737">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-737">Boolean</span></span>|<span data-ttu-id="3c85a-738">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="3c85a-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="3c85a-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="3c85a-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="3c85a-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="3c85a-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="3c85a-741">Aktivieren Sie Windows Defender Application Guard für neuere Windows-Builds.</span><span class="sxs-lookup"><span data-stu-id="3c85a-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="3c85a-742">Mögliche Werte sind: `notConfigured`, `enabledForEdge`, `enabledForOffice` und `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="3c85a-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="3c85a-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="3c85a-744">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="3c85a-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="3c85a-745">Zwischenablage zum Übertragen der Bilddatei, Textdatei oder keiner dieser Dateien blockieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="3c85a-746">Mögliche Werte: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="3c85a-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="3c85a-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="3c85a-748">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-748">Boolean</span></span>|<span data-ttu-id="3c85a-749">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="3c85a-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="3c85a-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="3c85a-751">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-751">Boolean</span></span>|<span data-ttu-id="3c85a-752">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="3c85a-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="3c85a-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="3c85a-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="3c85a-754">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-754">Boolean</span></span>|<span data-ttu-id="3c85a-755">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="3c85a-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="3c85a-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="3c85a-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="3c85a-757">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="3c85a-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="3c85a-758">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="3c85a-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="3c85a-759">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="3c85a-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="3c85a-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="3c85a-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="3c85a-761">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-761">Boolean</span></span>|<span data-ttu-id="3c85a-762">Erlaubt das Drucken im PDF-Format über Container.</span><span class="sxs-lookup"><span data-stu-id="3c85a-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="3c85a-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="3c85a-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="3c85a-764">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-764">Boolean</span></span>|<span data-ttu-id="3c85a-765">Erlaubt das Drucken im XPS-Format über Container.</span><span class="sxs-lookup"><span data-stu-id="3c85a-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="3c85a-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="3c85a-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="3c85a-767">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-767">Boolean</span></span>|<span data-ttu-id="3c85a-768">Erlaubt das Drucken mit lokalen Druckern über Container.</span><span class="sxs-lookup"><span data-stu-id="3c85a-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="3c85a-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="3c85a-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="3c85a-770">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-770">Boolean</span></span>|<span data-ttu-id="3c85a-771">Erlaubt das Drucken mit Netzwerkdruckern über Container.</span><span class="sxs-lookup"><span data-stu-id="3c85a-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="3c85a-772">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="3c85a-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="3c85a-773">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-773">Boolean</span></span>|<span data-ttu-id="3c85a-774">Anwendungsschutz für die Verwendung virtueller GPU zulassen</span><span class="sxs-lookup"><span data-stu-id="3c85a-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="3c85a-775">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="3c85a-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="3c85a-776">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-776">Boolean</span></span>|<span data-ttu-id="3c85a-777">Benutzer können Dateien von Edge im Application Guard-Container herunterladen und im Hostdateisystem speichern.</span><span class="sxs-lookup"><span data-stu-id="3c85a-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="3c85a-778">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="3c85a-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="3c85a-779">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-779">Boolean</span></span>|<span data-ttu-id="3c85a-780">Ermöglicht es dem Administrator, Standardbenutzern das Aktivieren von encrpytion während des Azure AD-Joins zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="3c85a-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="3c85a-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="3c85a-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="3c85a-782">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c85a-782">Boolean</span></span>|<span data-ttu-id="3c85a-783">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c85a-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="3c85a-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="3c85a-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="3c85a-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c85a-785">Boolean</span></span>|<span data-ttu-id="3c85a-786">Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.</span><span class="sxs-lookup"><span data-stu-id="3c85a-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="3c85a-787">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="3c85a-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="3c85a-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="3c85a-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="3c85a-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c85a-789">Boolean</span></span>|<span data-ttu-id="3c85a-790">Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.</span><span class="sxs-lookup"><span data-stu-id="3c85a-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="3c85a-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="3c85a-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="3c85a-793">BitLocker-System Laufwerk Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="3c85a-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="3c85a-794">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-794">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="3c85a-795">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-795">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="3c85a-796">BitLocker-Richtlinie für feste Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="3c85a-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="3c85a-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="3c85a-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3c85a-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="3c85a-799">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="3c85a-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3c85a-800">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c85a-800">Response</span></span>
<span data-ttu-id="3c85a-801">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3c85a-801">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c85a-802">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c85a-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c85a-803">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c85a-803">Request</span></span>
<span data-ttu-id="3c85a-804">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3c85a-804">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3c85a-805">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c85a-805">Response</span></span>
<span data-ttu-id="3c85a-p199">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c85a-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




