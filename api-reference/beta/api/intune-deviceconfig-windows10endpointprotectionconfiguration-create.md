---
title: Erstellen von „windows10EndpointProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8330a5bbce36d486d579a87b762d962a5fab2118
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140236"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="5f12f-103">Erstellen von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5f12f-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="5f12f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f12f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f12f-106">Diese Methode erstellt ein neues Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f12f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-107">Prerequisites</span></span>
<span data-ttu-id="5f12f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f12f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f12f-110">Permission type</span></span>|<span data-ttu-id="5f12f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f12f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f12f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f12f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f12f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f12f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f12f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f12f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f12f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f12f-115">Not supported.</span></span>|
|<span data-ttu-id="5f12f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f12f-116">Application</span></span>|<span data-ttu-id="5f12f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f12f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f12f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f12f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5f12f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f12f-119">Request headers</span></span>
|<span data-ttu-id="5f12f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5f12f-120">Header</span></span>|<span data-ttu-id="5f12f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5f12f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f12f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f12f-122">Authorization</span></span>|<span data-ttu-id="5f12f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f12f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f12f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f12f-124">Accept</span></span>|<span data-ttu-id="5f12f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f12f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f12f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f12f-126">Request body</span></span>
<span data-ttu-id="5f12f-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EndpointProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="5f12f-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="5f12f-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EndpointProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="5f12f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f12f-129">Property</span></span>|<span data-ttu-id="5f12f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5f12f-130">Type</span></span>|<span data-ttu-id="5f12f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f12f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f12f-132">id</span><span class="sxs-lookup"><span data-stu-id="5f12f-132">id</span></span>|<span data-ttu-id="5f12f-133">string</span><span class="sxs-lookup"><span data-stu-id="5f12f-133">String</span></span>|<span data-ttu-id="5f12f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5f12f-134">Key of the entity.</span></span> <span data-ttu-id="5f12f-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f12f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5f12f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f12f-137">DateTimeOffset</span></span>|<span data-ttu-id="5f12f-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f12f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5f12f-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="5f12f-140">roleScopeTagIds</span></span>|<span data-ttu-id="5f12f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5f12f-141">String collection</span></span>|<span data-ttu-id="5f12f-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="5f12f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5f12f-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5f12f-144">supportsScopeTags</span></span>|<span data-ttu-id="5f12f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-145">Boolean</span></span>|<span data-ttu-id="5f12f-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5f12f-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5f12f-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5f12f-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-149">This property is read-only.</span></span> <span data-ttu-id="5f12f-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f12f-151">createdDateTime</span></span>|<span data-ttu-id="5f12f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f12f-152">DateTimeOffset</span></span>|<span data-ttu-id="5f12f-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f12f-153">DateTime the object was created.</span></span> <span data-ttu-id="5f12f-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-155">description</span><span class="sxs-lookup"><span data-stu-id="5f12f-155">description</span></span>|<span data-ttu-id="5f12f-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-156">String</span></span>|<span data-ttu-id="5f12f-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5f12f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f12f-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5f12f-159">displayName</span></span>|<span data-ttu-id="5f12f-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-160">String</span></span>|<span data-ttu-id="5f12f-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5f12f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f12f-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-163">Version</span><span class="sxs-lookup"><span data-stu-id="5f12f-163">version</span></span>|<span data-ttu-id="5f12f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5f12f-164">Int32</span></span>|<span data-ttu-id="5f12f-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f12f-165">Version of the device configuration.</span></span> <span data-ttu-id="5f12f-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f12f-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="5f12f-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="5f12f-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="5f12f-169">Diese Richtlinie soll zusätzliche Sicherheit für externe DMA-fähige Geräte bieten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="5f12f-170">Es ermöglicht eine bessere Kontrolle über die Enumeration externer DMA-Geräte, die mit der DMA-Neuzuordnung/Gerätespeicher Isolierung und Sandkasten nicht kompatibel sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="5f12f-171">Diese Richtlinie wird nur wirksam, wenn der Kernel DMA-Schutz von der System Firmware unterstützt und aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="5f12f-172">Der Kernel DMA Protection ist eine Plattformfunktion, die nicht über Richtlinien oder Endbenutzer gesteuert werden kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="5f12f-173">Sie muss zum Zeitpunkt der Fertigung vom System unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="5f12f-174">Um zu überprüfen, ob das System den Kernel DMA-Schutz unterstützt, aktivieren Sie auf der Zusammenfassungsseite von MSINFO32. exe das Feld Kernel DMA Protection.</span><span class="sxs-lookup"><span data-stu-id="5f12f-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="5f12f-175">Mögliche Werte sind: `deviceDefault`, `blockAll` und `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="5f12f-176">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="5f12f-176">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="5f12f-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-178">Dieses Benutzerrecht wird von Credential Manager während der Sicherung/Wiederherstellung verwendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-178">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="5f12f-179">Die gespeicherten Anmeldeinformationen der Benutzer werden möglicherweise kompromittiert, wenn diese Berechtigung anderen Entitäten erteilt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-179">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="5f12f-180">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-180">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-181">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="5f12f-181">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="5f12f-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-183">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen über das Netzwerk eine Verbindung mit dem Computer herstellen dürfen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-183">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="5f12f-184">Der Status Allowed wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-184">State Allowed is supported.</span></span>|
|<span data-ttu-id="5f12f-185">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="5f12f-185">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="5f12f-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-187">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen blockieren, eine Verbindung mit dem Computer über das Netzwerk herzustellen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-187">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="5f12f-188">Status Block wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-188">State Block is supported.</span></span>|
|<span data-ttu-id="5f12f-189">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5f12f-189">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="5f12f-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-191">Dieses Benutzerrecht ermöglicht es einem Prozess, einen beliebigen Benutzer ohne Authentifizierung zu imitieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-191">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="5f12f-192">Der Prozess kann daher Zugriff auf die gleichen lokalen Ressourcen wie diesen Benutzer erlangen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-192">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="5f12f-193">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-194">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="5f12f-194">userRightsLocalLogOn</span></span>|[<span data-ttu-id="5f12f-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-196">Dieses Benutzerrecht bestimmt, welche Benutzer sich am Computer anmelden können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-196">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="5f12f-197">Status NotConfigured, zulässig und blockiert werden alle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-197">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="5f12f-198">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="5f12f-198">userRightsBackupData</span></span>|[<span data-ttu-id="5f12f-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-200">Dieses Benutzerrecht bestimmt, welche Benutzer beim Sichern von Dateien und Verzeichnissen Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-200">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="5f12f-201">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-202">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="5f12f-202">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="5f12f-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-204">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen die Uhrzeit und das Datum für die interne Uhr des Computers ändern können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-204">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="5f12f-205">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-206">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="5f12f-206">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="5f12f-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-208">Diese Sicherheitseinstellung bestimmt, ob Benutzer globale Objekte erstellen können, die für alle Sitzungen zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-208">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="5f12f-209">Benutzer, die globale Objekte erstellen können, könnten sich auf Prozesse auswirken, die in Sitzungen anderer Benutzer ausgeführt werden, was zu Anwendungsfehlern oder Datenbeschädigungen führen kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-209">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="5f12f-210">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-211">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="5f12f-211">userRightsCreatePageFile</span></span>|[<span data-ttu-id="5f12f-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-213">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen eine interne API aufrufen können, um die Größe einer Auslagerungsdatei zu erstellen und zu ändern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-213">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="5f12f-214">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-215">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="5f12f-215">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="5f12f-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-217">Dieses Benutzerrecht bestimmt, welche Konten von Prozessen verwendet werden können, um mithilfe des Objekt-Managers ein Verzeichnisobjekt zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-217">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="5f12f-218">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-219">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="5f12f-219">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="5f12f-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-221">Dieses Benutzerrecht bestimmt, ob der Benutzer einen symbolischen Link von dem Computer aus erstellen kann, auf dem Sie angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-221">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="5f12f-222">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-223">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="5f12f-223">userRightsCreateToken</span></span>|[<span data-ttu-id="5f12f-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-225">Dieses Benutzerrecht bestimmt, welche Benutzer/Gruppen von Prozessen verwendet werden können, um ein Token zu erstellen, das dann verwendet werden kann, um Zugriff auf lokale Ressourcen zu erhalten, wenn der Prozess eine interne API zum Erstellen eines Zugriffstokens verwendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-225">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="5f12f-226">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-227">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="5f12f-227">userRightsDebugPrograms</span></span>|[<span data-ttu-id="5f12f-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-229">Dieses Benutzerrecht bestimmt, welche Benutzer einen Debugger an einen beliebigen Prozess oder an den Kernel anfügen können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-229">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="5f12f-230">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="5f12f-231">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="5f12f-231">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="5f12f-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-233">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen nicht als Remote Desktop Dienste-Client angemeldet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-233">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="5f12f-234">Nur Status NotConfigured und blockiert werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-234">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="5f12f-235">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="5f12f-235">userRightsDelegation</span></span>|[<span data-ttu-id="5f12f-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-237">Dieses Benutzerrecht bestimmt, welche Benutzer die Einstellung für die vertrauenswürdige deLegierung für ein Benutzer-oder Computerobjekt festlegen können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-237">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="5f12f-238">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-238">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-239">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="5f12f-239">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="5f12f-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-241">Dieses Benutzerrecht bestimmt, welche Konten von einem Prozess zum Hinzufügen von Einträgen zum Sicherheitsprotokoll verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-241">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="5f12f-242">Das Sicherheitsprotokoll wird verwendet, um nicht autorisierten Systemzugriff nachzuverfolgen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-242">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="5f12f-243">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-244">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="5f12f-244">userRightsImpersonateClient</span></span>|[<span data-ttu-id="5f12f-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-246">Durch das Zuweisen dieses Benutzerrechts zu einem Benutzer können Programme, die im Auftrag dieses Benutzers laufen, die Identität eines Clients annehmen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-246">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="5f12f-247">Wenn Sie dieses Benutzerrecht für diese Art von Identitätswechsel benötigen, wird verhindert, dass ein nicht autorisierter Benutzer einen Client dazu überzeugt, eine Verbindung mit einem Dienst herzustellen, den er erstellt hat, und dann die Identität dieses Clients annehmen, wodurch die Berechtigungen des nicht autorisierten Benutzers erhöht werden können administrative oder Systemebenen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-247">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="5f12f-248">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-249">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="5f12f-249">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="5f12f-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-251">Dieses Benutzerrecht bestimmt, welche Konten einen Prozess mit Schreibeigenschaften Zugriff auf einen anderen Prozess verwenden können, um die dem anderen Prozess zugewiesene Ausführungspriorität zu verlängern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-251">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="5f12f-252">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-253">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="5f12f-253">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="5f12f-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-255">Dieses Benutzerrecht bestimmt, welche Benutzer Gerätetreiber oder anderen Code im Kernelmodus dynamisch laden und entladen können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-255">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="5f12f-256">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-257">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="5f12f-257">userRightsLockMemory</span></span>|[<span data-ttu-id="5f12f-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-259">Dieses Benutzerrecht bestimmt, welche Konten einen Prozess verwenden können, um Daten im physischen Arbeitsspeicher zu speichern, wodurch verhindert wird, dass das System die Daten auf dem Datenträger in den virtuellen Arbeitsspeicher eingibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-259">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="5f12f-260">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-261">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="5f12f-261">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="5f12f-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-263">Dieses Benutzerrecht bestimmt, welche Benutzer die Objektzugriffs-Überwachungsoptionen für einzelne Ressourcen wie Dateien, Active Directory-Objekte und Registrierungsschlüssel angeben können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-263">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="5f12f-264">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-265">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="5f12f-265">userRightsManageVolumes</span></span>|[<span data-ttu-id="5f12f-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-267">Dieses Benutzerrecht bestimmt, welche Benutzer und Gruppen Wartungsaufgaben auf einem Volume ausführen können, beispielsweise die Remote Defragmentierung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-267">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="5f12f-268">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-269">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="5f12f-269">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="5f12f-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-271">Dieses Benutzerrecht bestimmt, wer die Werte der Firmware-Umgebung ändern kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-271">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="5f12f-272">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-273">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="5f12f-273">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="5f12f-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-275">Dieses Benutzerrecht bestimmt, welche Benutzerkonten die Integritäts Bezeichnung von Objekten wie Dateien, Registrierungsschlüssel oder Prozesse ändern können, die anderen Benutzern gehören.</span><span class="sxs-lookup"><span data-stu-id="5f12f-275">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="5f12f-276">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-277">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="5f12f-277">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="5f12f-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-279">Dieses Benutzerrecht bestimmt, welche Benutzer Leistungsüberwachungstools verwenden können, um die Leistung von Systemprozessen zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-279">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="5f12f-280">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-281">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="5f12f-281">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="5f12f-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-283">Dieses Benutzerrecht bestimmt, welche Benutzer einen Computer von einem Remotestandort im Netzwerk Herunterfahren dürfen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-283">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="5f12f-284">Missbrauch dieses Benutzerrechts kann zu einem Denial-of-Service führen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-284">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="5f12f-285">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-286">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="5f12f-286">userRightsRestoreData</span></span>|[<span data-ttu-id="5f12f-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-288">Dieses Benutzerrecht bestimmt, welche Benutzer bei der Wiederherstellung gesicherter Dateien und Verzeichnisse Datei-, Verzeichnis-, Registrierungs-und andere persistent Objects-Berechtigungen umgehen können, und bestimmt, welche Benutzer einen gültigen Sicherheitsprinzipal als Besitzer eines Objekts festlegen können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-288">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="5f12f-289">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-290">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="5f12f-290">userRightsTakeOwnership</span></span>|[<span data-ttu-id="5f12f-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-292">Dieses Benutzerrecht bestimmt, welche Benutzer den Besitz eines sicherungsfähigen Objekts im System übernehmen können, einschließlich Active Directory-Objekte, Dateien und Ordner, Drucker, Registrierungsschlüssel, Prozesse und Threads.</span><span class="sxs-lookup"><span data-stu-id="5f12f-292">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="5f12f-293">Nur Status NotConfigured und Allowed werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="5f12f-294">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="5f12f-294">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="5f12f-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="5f12f-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="5f12f-296">Diese Sicherheitseinstellung bestimmt, welche Dienstkonten verhindert werden, einen Prozess als Dienst zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-296">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="5f12f-297">Hinweis: Diese Sicherheitseinstellung gilt nicht für die System-, lokalen Dienst-oder Netzwerkdienstkonten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-297">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="5f12f-298">Nur Status blockiert wird unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-298">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="5f12f-299">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="5f12f-299">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="5f12f-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-300">Boolean</span></span>|<span data-ttu-id="5f12f-301">Diese Einstellung bestimmt, ob Xbox Game Save (1) oder Disabled (0) aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-301">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="5f12f-302">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="5f12f-302">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="5f12f-303">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="5f12f-303">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="5f12f-304">Diese Einstellung bestimmt, ob der Starttyp des Zubehör Verwaltungsdiensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-304">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="5f12f-305">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="5f12f-305">Default: Manual.</span></span> <span data-ttu-id="5f12f-306">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-306">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="5f12f-307">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="5f12f-307">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="5f12f-308">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="5f12f-308">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="5f12f-309">Diese Einstellung bestimmt, ob der Starttyp des Live auth Manager-Diensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-309">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="5f12f-310">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="5f12f-310">Default: Manual.</span></span> <span data-ttu-id="5f12f-311">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-311">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="5f12f-312">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="5f12f-312">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="5f12f-313">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="5f12f-313">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="5f12f-314">Diese Einstellung bestimmt, ob der Starttyp des Live Spiel-Diensts automatisch ist (2), manuell (3), deaktiviert (4).</span><span class="sxs-lookup"><span data-stu-id="5f12f-314">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="5f12f-315">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="5f12f-315">Default: Manual.</span></span> <span data-ttu-id="5f12f-316">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-316">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="5f12f-317">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="5f12f-317">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="5f12f-318">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="5f12f-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="5f12f-319">Diese Einstellung bestimmt, ob der Starttyp des Netzwerkdiensts automatisch (2), manuell (3), deaktiviert (4) ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-319">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="5f12f-320">Standard: manual.</span><span class="sxs-lookup"><span data-stu-id="5f12f-320">Default: Manual.</span></span> <span data-ttu-id="5f12f-321">Mögliche Werte sind: `manual`, `automatic` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="5f12f-322">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="5f12f-322">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="5f12f-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-323">Boolean</span></span>|<span data-ttu-id="5f12f-324">Verhindern, dass Benutzer neue Microsoft-Konten zu diesem Computer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-324">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="5f12f-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="5f12f-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="5f12f-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-326">Boolean</span></span>|<span data-ttu-id="5f12f-327">Aktivieren Sie lokale Konten, die nicht kennwortgeschützt sind, um sich an anderen Speicherorten als dem physischen Gerät anzumelden. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-327">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="5f12f-328">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="5f12f-328">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="5f12f-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-329">Boolean</span></span>|<span data-ttu-id="5f12f-330">Bestimmt, ob das lokale Administrator Konto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-330">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="5f12f-331">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="5f12f-331">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="5f12f-332">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-332">String</span></span>|<span data-ttu-id="5f12f-333">Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Administrator" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-333">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="5f12f-334">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="5f12f-334">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="5f12f-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-335">Boolean</span></span>|<span data-ttu-id="5f12f-336">Bestimmt, ob das Gastkonto aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-336">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="5f12f-337">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="5f12f-337">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="5f12f-338">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-338">String</span></span>|<span data-ttu-id="5f12f-339">Definieren Sie einen anderen Kontonamen, der der Sicherheits-ID (SID) für das Konto "Guest" zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-339">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="5f12f-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="5f12f-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="5f12f-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-341">Boolean</span></span>|<span data-ttu-id="5f12f-342">Verhindern, dass ein tragbarer Computer ohne Anmeldung abdockt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-342">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="5f12f-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="5f12f-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="5f12f-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-344">Boolean</span></span>|<span data-ttu-id="5f12f-345">Beschränken Sie die Installation von Druckertreibern im Rahmen der Verbindung zu einem freigegebenen Drucker nur mit Administratoren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-345">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="5f12f-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="5f12f-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="5f12f-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-347">Boolean</span></span>|<span data-ttu-id="5f12f-348">Wenn Sie diese Einstellung aktivieren, kann nur interaktiv auf CD-ROM-Medien zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-348">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="5f12f-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="5f12f-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="5f12f-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="5f12f-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="5f12f-351">Legen Sie fest, wer Wechseldatenträger formatieren und Auswerfen darf.</span><span class="sxs-lookup"><span data-stu-id="5f12f-351">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="5f12f-352">Mögliche Werte: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-352">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="5f12f-353">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="5f12f-353">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="5f12f-354">Int32</span><span class="sxs-lookup"><span data-stu-id="5f12f-354">Int32</span></span>|<span data-ttu-id="5f12f-355">Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-355">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="5f12f-356">Gültige Werte 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="5f12f-356">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="5f12f-357">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="5f12f-357">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="5f12f-358">Int32</span><span class="sxs-lookup"><span data-stu-id="5f12f-358">Int32</span></span>|<span data-ttu-id="5f12f-359">Definieren Sie maximale Minuten der Inaktivität auf dem Anmeldebildschirm des interaktiven Desktops, bis der Bildschirmschoner ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="5f12f-360">Gültige Werte 0 bis 9999</span><span class="sxs-lookup"><span data-stu-id="5f12f-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="5f12f-361">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="5f12f-361">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="5f12f-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-362">Boolean</span></span>|<span data-ttu-id="5f12f-363">Die Tastenkombination STRG + ALT + ENTF muss gedrückt werden, bevor sich ein Benutzer anmelden kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-363">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="5f12f-364">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="5f12f-364">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="5f12f-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-365">Boolean</span></span>|<span data-ttu-id="5f12f-366">Zeigen Sie nicht den Benutzernamen der letzten Person an, die sich auf diesem Gerät angemeldet hat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-366">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="5f12f-367">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="5f12f-367">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="5f12f-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-368">Boolean</span></span>|<span data-ttu-id="5f12f-369">Zeigen Sie nicht den Benutzernamen der Person an, die sich bei diesem Gerät anmeldet, nachdem Sie die Anmeldeinformationen eingegeben haben, und bevor der Desktop des Geräts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-369">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="5f12f-370">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="5f12f-370">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="5f12f-371">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-371">String</span></span>|<span data-ttu-id="5f12f-372">Festlegen des Nachrichten Titels für Benutzer, die sich anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-372">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="5f12f-373">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="5f12f-373">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="5f12f-374">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-374">String</span></span>|<span data-ttu-id="5f12f-375">Festlegen des Nachrichtentexts für Benutzer, die sich anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-375">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="5f12f-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="5f12f-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="5f12f-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-377">Boolean</span></span>|<span data-ttu-id="5f12f-378">Blockieren Sie PKU2U-Authentifizierungsanforderungen für dieses Gerät, um Online Identitäten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-378">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="5f12f-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="5f12f-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="5f12f-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-380">Boolean</span></span>|<span data-ttu-id="5f12f-381">UI Helper Boolean für LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager-Entität</span><span class="sxs-lookup"><span data-stu-id="5f12f-381">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="5f12f-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="5f12f-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="5f12f-383">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-383">String</span></span>|<span data-ttu-id="5f12f-384">Bearbeiten Sie die standardmäßige Zeichenfolge für die Sicherheitsdeskriptor-Definition, um Benutzern und Gruppen das Ausführen von Remote anrufen für SAM zu erlauben oder zu verweigern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-384">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="5f12f-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="5f12f-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="5f12f-386">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5f12f-386">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="5f12f-387">Mit dieser Sicherheitseinstellung kann ein Client die 128-Bit-Verschlüsselung und/oder die NTLMv2-Sitzungssicherheit aushandeln.</span><span class="sxs-lookup"><span data-stu-id="5f12f-387">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="5f12f-388">Mögliche Werte: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-388">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="5f12f-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="5f12f-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="5f12f-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5f12f-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="5f12f-391">Mit dieser Sicherheitseinstellung kann ein Server die Aushandlung der 128-Bit-Verschlüsselung und/oder der NTLMv2-Sitzungssicherheit erfordern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-391">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="5f12f-392">Mögliche Werte: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="5f12f-393">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="5f12f-393">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="5f12f-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="5f12f-394">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="5f12f-395">Diese Sicherheitseinstellung bestimmt, welches Abfrage-/Antwort Authentifizierungsprotokoll für Netzwerkanmeldungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-395">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="5f12f-396">Mögliche Werte sind: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm` und `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-396">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="5f12f-397">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="5f12f-397">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="5f12f-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-398">Boolean</span></span>|<span data-ttu-id="5f12f-399">Wenn diese Option aktiviert ist, erlaubt der SMB-Client unsichere Gastanmeldungen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-399">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="5f12f-400">Wenn nicht konfiguriert, lehnt der SMB-Client unsichere Gastanmeldungen ab.</span><span class="sxs-lookup"><span data-stu-id="5f12f-400">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="5f12f-401">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="5f12f-401">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="5f12f-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-402">Boolean</span></span>|<span data-ttu-id="5f12f-403">Diese Sicherheitseinstellung bestimmt, ob die Auslagerungsdatei des virtuellen Speichers gelöscht wird, wenn das System heruntergefahren wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-403">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="5f12f-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="5f12f-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="5f12f-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-405">Boolean</span></span>|<span data-ttu-id="5f12f-406">Diese Sicherheitseinstellung bestimmt, ob ein Computer heruntergefahren werden kann, ohne sich bei Windows anmelden zu müssen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-406">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="5f12f-407">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="5f12f-407">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="5f12f-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-408">Boolean</span></span>|<span data-ttu-id="5f12f-409">Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-409">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="5f12f-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="5f12f-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="5f12f-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-411">Boolean</span></span>|<span data-ttu-id="5f12f-412">Virtualisieren von Datei-und Registrierungs Schreibfehlern pro Benutzerspeicherorte</span><span class="sxs-lookup"><span data-stu-id="5f12f-412">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="5f12f-413">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="5f12f-413">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="5f12f-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-414">Boolean</span></span>|<span data-ttu-id="5f12f-415">Erzwingen Sie die Validierung des PKI-Zertifizierungspfads für eine bestimmte ausführbare Datei, bevor Sie ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-415">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="5f12f-416">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="5f12f-416">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="5f12f-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="5f12f-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="5f12f-418">Definieren Sie das Verhalten der Eingabeaufforderung für Administratoren im AdministratorgenehmigungsModus.</span><span class="sxs-lookup"><span data-stu-id="5f12f-418">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="5f12f-419">Mögliche Werte sind: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent` und `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-419">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="5f12f-420">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="5f12f-420">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="5f12f-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="5f12f-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="5f12f-422">Definieren Sie das Verhalten der Eingabeaufforderung für Standardbenutzer.</span><span class="sxs-lookup"><span data-stu-id="5f12f-422">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="5f12f-423">Mögliche Werte: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-423">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="5f12f-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="5f12f-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="5f12f-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-425">Boolean</span></span>|<span data-ttu-id="5f12f-426">Aktivieren Sie alle Elevation-Anforderungen, um anstelle des sicheren Desktops zum Desktop des interaktiven Benutzers zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="5f12f-426">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="5f12f-427">Richtlinieneinstellungen für das Ansage Verhalten für Administratoren und Standardbenutzer werden verwendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-427">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="5f12f-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="5f12f-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="5f12f-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-429">Boolean</span></span>|<span data-ttu-id="5f12f-430">App-Installationen, die erhöhte Rechte erfordern, werden zur Eingabe von Administratoranmeldeinformationen aufgefordert. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-430">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="5f12f-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="5f12f-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="5f12f-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-432">Boolean</span></span>|<span data-ttu-id="5f12f-433">Zulassen, dass UIAccess-apps ohne Verwendung des sicheren Desktops zur Eingabe aufgefordert werden. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-433">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="5f12f-434">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="5f12f-434">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="5f12f-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-435">Boolean</span></span>|<span data-ttu-id="5f12f-436">Definiert, ob das integrierte Administratorkonto den AdministratorgenehmigungsModus verwendet oder alle apps mit vollständigen Administratorrechten ausführt. Standard ist aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-436">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="5f12f-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="5f12f-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="5f12f-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-438">Boolean</span></span>|<span data-ttu-id="5f12f-439">Legen Sie fest, ob der AdministratorgenehmigungsModus und alle UAC-Richtlinieneinstellungen aktiviert sind, Standard ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-439">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="5f12f-440">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="5f12f-440">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="5f12f-441">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="5f12f-441">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="5f12f-442">Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-442">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="5f12f-443">Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-443">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="5f12f-444">Mögliche Werte: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-444">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="5f12f-445">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="5f12f-445">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="5f12f-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="5f12f-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="5f12f-447">Konfigurieren Sie die Benutzerinformationen, die angezeigt werden, wenn die Sitzung gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-447">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="5f12f-448">Wenn nicht konfiguriert, werden Benutzeranzeigename, Domäne und Benutzername angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-448">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="5f12f-449">Mögliche Werte: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-449">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="5f12f-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="5f12f-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="5f12f-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-451">Boolean</span></span>|<span data-ttu-id="5f12f-452">Diese Sicherheitseinstellung bestimmt, ob der SMB-Client versucht, die SMB-Paketsignierung auszuhandeln.</span><span class="sxs-lookup"><span data-stu-id="5f12f-452">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="5f12f-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="5f12f-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="5f12f-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-454">Boolean</span></span>|<span data-ttu-id="5f12f-455">Diese Sicherheitseinstellung bestimmt, ob die Paketsignierung für die SMB-Clientkomponente erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-455">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="5f12f-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="5f12f-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="5f12f-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-457">Boolean</span></span>|<span data-ttu-id="5f12f-458">Wenn diese Sicherheitseinstellung aktiviert ist, kann der SMB-Redirector (Server Message Block) Klartext-Kennwörter an nicht-Microsoft SMB-Server senden, die die Kennwortverschlüsselung während der Authentifizierung nicht unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-458">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="5f12f-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="5f12f-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="5f12f-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-460">Boolean</span></span>|<span data-ttu-id="5f12f-461">Diese Sicherheitseinstellung bestimmt, ob für die SMB-Serverkomponente eine Paketsignierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-461">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="5f12f-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="5f12f-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="5f12f-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-463">Boolean</span></span>|<span data-ttu-id="5f12f-464">Diese Sicherheitseinstellung bestimmt, ob der SMB-Server die SMB-Paketsignierung mit Clients aushandelt, die ihn anfordern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-464">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="5f12f-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="5f12f-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="5f12f-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-466">Boolean</span></span>|<span data-ttu-id="5f12f-467">Diese Sicherheitseinstellung beschränkt den anonymen Zugriff auf Freigaben und Pipes standardmäßig auf die Einstellungen für Named Pipes, auf die anonym zugegriffen werden kann, und auf Freigaben, auf die anonym zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-467">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="5f12f-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="5f12f-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="5f12f-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-469">Boolean</span></span>|<span data-ttu-id="5f12f-470">Diese Sicherheitseinstellung bestimmt, welche zusätzlichen Berechtigungen für anonyme Verbindungen mit dem Computer erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-470">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="5f12f-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="5f12f-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="5f12f-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-472">Boolean</span></span>|<span data-ttu-id="5f12f-473">Diese Sicherheitseinstellung bestimmt, ob anonyme Benutzer bestimmte Aktivitäten ausführen können, beispielsweise das Aufzählen der Namen von Domänenkonten und Netzwerkfreigaben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-473">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="5f12f-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="5f12f-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="5f12f-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-475">Boolean</span></span>|<span data-ttu-id="5f12f-476">Diese Sicherheitseinstellung bestimmt, ob bei der nächsten Kennwortänderung der LAN-Manager (LM)-Hashwert für das neue Kennwort gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-476">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="5f12f-477">Sie wird nicht standardmäßig gespeichert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-477">It’s not stored by default.</span></span>|
|<span data-ttu-id="5f12f-478">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="5f12f-478">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="5f12f-479">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="5f12f-479">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="5f12f-480">Diese Sicherheitseinstellung bestimmt, was geschieht, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Lesegerät entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-480">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="5f12f-481">Mögliche Werte: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-481">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="5f12f-482">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-482">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="5f12f-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-483">Boolean</span></span>|<span data-ttu-id="5f12f-484">Wird verwendet, um die Anzeige des App-und Browser Schutzbereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-484">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="5f12f-485">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-485">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="5f12f-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-486">Boolean</span></span>|<span data-ttu-id="5f12f-487">Wird verwendet, um die Anzeige des Bereichs Familienoptionen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-487">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="5f12f-488">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-488">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="5f12f-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-489">Boolean</span></span>|<span data-ttu-id="5f12f-490">Wird verwendet, um die Anzeige der Geräteleistung und des Integritäts Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-490">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="5f12f-491">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-491">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="5f12f-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-492">Boolean</span></span>|<span data-ttu-id="5f12f-493">Wird verwendet, um die Anzeige des Firewall-und Netzwerkschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-493">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="5f12f-494">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-494">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="5f12f-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-495">Boolean</span></span>|<span data-ttu-id="5f12f-496">Wird verwendet, um die Anzeige des Viren-und Bedrohungsschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-496">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="5f12f-497">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-497">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="5f12f-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-498">Boolean</span></span>|<span data-ttu-id="5f12f-499">Wird verwendet, um die Anzeige des Kontoschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-499">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="5f12f-500">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-500">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="5f12f-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-501">Boolean</span></span>|<span data-ttu-id="5f12f-502">Wird verwendet, um die Anzeige der Schaltfläche TPM löschen zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-502">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="5f12f-503">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-503">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="5f12f-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-504">Boolean</span></span>|<span data-ttu-id="5f12f-505">Wird verwendet, um die Anzeige des Hardwareschutz Bereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-505">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="5f12f-506">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-506">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="5f12f-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-507">Boolean</span></span>|<span data-ttu-id="5f12f-508">Wird verwendet, um die Anzeige des Benachrichtigungsbereichs-Steuerelements zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-508">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="5f12f-509">Der Benutzer muss sich abmelden und sich anmelden oder den Computer neu starten, damit diese Einstellung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-509">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="5f12f-510">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-510">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="5f12f-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-511">Boolean</span></span>|<span data-ttu-id="5f12f-512">Wird verwendet, um die Anzeige des Ransomware-Schutzbereichs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-512">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="5f12f-513">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-513">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="5f12f-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-514">Boolean</span></span>|<span data-ttu-id="5f12f-515">Wird verwendet, um die Anzeige des sicheren Startbereichs unter Gerätesicherheit zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-515">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="5f12f-516">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-516">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="5f12f-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-517">Boolean</span></span>|<span data-ttu-id="5f12f-518">Wird verwendet, um die Anzeige der Sicherheitsprozess-Problembehandlung unter Gerätesicherheit zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-518">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="5f12f-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="5f12f-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="5f12f-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-520">Boolean</span></span>|<span data-ttu-id="5f12f-521">Wird verwendet, um die Anzeige der TPM-Update-Firmware zu deaktivieren, wenn eine Sicherheitsanfälligkeit erkannt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-521">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="5f12f-522">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="5f12f-522">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="5f12f-523">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-523">String</span></span>|<span data-ttu-id="5f12f-524">Der Name des Unternehmens, der den Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-524">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="5f12f-525">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="5f12f-525">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="5f12f-526">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-526">String</span></span>|<span data-ttu-id="5f12f-527">Die e-Mail-Adresse, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-527">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="5f12f-528">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="5f12f-528">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="5f12f-529">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-529">String</span></span>|<span data-ttu-id="5f12f-530">Die Telefonnummer oder die Skype-ID, die Benutzern angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-530">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="5f12f-531">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="5f12f-531">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="5f12f-532">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-532">String</span></span>|<span data-ttu-id="5f12f-533">Die URL des Hilfe Portals, die für Benutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-533">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="5f12f-534">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="5f12f-534">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="5f12f-535">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="5f12f-535">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="5f12f-536">Benachrichtigungen, die aus den angezeigten Bereichen der App angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-536">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="5f12f-537">Mögliche Werte sind: `notConfigured`, `blockNoncriticalNotifications` und `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-537">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="5f12f-538">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="5f12f-538">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="5f12f-539">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="5f12f-539">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="5f12f-540">Konfigurieren Sie, wo die IT-Kontaktinformationen Endbenutzern angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-540">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="5f12f-541">Mögliche Werte: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-541">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="5f12f-542">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="5f12f-542">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="5f12f-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-543">Boolean</span></span>|<span data-ttu-id="5f12f-544">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="5f12f-544">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="5f12f-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="5f12f-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="5f12f-546">Int32</span><span class="sxs-lookup"><span data-stu-id="5f12f-546">Int32</span></span>|<span data-ttu-id="5f12f-547">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="5f12f-547">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="5f12f-548">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-548">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="5f12f-549">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="5f12f-549">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="5f12f-550">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="5f12f-550">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="5f12f-551">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="5f12f-551">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="5f12f-552">Wählen Sie die zu verwendende vorinstallierte Tasten Codierung aus.</span><span class="sxs-lookup"><span data-stu-id="5f12f-552">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="5f12f-553">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-553">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="5f12f-554">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="5f12f-554">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="5f12f-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-555">Boolean</span></span>|<span data-ttu-id="5f12f-556">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-556">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="5f12f-557">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="5f12f-557">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="5f12f-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-558">Boolean</span></span>|<span data-ttu-id="5f12f-559">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-559">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="5f12f-560">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="5f12f-560">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="5f12f-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-561">Boolean</span></span>|<span data-ttu-id="5f12f-562">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-562">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="5f12f-563">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="5f12f-563">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="5f12f-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-564">Boolean</span></span>|<span data-ttu-id="5f12f-565">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-565">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="5f12f-566">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="5f12f-566">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="5f12f-567">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="5f12f-567">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="5f12f-568">Geben Sie an, wie die Zertifikatssperrliste erzwungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-568">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="5f12f-569">Mögliche Werte: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-569">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="5f12f-570">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="5f12f-570">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="5f12f-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-571">Boolean</span></span>|<span data-ttu-id="5f12f-572">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="5f12f-572">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="5f12f-573">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="5f12f-573">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="5f12f-574">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="5f12f-574">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="5f12f-575">Konfiguriert, wie Paketwarteschlangen im Tunnel Gateway-Szenario angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-575">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="5f12f-576">Mögliche Werte: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-576">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="5f12f-577">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="5f12f-577">firewallProfileDomain</span></span>|[<span data-ttu-id="5f12f-578">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5f12f-578">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="5f12f-579">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="5f12f-579">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="5f12f-580">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="5f12f-580">firewallProfilePublic</span></span>|[<span data-ttu-id="5f12f-581">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5f12f-581">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="5f12f-582">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="5f12f-582">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="5f12f-583">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="5f12f-583">firewallProfilePrivate</span></span>|[<span data-ttu-id="5f12f-584">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5f12f-584">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="5f12f-585">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="5f12f-585">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="5f12f-586">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="5f12f-586">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="5f12f-587">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-587">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-588">Wert, der das Verhalten von Adobe Reader beim Erstellen von untergeordneten Prozessen angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-588">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="5f12f-589">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-589">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-590">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="5f12f-590">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="5f12f-591">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5f12f-591">String collection</span></span>|<span data-ttu-id="5f12f-592">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-592">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="5f12f-593">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-593">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="5f12f-594">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-594">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-595">Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-595">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="5f12f-596">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-596">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-597">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="5f12f-597">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="5f12f-598">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-598">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-599">Wert, der das Verhalten von Office-Anwendungen angibt, das in andere Prozesse einfügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-599">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="5f12f-600">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-600">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-601">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="5f12f-601">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="5f12f-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-603">Wert, der das Verhalten von Office-Kommunikationsanwendungen, einschließlich Microsoft Outlook, zum Erstellen von untergeordneten Prozessen angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-603">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="5f12f-604">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="5f12f-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="5f12f-606">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-606">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-607">Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-607">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="5f12f-608">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-608">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="5f12f-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="5f12f-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-611">Wert, der das Verhalten von Office-Anwendungen/-Makros angibt, die ausführbare Inhalte erstellen oder starten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="5f12f-612">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-612">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-613">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="5f12f-613">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="5f12f-614">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-615">Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse.</span><span class="sxs-lookup"><span data-stu-id="5f12f-615">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="5f12f-616">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-617">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="5f12f-617">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="5f12f-618">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-619">Wert, der das Verhalten der Office-Anwendung startet untergeordnete Prozesse.</span><span class="sxs-lookup"><span data-stu-id="5f12f-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="5f12f-620">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-621">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="5f12f-621">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="5f12f-622">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-623">Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-623">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="5f12f-624">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-625">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="5f12f-625">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="5f12f-626">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-627">Wert, der das Verhalten von Win32-Importen aus Makrocode in Office angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="5f12f-628">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-629">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="5f12f-629">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="5f12f-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-631">Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-631">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="5f12f-632">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-633">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="5f12f-633">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="5f12f-634">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-635">Wert, der das Verhalten von verschleierten js/VBS/PS/Macro-Code angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="5f12f-636">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-637">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-637">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="5f12f-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-639">Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-639">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="5f12f-640">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-641">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="5f12f-641">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="5f12f-642">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-643">Wert, der das Verhalten von JS/VBS ausführt, das aus dem Internet heruntergeladen wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="5f12f-644">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-645">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="5f12f-645">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="5f12f-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-647">Wert, der angibt, ob das unter System für die Windows Local Security Authority gestohlen werden darf.</span><span class="sxs-lookup"><span data-stu-id="5f12f-647">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="5f12f-648">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-649">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="5f12f-649">defenderProcessCreationType</span></span>|[<span data-ttu-id="5f12f-650">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-651">Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-651">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="5f12f-652">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-653">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="5f12f-653">defenderProcessCreation</span></span>|[<span data-ttu-id="5f12f-654">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-655">Wert, der die Antwort auf Prozess Kreationen aus PSExec und WMI-Befehlen angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="5f12f-656">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-657">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="5f12f-657">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="5f12f-658">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-659">Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-659">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="5f12f-660">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-661">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="5f12f-661">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="5f12f-662">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-663">Wert, der die Antwort auf nicht vertrauenswürdige und nicht signierte Prozesse angibt, die von USB ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="5f12f-664">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-665">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="5f12f-665">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="5f12f-666">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-667">Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-667">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="5f12f-668">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-669">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="5f12f-669">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="5f12f-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-671">Wert, der die Antwort auf ausführbare Dateien angibt, die den Kriterien Prävalenz, Alter oder Vertrauenswürdige Listen nicht entsprechen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="5f12f-672">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-673">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-673">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="5f12f-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5f12f-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="5f12f-675">Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-675">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="5f12f-676">Mögliche Werte sind: `userDefined`, `block` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-677">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="5f12f-677">defenderEmailContentExecution</span></span>|[<span data-ttu-id="5f12f-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-679">Wert, der angibt, ob die Ausführung von ausführbaren Inhalten (exe, dll, PS, JS, VBS usw.) aus e-Mail (Webmail/Mail-Client) gelöscht werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="5f12f-680">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-681">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-681">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="5f12f-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-683">Wert, der die Verwendung von erweitertem Schutz gegen ransomeware angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-683">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="5f12f-684">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-685">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="5f12f-685">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="5f12f-686">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-686">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="5f12f-687">Wert, der das Verhalten von geschützten Ordnern angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-687">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="5f12f-688">Mögliche Werte: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-688">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="5f12f-689">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="5f12f-689">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="5f12f-690">String collection</span><span class="sxs-lookup"><span data-stu-id="5f12f-690">String collection</span></span>|<span data-ttu-id="5f12f-691">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-691">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="5f12f-692">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="5f12f-692">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="5f12f-693">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5f12f-693">String collection</span></span>|<span data-ttu-id="5f12f-694">Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-694">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="5f12f-695">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-695">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="5f12f-696">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="5f12f-696">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="5f12f-697">Wert, der das Verhalten von NetworkProtection angibt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-697">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="5f12f-698">Mögliche Werte sind: `userDefined`, `enable` und `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-698">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="5f12f-699">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="5f12f-699">defenderExploitProtectionXml</span></span>|<span data-ttu-id="5f12f-700">Binär</span><span class="sxs-lookup"><span data-stu-id="5f12f-700">Binary</span></span>|<span data-ttu-id="5f12f-701">XML-Inhalte mit Details zum Exploit-Schutz.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-701">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="5f12f-702">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="5f12f-702">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="5f12f-703">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-703">String</span></span>|<span data-ttu-id="5f12f-704">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-704">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="5f12f-705">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="5f12f-705">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="5f12f-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-706">Boolean</span></span>|<span data-ttu-id="5f12f-707">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-707">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="5f12f-708">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="5f12f-708">appLockerApplicationControl</span></span>|[<span data-ttu-id="5f12f-709">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="5f12f-709">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="5f12f-710">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="5f12f-710">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="5f12f-711">Mögliche Werte: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-711">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="5f12f-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="5f12f-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="5f12f-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="5f12f-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="5f12f-714">Aktivieren Sie die Aktivierung der Anmeldeinformationen, wenn die Platt Form sicherheitsStufe mit Secure Boot-und Virtualisierungs-basierter Sicherheit aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-714">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="5f12f-715">Mögliche Werte sind: `notConfigured`, `enableWithUEFILock` und `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-715">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="5f12f-716">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="5f12f-716">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="5f12f-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-717">Boolean</span></span>|<span data-ttu-id="5f12f-718">Aktiviert die Virtualisierungs-basierte Sicherheit (VBS).</span><span class="sxs-lookup"><span data-stu-id="5f12f-718">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="5f12f-719">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="5f12f-719">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="5f12f-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-720">Boolean</span></span>|<span data-ttu-id="5f12f-721">Gibt an, ob die Platt Form sicherheitsStufe beim nächsten Neustart aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-721">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="5f12f-722">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="5f12f-722">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="5f12f-723">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-723">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f12f-724">Ermöglicht es dem IT-Administrator, den Start von System Guard zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-724">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="5f12f-725">Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-725">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f12f-726">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="5f12f-726">smartScreenEnableInShell</span></span>|<span data-ttu-id="5f12f-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-727">Boolean</span></span>|<span data-ttu-id="5f12f-728">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="5f12f-728">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="5f12f-729">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="5f12f-729">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="5f12f-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-730">Boolean</span></span>|<span data-ttu-id="5f12f-731">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-731">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="5f12f-732">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="5f12f-732">applicationGuardEnabled</span></span>|<span data-ttu-id="5f12f-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-733">Boolean</span></span>|<span data-ttu-id="5f12f-734">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="5f12f-734">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="5f12f-735">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="5f12f-735">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="5f12f-736">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="5f12f-736">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="5f12f-737">Aktivieren Sie Windows Defender Application Guard für neuere Windows-Builds.</span><span class="sxs-lookup"><span data-stu-id="5f12f-737">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="5f12f-738">Mögliche Werte: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-738">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="5f12f-739">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="5f12f-739">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="5f12f-740">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="5f12f-740">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="5f12f-741">Zwischenablage zum Übertragen der Bilddatei, Textdatei oder keiner dieser Dateien blockieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-741">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="5f12f-742">Mögliche Werte: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-742">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="5f12f-743">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="5f12f-743">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="5f12f-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-744">Boolean</span></span>|<span data-ttu-id="5f12f-745">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-745">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="5f12f-746">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="5f12f-746">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="5f12f-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-747">Boolean</span></span>|<span data-ttu-id="5f12f-748">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="5f12f-748">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="5f12f-749">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="5f12f-749">applicationGuardForceAuditing</span></span>|<span data-ttu-id="5f12f-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-750">Boolean</span></span>|<span data-ttu-id="5f12f-751">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="5f12f-751">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="5f12f-752">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="5f12f-752">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="5f12f-753">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="5f12f-753">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="5f12f-754">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-754">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="5f12f-755">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-755">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="5f12f-756">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="5f12f-756">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="5f12f-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-757">Boolean</span></span>|<span data-ttu-id="5f12f-758">Erlaubt das Drucken im PDF-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-758">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="5f12f-759">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="5f12f-759">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="5f12f-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-760">Boolean</span></span>|<span data-ttu-id="5f12f-761">Erlaubt das Drucken im XPS-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-761">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="5f12f-762">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="5f12f-762">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="5f12f-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-763">Boolean</span></span>|<span data-ttu-id="5f12f-764">Erlaubt das Drucken auf lokalen Druckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-764">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="5f12f-765">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="5f12f-765">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="5f12f-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-766">Boolean</span></span>|<span data-ttu-id="5f12f-767">Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-767">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="5f12f-768">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="5f12f-768">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="5f12f-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-769">Boolean</span></span>|<span data-ttu-id="5f12f-770">Anwendungsschutz für die Verwendung virtueller GPU zulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-770">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="5f12f-771">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="5f12f-771">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="5f12f-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-772">Boolean</span></span>|<span data-ttu-id="5f12f-773">Benutzer können Dateien von Edge im Application Guard-Container herunterladen und im Hostdateisystem speichern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-773">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="5f12f-774">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="5f12f-774">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="5f12f-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-775">Boolean</span></span>|<span data-ttu-id="5f12f-776">Ermöglicht es dem Administrator, Standardbenutzern das Aktivieren von encrpytion während des Azure AD-Joins zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-776">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="5f12f-777">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="5f12f-777">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="5f12f-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-778">Boolean</span></span>|<span data-ttu-id="5f12f-779">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-779">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="5f12f-780">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="5f12f-780">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="5f12f-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-781">Boolean</span></span>|<span data-ttu-id="5f12f-782">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-782">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="5f12f-783">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="5f12f-783">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="5f12f-784">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="5f12f-784">bitLockerEncryptDevice</span></span>|<span data-ttu-id="5f12f-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f12f-785">Boolean</span></span>|<span data-ttu-id="5f12f-786">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="5f12f-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="5f12f-787">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-787">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="5f12f-788">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-788">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="5f12f-789">BitLocker-System Laufwerk Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="5f12f-789">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="5f12f-790">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-790">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="5f12f-791">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-791">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="5f12f-792">BitLocker-Richtlinie für feste Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="5f12f-792">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="5f12f-793">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-793">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="5f12f-794">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5f12f-794">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="5f12f-795">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="5f12f-795">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5f12f-796">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f12f-796">Response</span></span>
<span data-ttu-id="5f12f-797">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5f12f-797">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f12f-798">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f12f-798">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f12f-799">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f12f-799">Request</span></span>
<span data-ttu-id="5f12f-800">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-800">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26778

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

### <a name="response"></a><span data-ttu-id="5f12f-801">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f12f-801">Response</span></span>
<span data-ttu-id="5f12f-p198">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-p198">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26950

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




