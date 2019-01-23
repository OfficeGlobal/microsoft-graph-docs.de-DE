---
title: Erstellen von androidDeviceOwnerGeneralDeviceConfiguration
description: Erstellen eines neuen AndroidDeviceOwnerGeneralDeviceConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93df53db7c19df9134370f9dbd703d99f631b688
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421221"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="263fe-103">Erstellen von androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="263fe-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="263fe-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="263fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="263fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="263fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="263fe-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="263fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="263fe-107">Erstellen eines neuen [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="263fe-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="263fe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="263fe-108">Prerequisites</span></span>
<span data-ttu-id="263fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="263fe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="263fe-111">Permission type</span></span>|<span data-ttu-id="263fe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="263fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="263fe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="263fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="263fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="263fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="263fe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="263fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="263fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="263fe-116">Not supported.</span></span>|
|<span data-ttu-id="263fe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="263fe-117">Application</span></span>|<span data-ttu-id="263fe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="263fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="263fe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="263fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="263fe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="263fe-120">Request headers</span></span>
|<span data-ttu-id="263fe-121">Header</span><span class="sxs-lookup"><span data-stu-id="263fe-121">Header</span></span>|<span data-ttu-id="263fe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="263fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="263fe-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="263fe-123">Authorization</span></span>|<span data-ttu-id="263fe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="263fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="263fe-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="263fe-125">Accept</span></span>|<span data-ttu-id="263fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="263fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="263fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="263fe-127">Request body</span></span>
<span data-ttu-id="263fe-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidDeviceOwnerGeneralDeviceConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="263fe-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="263fe-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidDeviceOwnerGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="263fe-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="263fe-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="263fe-130">Property</span></span>|<span data-ttu-id="263fe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="263fe-131">Type</span></span>|<span data-ttu-id="263fe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="263fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="263fe-133">id</span><span class="sxs-lookup"><span data-stu-id="263fe-133">id</span></span>|<span data-ttu-id="263fe-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263fe-134">String</span></span>|<span data-ttu-id="263fe-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="263fe-135">Key of the entity.</span></span> <span data-ttu-id="263fe-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="263fe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="263fe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="263fe-138">DateTimeOffset</span></span>|<span data-ttu-id="263fe-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="263fe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="263fe-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="263fe-141">roleScopeTagIds</span></span>|<span data-ttu-id="263fe-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="263fe-142">String collection</span></span>|<span data-ttu-id="263fe-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="263fe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="263fe-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="263fe-145">supportsScopeTags</span></span>|<span data-ttu-id="263fe-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-146">Boolean</span></span>|<span data-ttu-id="263fe-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="263fe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="263fe-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="263fe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="263fe-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="263fe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="263fe-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="263fe-150">This property is read-only.</span></span> <span data-ttu-id="263fe-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="263fe-152">createdDateTime</span></span>|<span data-ttu-id="263fe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="263fe-153">DateTimeOffset</span></span>|<span data-ttu-id="263fe-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="263fe-154">DateTime the object was created.</span></span> <span data-ttu-id="263fe-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-156">description</span><span class="sxs-lookup"><span data-stu-id="263fe-156">description</span></span>|<span data-ttu-id="263fe-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263fe-157">String</span></span>|<span data-ttu-id="263fe-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="263fe-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="263fe-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-160">displayName</span><span class="sxs-lookup"><span data-stu-id="263fe-160">displayName</span></span>|<span data-ttu-id="263fe-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263fe-161">String</span></span>|<span data-ttu-id="263fe-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="263fe-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="263fe-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-164">Version</span><span class="sxs-lookup"><span data-stu-id="263fe-164">version</span></span>|<span data-ttu-id="263fe-165">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-165">Int32</span></span>|<span data-ttu-id="263fe-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="263fe-166">Version of the device configuration.</span></span> <span data-ttu-id="263fe-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="263fe-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="263fe-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="263fe-168">accountsBlockModification</span></span>|<span data-ttu-id="263fe-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-169">Boolean</span></span>|<span data-ttu-id="263fe-170">Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="263fe-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="263fe-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="263fe-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-172">Boolean</span></span>|<span data-ttu-id="263fe-173">Gibt an, ob der Benutzer berechtigt ist, um das Festlegen von unbekannten Quellen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="263fe-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="263fe-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="263fe-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="263fe-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="263fe-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="263fe-176">Gibt den Wert des app-Richtlinie für die automatische Aktualisierung.</span><span class="sxs-lookup"><span data-stu-id="263fe-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="263fe-177">Mögliche Werte sind: `notConfigured`, `userChoice`, `never`, `wiFiOnly` und `always`.</span><span class="sxs-lookup"><span data-stu-id="263fe-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="263fe-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="263fe-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="263fe-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="263fe-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="263fe-180">Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, ob eine nicht für die app speziell definiert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="263fe-181">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="263fe-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="263fe-182">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="263fe-182">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="263fe-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-183">Boolean</span></span>|<span data-ttu-id="263fe-184">Ob alle apps empfehlen überspringen Hinweise ersten Mal verwenden, die sie möglicherweise hinzugefügt haben.</span><span class="sxs-lookup"><span data-stu-id="263fe-184">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="263fe-185">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="263fe-185">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="263fe-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-186">Boolean</span></span>|<span data-ttu-id="263fe-187">Gibt an, ob vom Bluetooth konfigurieren einen Benutzer blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-187">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="263fe-188">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="263fe-188">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="263fe-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-189">Boolean</span></span>|<span data-ttu-id="263fe-190">Gibt an, ob einen Benutzer von der Freigabe von Kontakten über Bluetooth blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-190">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="263fe-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-191">cameraBlocked</span></span>|<span data-ttu-id="263fe-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-192">Boolean</span></span>|<span data-ttu-id="263fe-193">Gibt an, ob die Verwendung der Kamera zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-193">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="263fe-194">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="263fe-194">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="263fe-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-195">Boolean</span></span>|<span data-ttu-id="263fe-196">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="263fe-196">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="263fe-197">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-197">dataRoamingBlocked</span></span>|<span data-ttu-id="263fe-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-198">Boolean</span></span>|<span data-ttu-id="263fe-199">Gibt an, ob einen Benutzer von servergespeicherten Daten blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-199">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="263fe-200">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-200">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="263fe-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-201">Boolean</span></span>|<span data-ttu-id="263fe-202">Gibt an, ob die Benutzer manuell ändern, die Datums- oder Uhrzeitwerte auf dem Gerät blockieren</span><span class="sxs-lookup"><span data-stu-id="263fe-202">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="263fe-203">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="263fe-203">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="263fe-204">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="263fe-204">String collection</span></span>|<span data-ttu-id="263fe-205">Liste der Google-Konto-e-Mails, die erforderlich sind, um zu authentifizieren, nachdem ein Gerät ist Factory zurückzusetzen, bevor eingerichtet werden kann.</span><span class="sxs-lookup"><span data-stu-id="263fe-205">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="263fe-206">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-206">factoryResetBlocked</span></span>|<span data-ttu-id="263fe-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-207">Boolean</span></span>|<span data-ttu-id="263fe-208">Gibt an, ob die Option zum Factory in den Einstellungen deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-208">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="263fe-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="263fe-209">kioskModeApps</span></span>|<span data-ttu-id="263fe-210">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="263fe-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="263fe-211">Eine Liste der verwalteten apps, die das Gerät bei im Kioskmodus zurückgekehrt ist angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="263fe-211">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="263fe-212">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="263fe-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="263fe-213">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="263fe-213">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="263fe-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263fe-214">String</span></span>|<span data-ttu-id="263fe-215">URL zu einem öffentlich zugänglichen Bild für den Hintergrund verwenden, wenn das Gerät im Kioskmodus zurückgekehrt ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-215">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="263fe-216">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="263fe-216">kioskModeExitCode</span></span>|<span data-ttu-id="263fe-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263fe-217">String</span></span>|<span data-ttu-id="263fe-218">Beenden Sie Code, damit der Benutzer von Kioskmodus Escapezeichen, wenn das Gerät im Kioskmodus zurückgekehrt ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-218">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="263fe-219">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="263fe-219">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="263fe-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-220">Boolean</span></span>|<span data-ttu-id="263fe-221">Ob Sie eine virtuelle private Schaltfläche angezeigt wird, wenn das Gerät im Kioskmodus zurückgekehrt ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-221">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="263fe-222">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="263fe-222">microphoneForceMute</span></span>|<span data-ttu-id="263fe-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-223">Boolean</span></span>|<span data-ttu-id="263fe-224">Gibt an, ob blockieren Aufheben der stummschaltung für das Mikrofon auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="263fe-224">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="263fe-225">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="263fe-225">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="263fe-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-226">Boolean</span></span>|<span data-ttu-id="263fe-227">Gibt an, ob das Gerät zulässig, eine Verbindung mit einer temporären-Verbindung beim Starten.</span><span class="sxs-lookup"><span data-stu-id="263fe-227">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="263fe-228">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="263fe-228">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="263fe-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-229">Boolean</span></span>|<span data-ttu-id="263fe-230">Gibt an, ob ausgehende Balken NFK blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-230">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="263fe-231">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="263fe-231">passwordBlockKeyguard</span></span>|<span data-ttu-id="263fe-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-232">Boolean</span></span>|<span data-ttu-id="263fe-233">Gibt an, ob die Keyguard deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-233">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="263fe-234">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="263fe-234">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="263fe-235">[AndroidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="263fe-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="263fe-236">Liste der Features des Geräts Keyguard blockiert.</span><span class="sxs-lookup"><span data-stu-id="263fe-236">List of device keyguard features to block.</span></span> <span data-ttu-id="263fe-237">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="263fe-237">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="263fe-238">Mögliche Werte sind: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput` und `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="263fe-238">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="263fe-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="263fe-239">passwordExpirationDays</span></span>|<span data-ttu-id="263fe-240">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-240">Int32</span></span>|<span data-ttu-id="263fe-241">Gibt die Zeitspanne in Sekunden an, die für ein Kennwort festgelegt werden kann, bevor sie abläuft und ein neues Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="263fe-241">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="263fe-242">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="263fe-242">Valid values 1 to 365</span></span>|
|<span data-ttu-id="263fe-243">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="263fe-243">passwordMinimumLength</span></span>|<span data-ttu-id="263fe-244">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-244">Int32</span></span>|<span data-ttu-id="263fe-245">Gibt die minimale Länge des Kennworts auf dem Gerät erforderlich.</span><span class="sxs-lookup"><span data-stu-id="263fe-245">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="263fe-246">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="263fe-246">Valid values 4 to 16</span></span>|
|<span data-ttu-id="263fe-247">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="263fe-247">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="263fe-248">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-248">Int32</span></span>|<span data-ttu-id="263fe-249">Zeit in Millisekunden vor dem Timeout der Bildschirm Inaktivität.</span><span class="sxs-lookup"><span data-stu-id="263fe-249">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="263fe-250">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="263fe-250">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="263fe-251">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-251">Int32</span></span>|<span data-ttu-id="263fe-252">Gibt die Länge des Kennwortverlauf, wobei der Benutzer nicht möglich wird ein neues Kennwort eingeben, das im Verlauf jedes beliebige Kennwort identisch ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-252">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="263fe-253">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="263fe-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="263fe-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="263fe-254">passwordRequiredType</span></span>|[<span data-ttu-id="263fe-255">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="263fe-255">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="263fe-256">Gibt die Mindestlänge für Kennwort Qualität auf dem Gerät erforderlich.</span><span class="sxs-lookup"><span data-stu-id="263fe-256">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="263fe-257">Mögliche Werte sind: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="263fe-257">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="263fe-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="263fe-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="263fe-259">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-259">Int32</span></span>|<span data-ttu-id="263fe-260">Gibt an, wie oft ein Benutzer ein ungültiges Kennwort eingeben kann, bevor das Gerät bereinigt wird.</span><span class="sxs-lookup"><span data-stu-id="263fe-260">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="263fe-261">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="263fe-261">Valid values 4 to 11</span></span>|
|<span data-ttu-id="263fe-262">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-262">safeBootBlocked</span></span>|<span data-ttu-id="263fe-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-263">Boolean</span></span>|<span data-ttu-id="263fe-264">Gibt an, ob neu gestartet, dass das Gerät in abgesicherten Modus deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-264">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="263fe-265">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-265">screenCaptureBlocked</span></span>|<span data-ttu-id="263fe-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-266">Boolean</span></span>|<span data-ttu-id="263fe-267">Gibt an, ob die Funktion auszuführende Screenshots deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-267">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="263fe-268">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="263fe-268">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="263fe-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-269">Boolean</span></span>|<span data-ttu-id="263fe-270">Gibt an, ob die Benutzer aus der debugging-Funktionen auf dem Gerät aktivieren blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-270">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="263fe-271">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="263fe-271">securityRequireVerifyApps</span></span>|<span data-ttu-id="263fe-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-272">Boolean</span></span>|<span data-ttu-id="263fe-273">Gibt an, ob überprüfen apps ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="263fe-273">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="263fe-274">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-274">statusBarBlocked</span></span>|<span data-ttu-id="263fe-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-275">Boolean</span></span>|<span data-ttu-id="263fe-276">Gibt an, ob oder den Status Leiste deaktiviert ist, einschließlich Benachrichtigungen, schnelle Einstellungen und anderen Bildschirm überlagert.</span><span class="sxs-lookup"><span data-stu-id="263fe-276">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="263fe-277">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="263fe-277">stayOnModes</span></span>|<span data-ttu-id="263fe-278">[AndroidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="263fe-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="263fe-279">Liste der Modi, in denen der Anzeige des Geräts eingeschaltet, verbleibt.</span><span class="sxs-lookup"><span data-stu-id="263fe-279">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="263fe-280">Diese Sammlung kann maximal 4 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="263fe-280">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="263fe-281">Mögliche Werte: sind `notConfigured`, `ac`, `usb` und `wireless`.</span><span class="sxs-lookup"><span data-stu-id="263fe-281">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="263fe-282">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="263fe-282">storageAllowUsb</span></span>|<span data-ttu-id="263fe-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-283">Boolean</span></span>|<span data-ttu-id="263fe-284">Gibt an, ob USB-Massenspeichergerät zulassen.</span><span class="sxs-lookup"><span data-stu-id="263fe-284">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="263fe-285">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="263fe-285">storageBlockExternalMedia</span></span>|<span data-ttu-id="263fe-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-286">Boolean</span></span>|<span data-ttu-id="263fe-287">Gibt an, ob externe Medien zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-287">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="263fe-288">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="263fe-288">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="263fe-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-289">Boolean</span></span>|<span data-ttu-id="263fe-290">Gibt an, ob USB-Dateiübertragung zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-290">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="263fe-291">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="263fe-291">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="263fe-292">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-292">Int32</span></span>|<span data-ttu-id="263fe-293">Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster beginnt.</span><span class="sxs-lookup"><span data-stu-id="263fe-293">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="263fe-294">Gültige Werte von 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="263fe-294">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="263fe-295">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="263fe-295">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="263fe-296">Int32</span><span class="sxs-lookup"><span data-stu-id="263fe-296">Int32</span></span>|<span data-ttu-id="263fe-297">Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster endet.</span><span class="sxs-lookup"><span data-stu-id="263fe-297">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="263fe-298">Gültige Werte von 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="263fe-298">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="263fe-299">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="263fe-299">systemUpdateInstallType</span></span>|[<span data-ttu-id="263fe-300">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="263fe-300">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="263fe-301">Der Typ des Systemkonfiguration Update.</span><span class="sxs-lookup"><span data-stu-id="263fe-301">The type of system update configuration.</span></span> <span data-ttu-id="263fe-302">Mögliche Werte: sind `deviceDefault`, `postpone`, `windowed` und `automatic`.</span><span class="sxs-lookup"><span data-stu-id="263fe-302">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="263fe-303">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="263fe-303">systemWindowsBlocked</span></span>|<span data-ttu-id="263fe-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-304">Boolean</span></span>|<span data-ttu-id="263fe-305">Ob Android System blockieren auffordern, Windows, wie Popups, Telefon Aktivitäten und System-Benachrichtigungen.</span><span class="sxs-lookup"><span data-stu-id="263fe-305">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="263fe-306">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="263fe-306">usersBlockAdd</span></span>|<span data-ttu-id="263fe-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-307">Boolean</span></span>|<span data-ttu-id="263fe-308">Gibt an, ob Hinzufügen von Benutzern und Profile deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-308">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="263fe-309">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="263fe-309">usersBlockRemove</span></span>|<span data-ttu-id="263fe-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-310">Boolean</span></span>|<span data-ttu-id="263fe-311">Gibt an, ob Entfernen von anderen Benutzern vom Gerät zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-311">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="263fe-312">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="263fe-312">volumeBlockAdjustment</span></span>|<span data-ttu-id="263fe-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-313">Boolean</span></span>|<span data-ttu-id="263fe-314">Gibt an, ob anpassen, dass die Hauptlautstärke deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="263fe-314">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="263fe-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="263fe-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="263fe-316">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263fe-316">String</span></span>|<span data-ttu-id="263fe-317">Android-app-Paket-Name für die app, die eine VPN-Verbindung immer auf behandelt.</span><span class="sxs-lookup"><span data-stu-id="263fe-317">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="263fe-318">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="263fe-318">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="263fe-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-319">Boolean</span></span>|<span data-ttu-id="263fe-320">Wenn ein immer auf VPN Packen Sie Name werden, unabhängig davon, ob angegeben Netzwerkverkehr sperren, wenn diese VPN getrennt wird.</span><span class="sxs-lookup"><span data-stu-id="263fe-320">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="263fe-321">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="263fe-321">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="263fe-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-322">Boolean</span></span>|<span data-ttu-id="263fe-323">Gibt an, ob die Benutzer durch die Bearbeitung von Einstellungen für die WLAN-Verbindung zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-323">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="263fe-324">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="263fe-324">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="263fe-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="263fe-325">Boolean</span></span>|<span data-ttu-id="263fe-326">Gibt an, ob die Benutzer bearbeiten können nur die von der Richtlinie definierten Netzwerke blockieren.</span><span class="sxs-lookup"><span data-stu-id="263fe-326">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="263fe-327">Antwort</span><span class="sxs-lookup"><span data-stu-id="263fe-327">Response</span></span>
<span data-ttu-id="263fe-328">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="263fe-328">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263fe-329">Beispiel</span><span class="sxs-lookup"><span data-stu-id="263fe-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="263fe-330">Anforderung</span><span class="sxs-lookup"><span data-stu-id="263fe-330">Request</span></span>
<span data-ttu-id="263fe-331">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="263fe-331">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="263fe-332">Antwort</span><span class="sxs-lookup"><span data-stu-id="263fe-332">Response</span></span>
<span data-ttu-id="263fe-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="263fe-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




