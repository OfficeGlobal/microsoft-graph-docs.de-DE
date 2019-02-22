---
title: AndroidDeviceOwnerGeneralDeviceConfiguration erstellen
description: Erstellen eines neuen androidDeviceOwnerGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e05e696b0a2c127abdc8c365829599777f55beae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143092"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="f904d-103">AndroidDeviceOwnerGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="f904d-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f904d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f904d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f904d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f904d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f904d-106">Erstellen eines neuen [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f904d-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f904d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f904d-107">Prerequisites</span></span>
<span data-ttu-id="f904d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f904d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f904d-110">Permission type</span></span>|<span data-ttu-id="f904d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f904d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f904d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f904d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f904d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f904d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f904d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f904d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f904d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f904d-115">Not supported.</span></span>|
|<span data-ttu-id="f904d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f904d-116">Application</span></span>|<span data-ttu-id="f904d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f904d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f904d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f904d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f904d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f904d-119">Request headers</span></span>
|<span data-ttu-id="f904d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f904d-120">Header</span></span>|<span data-ttu-id="f904d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f904d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f904d-122">Authorization</span></span>|<span data-ttu-id="f904d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f904d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f904d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f904d-124">Accept</span></span>|<span data-ttu-id="f904d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f904d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f904d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f904d-126">Request body</span></span>
<span data-ttu-id="f904d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidDeviceOwnerGeneralDeviceConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f904d-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f904d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidDeviceOwnerGeneralDeviceConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f904d-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f904d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f904d-129">Property</span></span>|<span data-ttu-id="f904d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f904d-130">Type</span></span>|<span data-ttu-id="f904d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f904d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f904d-132">id</span><span class="sxs-lookup"><span data-stu-id="f904d-132">id</span></span>|<span data-ttu-id="f904d-133">string</span><span class="sxs-lookup"><span data-stu-id="f904d-133">String</span></span>|<span data-ttu-id="f904d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f904d-134">Key of the entity.</span></span> <span data-ttu-id="f904d-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f904d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f904d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f904d-137">DateTimeOffset</span></span>|<span data-ttu-id="f904d-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f904d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f904d-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="f904d-140">roleScopeTagIds</span></span>|<span data-ttu-id="f904d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f904d-141">String collection</span></span>|<span data-ttu-id="f904d-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="f904d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f904d-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f904d-144">supportsScopeTags</span></span>|<span data-ttu-id="f904d-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-145">Boolean</span></span>|<span data-ttu-id="f904d-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f904d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f904d-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="f904d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f904d-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f904d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f904d-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f904d-149">This property is read-only.</span></span> <span data-ttu-id="f904d-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f904d-151">createdDateTime</span></span>|<span data-ttu-id="f904d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f904d-152">DateTimeOffset</span></span>|<span data-ttu-id="f904d-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f904d-153">DateTime the object was created.</span></span> <span data-ttu-id="f904d-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-155">description</span><span class="sxs-lookup"><span data-stu-id="f904d-155">description</span></span>|<span data-ttu-id="f904d-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f904d-156">String</span></span>|<span data-ttu-id="f904d-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f904d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f904d-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f904d-159">displayName</span></span>|<span data-ttu-id="f904d-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f904d-160">String</span></span>|<span data-ttu-id="f904d-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f904d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f904d-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-163">Version</span><span class="sxs-lookup"><span data-stu-id="f904d-163">version</span></span>|<span data-ttu-id="f904d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-164">Int32</span></span>|<span data-ttu-id="f904d-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f904d-165">Version of the device configuration.</span></span> <span data-ttu-id="f904d-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f904d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f904d-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="f904d-167">accountsBlockModification</span></span>|<span data-ttu-id="f904d-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-168">Boolean</span></span>|<span data-ttu-id="f904d-169">Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="f904d-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f904d-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="f904d-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-171">Boolean</span></span>|<span data-ttu-id="f904d-172">Gibt an, ob der Benutzer die Einstellung für unbekannte Quellen aktivieren darf.</span><span class="sxs-lookup"><span data-stu-id="f904d-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="f904d-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="f904d-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="f904d-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="f904d-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="f904d-175">Gibt den Wert der APP-AutoUpdate-Richtlinie an.</span><span class="sxs-lookup"><span data-stu-id="f904d-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="f904d-176">Mögliche Werte: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="f904d-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="f904d-177">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="f904d-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="f904d-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="f904d-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="f904d-179">Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, wenn eine nicht speziell für die APP definiert ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="f904d-180">Mögliche Werte: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="f904d-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="f904d-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="f904d-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="f904d-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-182">Boolean</span></span>|<span data-ttu-id="f904d-183">Ob alle apps empfohlen werden, überspringen Sie möglicherweise hinzugefügte Hinweise zum ersten Mal.</span><span class="sxs-lookup"><span data-stu-id="f904d-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="f904d-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="f904d-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="f904d-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-185">Boolean</span></span>|<span data-ttu-id="f904d-186">Gibt an, ob ein Benutzer von der Konfiguration von Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="f904d-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="f904d-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="f904d-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-188">Boolean</span></span>|<span data-ttu-id="f904d-189">Gibt an, ob die Freigabe von Kontakten über Bluetooth durch einen Benutzer blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="f904d-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-190">cameraBlocked</span></span>|<span data-ttu-id="f904d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f904d-191">Boolean</span></span>|<span data-ttu-id="f904d-192">Gibt an, ob die Verwendung der Kamera deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="f904d-193">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="f904d-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="f904d-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-194">Boolean</span></span>|<span data-ttu-id="f904d-195">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="f904d-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-196">dataRoamingBlocked</span></span>|<span data-ttu-id="f904d-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-197">Boolean</span></span>|<span data-ttu-id="f904d-198">Gibt an, ob ein Benutzer vom Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="f904d-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="f904d-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-200">Boolean</span></span>|<span data-ttu-id="f904d-201">Gibt an, ob verhindert werden soll, dass der Benutzer das Datum oder die Uhrzeit auf dem Gerät manuell ändert.</span><span class="sxs-lookup"><span data-stu-id="f904d-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="f904d-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="f904d-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="f904d-203">String collection</span><span class="sxs-lookup"><span data-stu-id="f904d-203">String collection</span></span>|<span data-ttu-id="f904d-204">Liste der Google-Konto-e-Mails, die für die Authentifizierung erforderlich sind, nachdem ein Gerät zurückgesetzt wurde, bevor es eingerichtet werden kann.</span><span class="sxs-lookup"><span data-stu-id="f904d-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="f904d-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-205">factoryResetBlocked</span></span>|<span data-ttu-id="f904d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f904d-206">Boolean</span></span>|<span data-ttu-id="f904d-207">Gibt an, ob die Option Factory zurücksetzen in den Einstellungen deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="f904d-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="f904d-208">kioskModeApps</span></span>|<span data-ttu-id="f904d-209">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f904d-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f904d-210">Eine Liste der verwalteten apps, die angezeigt werden, wenn sich das Gerät im Kiosk Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="f904d-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="f904d-211">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f904d-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f904d-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="f904d-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="f904d-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f904d-213">String</span></span>|<span data-ttu-id="f904d-214">Die URL eines öffentlich zugänglichen Bilds, das für das Hintergrundbild verwendet werden soll, wenn sich das Gerät im Kiosk Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="f904d-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="f904d-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="f904d-215">kioskModeExitCode</span></span>|<span data-ttu-id="f904d-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f904d-216">String</span></span>|<span data-ttu-id="f904d-217">Beenden Sie Code, damit ein Benutzer aus dem Kioskmodus entkommen kann, wenn sich das Gerät im Kiosk-Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="f904d-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="f904d-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="f904d-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="f904d-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-219">Boolean</span></span>|<span data-ttu-id="f904d-220">Gibt an, ob eine virtuelle Start Schaltfläche angezeigt werden soll, wenn sich das Gerät im Kiosk Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="f904d-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="f904d-221">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="f904d-221">microphoneForceMute</span></span>|<span data-ttu-id="f904d-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-222">Boolean</span></span>|<span data-ttu-id="f904d-223">Gibt an, ob die Stummschaltung des Mikrofons auf dem Gerät blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-223">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="f904d-224">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="f904d-224">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="f904d-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-225">Boolean</span></span>|<span data-ttu-id="f904d-226">Gibt an, ob das Gerät beim Booten das Herstellen einer Verbindung mit einer temporären Netzwerkverbindung zulässt.</span><span class="sxs-lookup"><span data-stu-id="f904d-226">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="f904d-227">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="f904d-227">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="f904d-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-228">Boolean</span></span>|<span data-ttu-id="f904d-229">Gibt an, ob NFC-ausgehender Balken blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-229">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="f904d-230">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="f904d-230">passwordBlockKeyguard</span></span>|<span data-ttu-id="f904d-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-231">Boolean</span></span>|<span data-ttu-id="f904d-232">Gibt an, ob die Tastensperre deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-232">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="f904d-233">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="f904d-233">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="f904d-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f904d-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="f904d-235">Liste der zu blockierenden Geräte-Keyguard-Features.</span><span class="sxs-lookup"><span data-stu-id="f904d-235">List of device keyguard features to block.</span></span> <span data-ttu-id="f904d-236">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f904d-236">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="f904d-237">Mögliche Werte sind: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput` und `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="f904d-237">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="f904d-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f904d-238">passwordExpirationDays</span></span>|<span data-ttu-id="f904d-239">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-239">Int32</span></span>|<span data-ttu-id="f904d-240">Gibt den Zeitraum in Sekunden an, für den ein Kennwort festgelegt werden kann, bevor es abläuft und ein neues Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-240">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="f904d-241">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="f904d-241">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f904d-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f904d-242">passwordMinimumLength</span></span>|<span data-ttu-id="f904d-243">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-243">Int32</span></span>|<span data-ttu-id="f904d-244">Gibt die minimale Länge des auf dem Gerät erforderlichen Kennworts an.</span><span class="sxs-lookup"><span data-stu-id="f904d-244">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="f904d-245">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="f904d-245">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f904d-246">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f904d-246">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f904d-247">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-247">Int32</span></span>|<span data-ttu-id="f904d-248">Millisekunden der Inaktivität vor dem Timeout des Bildschirms.</span><span class="sxs-lookup"><span data-stu-id="f904d-248">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f904d-249">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="f904d-249">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="f904d-250">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-250">Int32</span></span>|<span data-ttu-id="f904d-251">Gibt die Länge des Kennwortverlaufs an, in der der Benutzer kein neues Kennwort eingeben kann, das mit einem Kennwort im Verlauf identisch ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-251">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="f904d-252">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="f904d-252">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f904d-253">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f904d-253">passwordRequiredType</span></span>|[<span data-ttu-id="f904d-254">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f904d-254">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="f904d-255">Gibt die auf dem Gerät erforderliche minimale Kenn Wort Qualität an.</span><span class="sxs-lookup"><span data-stu-id="f904d-255">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="f904d-256">Mögliche Werte sind: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="f904d-256">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f904d-257">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f904d-257">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f904d-258">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-258">Int32</span></span>|<span data-ttu-id="f904d-259">Gibt an, wie oft ein Benutzer ein falsches Kennwort eingeben kann, bevor das Gerät gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="f904d-259">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="f904d-260">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="f904d-260">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f904d-261">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-261">safeBootBlocked</span></span>|<span data-ttu-id="f904d-262">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-262">Boolean</span></span>|<span data-ttu-id="f904d-263">Gibt an, ob das Gerät in den sicheren Start neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="f904d-263">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="f904d-264">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-264">screenCaptureBlocked</span></span>|<span data-ttu-id="f904d-265">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-265">Boolean</span></span>|<span data-ttu-id="f904d-266">Gibt an, ob die Funktion zum Ausführen von Screenshots deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-266">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="f904d-267">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="f904d-267">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="f904d-268">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-268">Boolean</span></span>|<span data-ttu-id="f904d-269">Gibt an, ob verhindert werden soll, dass der Benutzer Debuggingfunktionen auf dem Gerät aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f904d-269">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="f904d-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f904d-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="f904d-271">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-271">Boolean</span></span>|<span data-ttu-id="f904d-272">Gibt an, ob apps überprüfen erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-272">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="f904d-273">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-273">statusBarBlocked</span></span>|<span data-ttu-id="f904d-274">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-274">Boolean</span></span>|<span data-ttu-id="f904d-275">Gibt an, ob die Statusleiste deaktiviert ist, einschließlich Benachrichtigungen, schnell Einstellungen und anderen Bildschirm-Overlays.</span><span class="sxs-lookup"><span data-stu-id="f904d-275">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="f904d-276">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="f904d-276">stayOnModes</span></span>|<span data-ttu-id="f904d-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f904d-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="f904d-278">Liste der Modi, in denen die Anzeige des Geräts eingeschaltet bleibt.</span><span class="sxs-lookup"><span data-stu-id="f904d-278">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="f904d-279">Diese Auflistung kann maximal 4 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f904d-279">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="f904d-280">Mögliche Werte: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="f904d-280">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="f904d-281">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="f904d-281">storageAllowUsb</span></span>|<span data-ttu-id="f904d-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-282">Boolean</span></span>|<span data-ttu-id="f904d-283">Gibt an, ob USB-Massenspeicher zugelassen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f904d-283">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="f904d-284">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="f904d-284">storageBlockExternalMedia</span></span>|<span data-ttu-id="f904d-285">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-285">Boolean</span></span>|<span data-ttu-id="f904d-286">Gibt an, ob externe Medien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f904d-286">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="f904d-287">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f904d-287">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="f904d-288">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-288">Boolean</span></span>|<span data-ttu-id="f904d-289">Gibt an, ob die USB-Dateiübertragung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-289">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="f904d-290">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="f904d-290">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="f904d-291">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-291">Int32</span></span>|<span data-ttu-id="f904d-292">Gibt die Anzahl von Minuten nach Mitternacht an, die das System Aktualisierungsfenster startet.</span><span class="sxs-lookup"><span data-stu-id="f904d-292">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="f904d-293">Gültige Werte 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="f904d-293">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="f904d-294">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="f904d-294">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="f904d-295">Int32</span><span class="sxs-lookup"><span data-stu-id="f904d-295">Int32</span></span>|<span data-ttu-id="f904d-296">Gibt die Anzahl von Minuten nach Mitternacht an, die das System Aktualisierungsfenster beendet.</span><span class="sxs-lookup"><span data-stu-id="f904d-296">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="f904d-297">Gültige Werte 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="f904d-297">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="f904d-298">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="f904d-298">systemUpdateInstallType</span></span>|[<span data-ttu-id="f904d-299">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="f904d-299">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="f904d-300">Der Typ der System Update Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="f904d-300">The type of system update configuration.</span></span> <span data-ttu-id="f904d-301">Mögliche Werte: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f904d-301">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="f904d-302">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="f904d-302">systemWindowsBlocked</span></span>|<span data-ttu-id="f904d-303">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-303">Boolean</span></span>|<span data-ttu-id="f904d-304">Gibt an, ob Android-Systemansage Fenster wie Toasts, Telefonaktivitäten und System Warnungen blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f904d-304">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="f904d-305">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="f904d-305">usersBlockAdd</span></span>|<span data-ttu-id="f904d-306">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-306">Boolean</span></span>|<span data-ttu-id="f904d-307">Gibt an, ob das Hinzufügen von Benutzern und Profilen deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-307">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="f904d-308">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="f904d-308">usersBlockRemove</span></span>|<span data-ttu-id="f904d-309">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-309">Boolean</span></span>|<span data-ttu-id="f904d-310">Gibt an, ob das Entfernen anderer Benutzer vom Gerät deaktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-310">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="f904d-311">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="f904d-311">volumeBlockAdjustment</span></span>|<span data-ttu-id="f904d-312">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-312">Boolean</span></span>|<span data-ttu-id="f904d-313">Gibt an, ob die Master Lautstärke deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f904d-313">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="f904d-314">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="f904d-314">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="f904d-315">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f904d-315">String</span></span>|<span data-ttu-id="f904d-316">Android-App-Paket Name für die APP, die eine Always-on-VPN-Verbindung verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="f904d-316">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="f904d-317">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="f904d-317">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="f904d-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-318">Boolean</span></span>|<span data-ttu-id="f904d-319">Wenn ein Name des Always-on-VPN-Pakets angegeben wird, unabhängig davon, ob der Netzwerkdatenverkehr beim Trennen der Verbindung mit dem VPN gesperrt werden soll.</span><span class="sxs-lookup"><span data-stu-id="f904d-319">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="f904d-320">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="f904d-320">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="f904d-321">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-321">Boolean</span></span>|<span data-ttu-id="f904d-322">Gibt an, ob verhindert werden soll, dass der Benutzer die Einstellungen für die WLAN-Verbindung bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="f904d-322">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="f904d-323">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="f904d-323">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="f904d-324">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f904d-324">Boolean</span></span>|<span data-ttu-id="f904d-325">Gibt an, ob verhindert werden soll, dass der Benutzer nur die von der Richtlinie definierten Netzwerke bearbeitet.</span><span class="sxs-lookup"><span data-stu-id="f904d-325">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f904d-326">Antwort</span><span class="sxs-lookup"><span data-stu-id="f904d-326">Response</span></span>
<span data-ttu-id="f904d-327">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f904d-327">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f904d-328">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f904d-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="f904d-329">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f904d-329">Request</span></span>
<span data-ttu-id="f904d-330">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f904d-330">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f904d-331">Antwort</span><span class="sxs-lookup"><span data-stu-id="f904d-331">Response</span></span>
<span data-ttu-id="f904d-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f904d-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




