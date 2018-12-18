---
title: AndroidDeviceOwnerGeneralDeviceConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidDeviceOwnerGeneralDeviceConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: bf81569d5af7e223ff24e34bc031a19633d22edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340096"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="1a5b6-103">AndroidDeviceOwnerGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1a5b6-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1a5b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a5b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a5b6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a5b6-107">Aktualisieren Sie die Eigenschaften eines [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a5b6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a5b6-108">Prerequisites</span></span>
<span data-ttu-id="1a5b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a5b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a5b6-111">Permission type</span></span>|<span data-ttu-id="1a5b6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a5b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a5b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a5b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a5b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a5b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a5b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a5b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a5b6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a5b6-116">Not supported.</span></span>|
|<span data-ttu-id="1a5b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a5b6-117">Application</span></span>|<span data-ttu-id="1a5b6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a5b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a5b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a5b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1a5b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a5b6-120">Request headers</span></span>
|<span data-ttu-id="1a5b6-121">Header</span><span class="sxs-lookup"><span data-stu-id="1a5b6-121">Header</span></span>|<span data-ttu-id="1a5b6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1a5b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a5b6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1a5b6-123">Authorization</span></span>|<span data-ttu-id="1a5b6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a5b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a5b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a5b6-125">Accept</span></span>|<span data-ttu-id="1a5b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a5b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a5b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a5b6-127">Request body</span></span>
<span data-ttu-id="1a5b6-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1a5b6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1a5b6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a5b6-130">Property</span></span>|<span data-ttu-id="1a5b6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1a5b6-131">Type</span></span>|<span data-ttu-id="1a5b6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a5b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a5b6-133">id</span><span class="sxs-lookup"><span data-stu-id="1a5b6-133">id</span></span>|<span data-ttu-id="1a5b6-134">String</span><span class="sxs-lookup"><span data-stu-id="1a5b6-134">String</span></span>|<span data-ttu-id="1a5b6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1a5b6-135">Key of the entity.</span></span> <span data-ttu-id="1a5b6-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a5b6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1a5b6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a5b6-138">DateTimeOffset</span></span>|<span data-ttu-id="1a5b6-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1a5b6-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a5b6-141">roleScopeTagIds</span></span>|<span data-ttu-id="1a5b6-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1a5b6-142">String collection</span></span>|<span data-ttu-id="1a5b6-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a5b6-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a5b6-145">supportsScopeTags</span></span>|<span data-ttu-id="1a5b6-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-146">Boolean</span></span>|<span data-ttu-id="1a5b6-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a5b6-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a5b6-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a5b6-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-150">This property is read-only.</span></span> <span data-ttu-id="1a5b6-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a5b6-152">createdDateTime</span></span>|<span data-ttu-id="1a5b6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a5b6-153">DateTimeOffset</span></span>|<span data-ttu-id="1a5b6-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-154">DateTime the object was created.</span></span> <span data-ttu-id="1a5b6-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-156">description</span><span class="sxs-lookup"><span data-stu-id="1a5b6-156">description</span></span>|<span data-ttu-id="1a5b6-157">String</span><span class="sxs-lookup"><span data-stu-id="1a5b6-157">String</span></span>|<span data-ttu-id="1a5b6-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a5b6-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1a5b6-160">displayName</span></span>|<span data-ttu-id="1a5b6-161">String</span><span class="sxs-lookup"><span data-stu-id="1a5b6-161">String</span></span>|<span data-ttu-id="1a5b6-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a5b6-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-164">Version</span><span class="sxs-lookup"><span data-stu-id="1a5b6-164">version</span></span>|<span data-ttu-id="1a5b6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-165">Int32</span></span>|<span data-ttu-id="1a5b6-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-166">Version of the device configuration.</span></span> <span data-ttu-id="1a5b6-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a5b6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a5b6-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="1a5b6-168">accountsBlockModification</span></span>|<span data-ttu-id="1a5b6-169">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-169">Boolean</span></span>|<span data-ttu-id="1a5b6-170">Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="1a5b6-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1a5b6-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="1a5b6-172">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-172">Boolean</span></span>|<span data-ttu-id="1a5b6-173">Gibt an, ob der Benutzer berechtigt ist, um das Festlegen von unbekannten Quellen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="1a5b6-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="1a5b6-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="1a5b6-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="1a5b6-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="1a5b6-176">Gibt den Wert des app-Richtlinie für die automatische Aktualisierung.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="1a5b6-177">Mögliche Werte sind: `notConfigured`, `userChoice`, `never`, `wiFiOnly` und `always`.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="1a5b6-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="1a5b6-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="1a5b6-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1a5b6-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="1a5b6-180">Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, ob eine nicht für die app speziell definiert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="1a5b6-181">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1a5b6-182">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a5b6-182">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="1a5b6-183">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-183">Boolean</span></span>|<span data-ttu-id="1a5b6-184">Gibt an, ob vom Bluetooth konfigurieren einen Benutzer blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-184">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="1a5b6-185">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="1a5b6-185">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="1a5b6-186">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-186">Boolean</span></span>|<span data-ttu-id="1a5b6-187">Gibt an, ob einen Benutzer von der Freigabe von Kontakten über Bluetooth blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-187">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="1a5b6-188">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-188">cameraBlocked</span></span>|<span data-ttu-id="1a5b6-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1a5b6-189">Boolean</span></span>|<span data-ttu-id="1a5b6-190">Gibt an, ob die Verwendung der Kamera zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-190">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="1a5b6-191">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="1a5b6-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="1a5b6-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1a5b6-192">Boolean</span></span>|<span data-ttu-id="1a5b6-193">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-193">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="1a5b6-194">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-194">dataRoamingBlocked</span></span>|<span data-ttu-id="1a5b6-195">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-195">Boolean</span></span>|<span data-ttu-id="1a5b6-196">Gibt an, ob einen Benutzer von servergespeicherten Daten blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-196">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="1a5b6-197">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-197">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="1a5b6-198">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-198">Boolean</span></span>|<span data-ttu-id="1a5b6-199">Gibt an, ob die Benutzer manuell ändern, die Datums- oder Uhrzeitwerte auf dem Gerät blockieren</span><span class="sxs-lookup"><span data-stu-id="1a5b6-199">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="1a5b6-200">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="1a5b6-200">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="1a5b6-201">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1a5b6-201">String collection</span></span>|<span data-ttu-id="1a5b6-202">Liste der Google-Konto-e-Mails, die erforderlich sind, um zu authentifizieren, nachdem ein Gerät ist Factory zurückzusetzen, bevor eingerichtet werden kann.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-202">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="1a5b6-203">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-203">factoryResetBlocked</span></span>|<span data-ttu-id="1a5b6-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1a5b6-204">Boolean</span></span>|<span data-ttu-id="1a5b6-205">Gibt an, ob die Option zum Factory in den Einstellungen deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-205">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="1a5b6-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="1a5b6-206">kioskModeApps</span></span>|<span data-ttu-id="1a5b6-207">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a5b6-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1a5b6-208">Eine Liste der verwalteten apps, die das Gerät bei im Kioskmodus zurückgekehrt ist angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-208">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="1a5b6-209">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1a5b6-210">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="1a5b6-210">microphoneForceMute</span></span>|<span data-ttu-id="1a5b6-211">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-211">Boolean</span></span>|<span data-ttu-id="1a5b6-212">Gibt an, ob blockieren Aufheben der stummschaltung für das Mikrofon auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-212">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="1a5b6-213">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="1a5b6-213">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="1a5b6-214">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-214">Boolean</span></span>|<span data-ttu-id="1a5b6-215">Gibt an, ob das Gerät zulässig, eine Verbindung mit einer temporären-Verbindung beim Starten.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-215">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="1a5b6-216">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="1a5b6-216">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="1a5b6-217">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-217">Boolean</span></span>|<span data-ttu-id="1a5b6-218">Gibt an, ob ausgehende Balken NFK blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-218">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="1a5b6-219">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="1a5b6-219">passwordBlockKeyguard</span></span>|<span data-ttu-id="1a5b6-220">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-220">Boolean</span></span>|<span data-ttu-id="1a5b6-221">Gibt an, ob die Keyguard deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-221">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="1a5b6-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1a5b6-222">passwordExpirationDays</span></span>|<span data-ttu-id="1a5b6-223">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-223">Int32</span></span>|<span data-ttu-id="1a5b6-224">Gibt die Zeitspanne in Sekunden an, die für ein Kennwort festgelegt werden kann, bevor sie abläuft und ein neues Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-224">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="1a5b6-225">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1a5b6-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1a5b6-226">passwordMinimumLength</span></span>|<span data-ttu-id="1a5b6-227">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-227">Int32</span></span>|<span data-ttu-id="1a5b6-228">Gibt die minimale Länge des Kennworts auf dem Gerät erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-228">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="1a5b6-229">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1a5b6-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1a5b6-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1a5b6-231">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-231">Int32</span></span>|<span data-ttu-id="1a5b6-232">Zeit in Millisekunden vor dem Timeout der Bildschirm Inaktivität.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-232">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1a5b6-233">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="1a5b6-233">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1a5b6-234">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-234">Int32</span></span>|<span data-ttu-id="1a5b6-235">Gibt die Länge des Kennwortverlauf, wobei der Benutzer nicht möglich wird ein neues Kennwort eingeben, das im Verlauf jedes beliebige Kennwort identisch ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-235">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="1a5b6-236">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1a5b6-237">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1a5b6-237">passwordRequiredType</span></span>|[<span data-ttu-id="1a5b6-238">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1a5b6-238">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1a5b6-239">Gibt die Mindestlänge für Kennwort Qualität auf dem Gerät erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-239">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="1a5b6-240">Mögliche Werte sind: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-240">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1a5b6-241">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1a5b6-241">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1a5b6-242">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-242">Int32</span></span>|<span data-ttu-id="1a5b6-243">Gibt an, wie oft ein Benutzer ein ungültiges Kennwort eingeben kann, bevor das Gerät bereinigt wird.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-243">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="1a5b6-244">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-244">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1a5b6-245">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-245">safeBootBlocked</span></span>|<span data-ttu-id="1a5b6-246">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-246">Boolean</span></span>|<span data-ttu-id="1a5b6-247">Gibt an, ob neu gestartet, dass das Gerät in abgesicherten Modus deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-247">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="1a5b6-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-248">screenCaptureBlocked</span></span>|<span data-ttu-id="1a5b6-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1a5b6-249">Boolean</span></span>|<span data-ttu-id="1a5b6-250">Gibt an, ob die Funktion auszuführende Screenshots deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-250">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="1a5b6-251">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="1a5b6-251">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="1a5b6-252">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-252">Boolean</span></span>|<span data-ttu-id="1a5b6-253">Gibt an, ob die Benutzer aus der debugging-Funktionen auf dem Gerät aktivieren blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-253">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="1a5b6-254">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1a5b6-254">securityRequireVerifyApps</span></span>|<span data-ttu-id="1a5b6-255">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1a5b6-255">Boolean</span></span>|<span data-ttu-id="1a5b6-256">Gibt an, ob überprüfen apps ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-256">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="1a5b6-257">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="1a5b6-257">statusBarBlocked</span></span>|<span data-ttu-id="1a5b6-258">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-258">Boolean</span></span>|<span data-ttu-id="1a5b6-259">Gibt an, ob oder den Status Leiste deaktiviert ist, einschließlich Benachrichtigungen, schnelle Einstellungen und anderen Bildschirm überlagert.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-259">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="1a5b6-260">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="1a5b6-260">stayOnModes</span></span>|<span data-ttu-id="1a5b6-261">[AndroidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1a5b6-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="1a5b6-262">Liste der Modi, in denen der Anzeige des Geräts eingeschaltet, verbleibt.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-262">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="1a5b6-263">Diese Sammlung kann maximal 4 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-263">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="1a5b6-264">Mögliche Werte: sind `notConfigured`, `ac`, `usb` und `wireless`.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-264">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="1a5b6-265">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="1a5b6-265">storageAllowUsb</span></span>|<span data-ttu-id="1a5b6-266">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-266">Boolean</span></span>|<span data-ttu-id="1a5b6-267">Gibt an, ob USB-Massenspeichergerät zulassen.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-267">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="1a5b6-268">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="1a5b6-268">storageBlockExternalMedia</span></span>|<span data-ttu-id="1a5b6-269">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-269">Boolean</span></span>|<span data-ttu-id="1a5b6-270">Gibt an, ob externe Medien zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-270">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="1a5b6-271">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="1a5b6-271">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="1a5b6-272">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-272">Boolean</span></span>|<span data-ttu-id="1a5b6-273">Gibt an, ob USB-Dateiübertragung zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-273">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="1a5b6-274">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="1a5b6-274">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="1a5b6-275">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-275">Int32</span></span>|<span data-ttu-id="1a5b6-276">Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster beginnt.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-276">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="1a5b6-277">Gültige Werte von 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="1a5b6-277">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1a5b6-278">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="1a5b6-278">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="1a5b6-279">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5b6-279">Int32</span></span>|<span data-ttu-id="1a5b6-280">Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster endet.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-280">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="1a5b6-281">Gültige Werte von 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="1a5b6-281">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1a5b6-282">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1a5b6-282">systemUpdateInstallType</span></span>|[<span data-ttu-id="1a5b6-283">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1a5b6-283">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="1a5b6-284">Der Typ des Systemkonfiguration Update.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-284">The type of system update configuration.</span></span> <span data-ttu-id="1a5b6-285">Mögliche Werte: sind `deviceDefault`, `postpone`, `windowed` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-285">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="1a5b6-286">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="1a5b6-286">usersBlockAdd</span></span>|<span data-ttu-id="1a5b6-287">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-287">Boolean</span></span>|<span data-ttu-id="1a5b6-288">Gibt an, ob Hinzufügen von Benutzern und Profile deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-288">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="1a5b6-289">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="1a5b6-289">usersBlockRemove</span></span>|<span data-ttu-id="1a5b6-290">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-290">Boolean</span></span>|<span data-ttu-id="1a5b6-291">Gibt an, ob Entfernen von anderen Benutzern vom Gerät zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-291">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="1a5b6-292">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="1a5b6-292">volumeBlockAdjustment</span></span>|<span data-ttu-id="1a5b6-293">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-293">Boolean</span></span>|<span data-ttu-id="1a5b6-294">Gibt an, ob anpassen, dass die Hauptlautstärke deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-294">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="1a5b6-295">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a5b6-295">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="1a5b6-296">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-296">Boolean</span></span>|<span data-ttu-id="1a5b6-297">Gibt an, ob die Benutzer durch die Bearbeitung von Einstellungen für die WLAN-Verbindung zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-297">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="1a5b6-298">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a5b6-298">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="1a5b6-299">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1a5b6-299">Boolean</span></span>|<span data-ttu-id="1a5b6-300">Gibt an, ob die Benutzer bearbeiten können nur die von der Richtlinie definierten Netzwerke blockieren.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-300">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1a5b6-301">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a5b6-301">Response</span></span>
<span data-ttu-id="1a5b6-302">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-302">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a5b6-303">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a5b6-303">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a5b6-304">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a5b6-304">Request</span></span>
<span data-ttu-id="1a5b6-305">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-305">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2073

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="1a5b6-306">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a5b6-306">Response</span></span>
<span data-ttu-id="1a5b6-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a5b6-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





