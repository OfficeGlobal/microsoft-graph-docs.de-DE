---
title: AndroidDeviceOwnerGeneralDeviceConfiguration erstellen
description: Erstellen eines neuen androidDeviceOwnerGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f82410f562d76f370e32863ed636cd3306cd4990
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964178"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="4e65e-103">AndroidDeviceOwnerGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="4e65e-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4e65e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e65e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e65e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4e65e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e65e-106">Erstellen eines neuen [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e65e-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e65e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e65e-107">Prerequisites</span></span>
<span data-ttu-id="4e65e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e65e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e65e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e65e-110">Permission type</span></span>|<span data-ttu-id="4e65e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e65e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e65e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e65e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e65e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e65e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e65e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e65e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e65e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e65e-115">Not supported.</span></span>|
|<span data-ttu-id="4e65e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e65e-116">Application</span></span>|<span data-ttu-id="4e65e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e65e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e65e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e65e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e65e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e65e-119">Request headers</span></span>
|<span data-ttu-id="4e65e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4e65e-120">Header</span></span>|<span data-ttu-id="4e65e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e65e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e65e-122">Authorization</span></span>|<span data-ttu-id="4e65e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e65e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e65e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4e65e-124">Accept</span></span>|<span data-ttu-id="4e65e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e65e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e65e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e65e-126">Request body</span></span>
<span data-ttu-id="4e65e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidDeviceOwnerGeneralDeviceConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4e65e-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4e65e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidDeviceOwnerGeneralDeviceConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4e65e-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4e65e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e65e-129">Property</span></span>|<span data-ttu-id="4e65e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4e65e-130">Type</span></span>|<span data-ttu-id="4e65e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e65e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e65e-132">id</span><span class="sxs-lookup"><span data-stu-id="4e65e-132">id</span></span>|<span data-ttu-id="4e65e-133">String</span><span class="sxs-lookup"><span data-stu-id="4e65e-133">String</span></span>|<span data-ttu-id="4e65e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4e65e-134">Key of the entity.</span></span> <span data-ttu-id="4e65e-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e65e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4e65e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e65e-137">DateTimeOffset</span></span>|<span data-ttu-id="4e65e-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e65e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4e65e-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="4e65e-140">roleScopeTagIds</span></span>|<span data-ttu-id="4e65e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4e65e-141">String collection</span></span>|<span data-ttu-id="4e65e-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="4e65e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4e65e-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4e65e-144">supportsScopeTags</span></span>|<span data-ttu-id="4e65e-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-145">Boolean</span></span>|<span data-ttu-id="4e65e-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e65e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4e65e-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="4e65e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4e65e-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="4e65e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4e65e-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e65e-149">This property is read-only.</span></span> <span data-ttu-id="4e65e-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e65e-151">createdDateTime</span></span>|<span data-ttu-id="4e65e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e65e-152">DateTimeOffset</span></span>|<span data-ttu-id="4e65e-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e65e-153">DateTime the object was created.</span></span> <span data-ttu-id="4e65e-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-155">description</span><span class="sxs-lookup"><span data-stu-id="4e65e-155">description</span></span>|<span data-ttu-id="4e65e-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e65e-156">String</span></span>|<span data-ttu-id="4e65e-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4e65e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4e65e-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4e65e-159">displayName</span></span>|<span data-ttu-id="4e65e-160">String</span><span class="sxs-lookup"><span data-stu-id="4e65e-160">String</span></span>|<span data-ttu-id="4e65e-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4e65e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4e65e-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-163">Version</span><span class="sxs-lookup"><span data-stu-id="4e65e-163">version</span></span>|<span data-ttu-id="4e65e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-164">Int32</span></span>|<span data-ttu-id="4e65e-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4e65e-165">Version of the device configuration.</span></span> <span data-ttu-id="4e65e-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e65e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e65e-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="4e65e-167">accountsBlockModification</span></span>|<span data-ttu-id="4e65e-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-168">Boolean</span></span>|<span data-ttu-id="4e65e-169">Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="4e65e-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="4e65e-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="4e65e-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-171">Boolean</span></span>|<span data-ttu-id="4e65e-172">Gibt an, ob der Benutzer die Einstellung für unbekannte Quellen aktivieren darf.</span><span class="sxs-lookup"><span data-stu-id="4e65e-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="4e65e-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="4e65e-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="4e65e-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="4e65e-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="4e65e-175">Gibt den Wert der APP-AutoUpdate-Richtlinie an.</span><span class="sxs-lookup"><span data-stu-id="4e65e-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="4e65e-176">Mögliche Werte: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="4e65e-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="4e65e-177">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="4e65e-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="4e65e-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="4e65e-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="4e65e-179">Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, wenn eine nicht speziell für die APP definiert ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="4e65e-180">Mögliche Werte sind: `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="4e65e-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="4e65e-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="4e65e-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="4e65e-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-182">Boolean</span></span>|<span data-ttu-id="4e65e-183">Ob alle apps empfohlen werden, überspringen Sie möglicherweise hinzugefügte Hinweise zum ersten Mal.</span><span class="sxs-lookup"><span data-stu-id="4e65e-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="4e65e-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e65e-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="4e65e-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-185">Boolean</span></span>|<span data-ttu-id="4e65e-186">Gibt an, ob ein Benutzer von der Konfiguration von Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="4e65e-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="4e65e-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="4e65e-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-188">Boolean</span></span>|<span data-ttu-id="4e65e-189">Gibt an, ob die Freigabe von Kontakten über Bluetooth durch einen Benutzer blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="4e65e-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-190">cameraBlocked</span></span>|<span data-ttu-id="4e65e-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-191">Boolean</span></span>|<span data-ttu-id="4e65e-192">Gibt an, ob die Verwendung der Kamera deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="4e65e-193">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4e65e-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="4e65e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e65e-194">Boolean</span></span>|<span data-ttu-id="4e65e-195">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="4e65e-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-196">dataRoamingBlocked</span></span>|<span data-ttu-id="4e65e-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-197">Boolean</span></span>|<span data-ttu-id="4e65e-198">Gibt an, ob ein Benutzer vom Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="4e65e-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="4e65e-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-200">Boolean</span></span>|<span data-ttu-id="4e65e-201">Gibt an, ob verhindert werden soll, dass der Benutzer das Datum oder die Uhrzeit auf dem Gerät manuell ändert.</span><span class="sxs-lookup"><span data-stu-id="4e65e-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="4e65e-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="4e65e-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="4e65e-203">String collection</span><span class="sxs-lookup"><span data-stu-id="4e65e-203">String collection</span></span>|<span data-ttu-id="4e65e-204">Liste der Google-Konto-e-Mails, die für die Authentifizierung erforderlich sind, nachdem ein Gerät zurückgesetzt wurde, bevor es eingerichtet werden kann.</span><span class="sxs-lookup"><span data-stu-id="4e65e-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="4e65e-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-205">factoryResetBlocked</span></span>|<span data-ttu-id="4e65e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e65e-206">Boolean</span></span>|<span data-ttu-id="4e65e-207">Gibt an, ob die Option Factory zurücksetzen in den Einstellungen deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="4e65e-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="4e65e-208">kioskModeApps</span></span>|<span data-ttu-id="4e65e-209">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4e65e-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4e65e-210">Eine Liste der verwalteten apps, die angezeigt werden, wenn sich das Gerät im Kiosk Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="4e65e-211">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4e65e-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4e65e-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="4e65e-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="4e65e-213">String</span><span class="sxs-lookup"><span data-stu-id="4e65e-213">String</span></span>|<span data-ttu-id="4e65e-214">Die URL eines öffentlich zugänglichen Bilds, das für das Hintergrundbild verwendet werden soll, wenn sich das Gerät im Kiosk Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4e65e-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="4e65e-215">kioskModeExitCode</span></span>|<span data-ttu-id="4e65e-216">String</span><span class="sxs-lookup"><span data-stu-id="4e65e-216">String</span></span>|<span data-ttu-id="4e65e-217">Beenden Sie Code, damit ein Benutzer aus dem Kioskmodus entkommen kann, wenn sich das Gerät im Kiosk-Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4e65e-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="4e65e-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="4e65e-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-219">Boolean</span></span>|<span data-ttu-id="4e65e-220">Gibt an, ob eine virtuelle Start Schaltfläche angezeigt werden soll, wenn sich das Gerät im Kiosk Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4e65e-221">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="4e65e-221">microphoneForceMute</span></span>|<span data-ttu-id="4e65e-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-222">Boolean</span></span>|<span data-ttu-id="4e65e-223">Gibt an, ob die Stummschaltung des Mikrofons auf dem Gerät blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-223">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="4e65e-224">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="4e65e-224">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="4e65e-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-225">Boolean</span></span>|<span data-ttu-id="4e65e-226">Gibt an, ob das Gerät beim Booten das Herstellen einer Verbindung mit einer temporären Netzwerkverbindung zulässt.</span><span class="sxs-lookup"><span data-stu-id="4e65e-226">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="4e65e-227">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="4e65e-227">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="4e65e-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-228">Boolean</span></span>|<span data-ttu-id="4e65e-229">Gibt an, ob NFC-ausgehender Balken blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-229">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="4e65e-230">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="4e65e-230">passwordBlockKeyguard</span></span>|<span data-ttu-id="4e65e-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-231">Boolean</span></span>|<span data-ttu-id="4e65e-232">Gibt an, ob die Tastensperre deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-232">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="4e65e-233">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="4e65e-233">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="4e65e-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e65e-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="4e65e-235">Liste der zu blockierenden Geräte-Keyguard-Features.</span><span class="sxs-lookup"><span data-stu-id="4e65e-235">List of device keyguard features to block.</span></span> <span data-ttu-id="4e65e-236">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4e65e-236">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="4e65e-237">Mögliche Werte: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="4e65e-237">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="4e65e-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4e65e-238">passwordExpirationDays</span></span>|<span data-ttu-id="4e65e-239">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-239">Int32</span></span>|<span data-ttu-id="4e65e-240">Gibt den Zeitraum in Sekunden an, für den ein Kennwort festgelegt werden kann, bevor es abläuft und ein neues Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-240">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="4e65e-241">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="4e65e-241">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4e65e-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4e65e-242">passwordMinimumLength</span></span>|<span data-ttu-id="4e65e-243">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-243">Int32</span></span>|<span data-ttu-id="4e65e-244">Gibt die minimale Länge des auf dem Gerät erforderlichen Kennworts an.</span><span class="sxs-lookup"><span data-stu-id="4e65e-244">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="4e65e-245">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="4e65e-245">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4e65e-246">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4e65e-246">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4e65e-247">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-247">Int32</span></span>|<span data-ttu-id="4e65e-248">Millisekunden der Inaktivität vor dem Timeout des Bildschirms.</span><span class="sxs-lookup"><span data-stu-id="4e65e-248">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4e65e-249">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="4e65e-249">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="4e65e-250">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-250">Int32</span></span>|<span data-ttu-id="4e65e-251">Gibt die Länge des Kennwortverlaufs an, in der der Benutzer kein neues Kennwort eingeben kann, das mit einem Kennwort im Verlauf identisch ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-251">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="4e65e-252">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="4e65e-252">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4e65e-253">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4e65e-253">passwordRequiredType</span></span>|[<span data-ttu-id="4e65e-254">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4e65e-254">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="4e65e-255">Gibt die auf dem Gerät erforderliche minimale Kenn Wort Qualität an.</span><span class="sxs-lookup"><span data-stu-id="4e65e-255">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="4e65e-256">Mögliche Werte: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="4e65e-256">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="4e65e-257">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4e65e-257">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4e65e-258">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-258">Int32</span></span>|<span data-ttu-id="4e65e-259">Gibt an, wie oft ein Benutzer ein falsches Kennwort eingeben kann, bevor das Gerät gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="4e65e-259">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="4e65e-260">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="4e65e-260">Valid values 4 to 11</span></span>|
|<span data-ttu-id="4e65e-261">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-261">safeBootBlocked</span></span>|<span data-ttu-id="4e65e-262">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-262">Boolean</span></span>|<span data-ttu-id="4e65e-263">Gibt an, ob das Gerät in den sicheren Start neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="4e65e-263">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="4e65e-264">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-264">screenCaptureBlocked</span></span>|<span data-ttu-id="4e65e-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e65e-265">Boolean</span></span>|<span data-ttu-id="4e65e-266">Gibt an, ob die Funktion zum Ausführen von Screenshots deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-266">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="4e65e-267">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="4e65e-267">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="4e65e-268">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-268">Boolean</span></span>|<span data-ttu-id="4e65e-269">Gibt an, ob verhindert werden soll, dass der Benutzer Debuggingfunktionen auf dem Gerät aktiviert.</span><span class="sxs-lookup"><span data-stu-id="4e65e-269">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="4e65e-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4e65e-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="4e65e-271">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-271">Boolean</span></span>|<span data-ttu-id="4e65e-272">Gibt an, ob apps überprüfen erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-272">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="4e65e-273">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-273">statusBarBlocked</span></span>|<span data-ttu-id="4e65e-274">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-274">Boolean</span></span>|<span data-ttu-id="4e65e-275">Gibt an, ob die Statusleiste deaktiviert ist, einschließlich Benachrichtigungen, schnell Einstellungen und anderen Bildschirm-Overlays.</span><span class="sxs-lookup"><span data-stu-id="4e65e-275">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="4e65e-276">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="4e65e-276">stayOnModes</span></span>|<span data-ttu-id="4e65e-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e65e-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="4e65e-278">Liste der Modi, in denen die Anzeige des Geräts eingeschaltet bleibt.</span><span class="sxs-lookup"><span data-stu-id="4e65e-278">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="4e65e-279">Diese Auflistung kann maximal 4 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4e65e-279">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="4e65e-280">Mögliche Werte sind: `notConfigured`, `ac`, `usb` und `wireless`.</span><span class="sxs-lookup"><span data-stu-id="4e65e-280">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="4e65e-281">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="4e65e-281">storageAllowUsb</span></span>|<span data-ttu-id="4e65e-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-282">Boolean</span></span>|<span data-ttu-id="4e65e-283">Gibt an, ob USB-Massenspeicher zugelassen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4e65e-283">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="4e65e-284">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="4e65e-284">storageBlockExternalMedia</span></span>|<span data-ttu-id="4e65e-285">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-285">Boolean</span></span>|<span data-ttu-id="4e65e-286">Gibt an, ob externe Medien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4e65e-286">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="4e65e-287">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="4e65e-287">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="4e65e-288">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-288">Boolean</span></span>|<span data-ttu-id="4e65e-289">Gibt an, ob die USB-Dateiübertragung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-289">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="4e65e-290">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="4e65e-290">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="4e65e-291">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-291">Int32</span></span>|<span data-ttu-id="4e65e-292">Gibt die Anzahl von Minuten nach Mitternacht an, die das System Aktualisierungsfenster startet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-292">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="4e65e-293">Gültige Werte 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="4e65e-293">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="4e65e-294">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="4e65e-294">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="4e65e-295">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65e-295">Int32</span></span>|<span data-ttu-id="4e65e-296">Gibt die Anzahl von Minuten nach Mitternacht an, die das System Aktualisierungsfenster beendet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-296">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="4e65e-297">Gültige Werte 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="4e65e-297">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="4e65e-298">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="4e65e-298">systemUpdateInstallType</span></span>|[<span data-ttu-id="4e65e-299">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="4e65e-299">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="4e65e-300">Der Typ der System Update Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="4e65e-300">The type of system update configuration.</span></span> <span data-ttu-id="4e65e-301">Mögliche Werte sind: `deviceDefault`, `postpone`, `windowed` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4e65e-301">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="4e65e-302">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="4e65e-302">systemWindowsBlocked</span></span>|<span data-ttu-id="4e65e-303">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-303">Boolean</span></span>|<span data-ttu-id="4e65e-304">Gibt an, ob Android-Systemansage Fenster wie Toasts, Telefonaktivitäten und System Warnungen blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4e65e-304">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="4e65e-305">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="4e65e-305">usersBlockAdd</span></span>|<span data-ttu-id="4e65e-306">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-306">Boolean</span></span>|<span data-ttu-id="4e65e-307">Gibt an, ob das Hinzufügen von Benutzern und Profilen deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-307">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="4e65e-308">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="4e65e-308">usersBlockRemove</span></span>|<span data-ttu-id="4e65e-309">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-309">Boolean</span></span>|<span data-ttu-id="4e65e-310">Gibt an, ob das Entfernen anderer Benutzer vom Gerät deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-310">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="4e65e-311">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="4e65e-311">volumeBlockAdjustment</span></span>|<span data-ttu-id="4e65e-312">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-312">Boolean</span></span>|<span data-ttu-id="4e65e-313">Gibt an, ob die Master Lautstärke deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4e65e-313">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="4e65e-314">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="4e65e-314">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="4e65e-315">String</span><span class="sxs-lookup"><span data-stu-id="4e65e-315">String</span></span>|<span data-ttu-id="4e65e-316">Android-App-Paket Name für die APP, die eine Always-on-VPN-Verbindung verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-316">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="4e65e-317">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="4e65e-317">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="4e65e-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-318">Boolean</span></span>|<span data-ttu-id="4e65e-319">Wenn ein Name des Always-on-VPN-Pakets angegeben wird, unabhängig davon, ob der Netzwerkdatenverkehr beim Trennen der Verbindung mit dem VPN gesperrt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4e65e-319">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="4e65e-320">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="4e65e-320">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="4e65e-321">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-321">Boolean</span></span>|<span data-ttu-id="4e65e-322">Gibt an, ob verhindert werden soll, dass der Benutzer die Einstellungen für die WLAN-Verbindung bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-322">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="4e65e-323">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="4e65e-323">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="4e65e-324">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4e65e-324">Boolean</span></span>|<span data-ttu-id="4e65e-325">Gibt an, ob verhindert werden soll, dass der Benutzer nur die von der Richtlinie definierten Netzwerke bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="4e65e-325">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="4e65e-326">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e65e-326">Response</span></span>
<span data-ttu-id="4e65e-327">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4e65e-327">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e65e-328">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e65e-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e65e-329">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e65e-329">Request</span></span>
<span data-ttu-id="4e65e-330">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e65e-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2517

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "appsRecommendSkippingFirstUseHints": true,
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
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
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
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="4e65e-331">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e65e-331">Response</span></span>
<span data-ttu-id="4e65e-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e65e-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2689

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
  "appsRecommendSkippingFirstUseHints": true,
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
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
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
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




