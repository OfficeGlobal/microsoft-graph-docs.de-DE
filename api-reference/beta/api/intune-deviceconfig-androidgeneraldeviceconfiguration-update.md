---
title: Aktualisieren von „androidGeneralDeviceConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a96b820670ee86fb425f128d964382df951e70b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143764"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="9426c-103">Aktualisieren von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="9426c-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="9426c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9426c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9426c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9426c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9426c-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9426c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9426c-107">Prerequisites</span></span>
<span data-ttu-id="9426c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9426c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9426c-110">Permission type</span></span>|<span data-ttu-id="9426c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9426c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9426c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9426c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9426c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9426c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9426c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9426c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9426c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9426c-115">Not supported.</span></span>|
|<span data-ttu-id="9426c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9426c-116">Application</span></span>|<span data-ttu-id="9426c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9426c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9426c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9426c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9426c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9426c-119">Request headers</span></span>
|<span data-ttu-id="9426c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9426c-120">Header</span></span>|<span data-ttu-id="9426c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9426c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9426c-122">Authorization</span></span>|<span data-ttu-id="9426c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9426c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9426c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9426c-124">Accept</span></span>|<span data-ttu-id="9426c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9426c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9426c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9426c-126">Request body</span></span>
<span data-ttu-id="9426c-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="9426c-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="9426c-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9426c-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="9426c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9426c-129">Property</span></span>|<span data-ttu-id="9426c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9426c-130">Type</span></span>|<span data-ttu-id="9426c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9426c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9426c-132">id</span><span class="sxs-lookup"><span data-stu-id="9426c-132">id</span></span>|<span data-ttu-id="9426c-133">string</span><span class="sxs-lookup"><span data-stu-id="9426c-133">String</span></span>|<span data-ttu-id="9426c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9426c-134">Key of the entity.</span></span> <span data-ttu-id="9426c-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9426c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9426c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9426c-137">DateTimeOffset</span></span>|<span data-ttu-id="9426c-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9426c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9426c-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="9426c-140">roleScopeTagIds</span></span>|<span data-ttu-id="9426c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9426c-141">String collection</span></span>|<span data-ttu-id="9426c-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="9426c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9426c-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9426c-144">supportsScopeTags</span></span>|<span data-ttu-id="9426c-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-145">Boolean</span></span>|<span data-ttu-id="9426c-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9426c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9426c-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="9426c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9426c-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9426c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9426c-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9426c-149">This property is read-only.</span></span> <span data-ttu-id="9426c-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9426c-151">createdDateTime</span></span>|<span data-ttu-id="9426c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9426c-152">DateTimeOffset</span></span>|<span data-ttu-id="9426c-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9426c-153">DateTime the object was created.</span></span> <span data-ttu-id="9426c-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-155">description</span><span class="sxs-lookup"><span data-stu-id="9426c-155">description</span></span>|<span data-ttu-id="9426c-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9426c-156">String</span></span>|<span data-ttu-id="9426c-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9426c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9426c-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9426c-159">displayName</span></span>|<span data-ttu-id="9426c-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9426c-160">String</span></span>|<span data-ttu-id="9426c-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9426c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9426c-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9426c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-163">Version</span><span class="sxs-lookup"><span data-stu-id="9426c-163">version</span></span>|<span data-ttu-id="9426c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9426c-164">Int32</span></span>|<span data-ttu-id="9426c-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9426c-165">Version of the device configuration.</span></span> <span data-ttu-id="9426c-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9426c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9426c-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="9426c-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="9426c-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-168">Boolean</span></span>|<span data-ttu-id="9426c-169">Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="9426c-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="9426c-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="9426c-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-171">Boolean</span></span>|<span data-ttu-id="9426c-172">Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="9426c-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="9426c-173">appsBlockYouTube</span></span>|<span data-ttu-id="9426c-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-174">Boolean</span></span>|<span data-ttu-id="9426c-175">Gibt an, ob die YouTube-App blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="9426c-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-176">bluetoothBlocked</span></span>|<span data-ttu-id="9426c-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="9426c-177">Boolean</span></span>|<span data-ttu-id="9426c-178">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="9426c-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-179">cameraBlocked</span></span>|<span data-ttu-id="9426c-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-180">Boolean</span></span>|<span data-ttu-id="9426c-181">Gibt an, ob die Verwendung der Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="9426c-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="9426c-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="9426c-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-183">Boolean</span></span>|<span data-ttu-id="9426c-184">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="9426c-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="9426c-185">cellularBlockMessaging</span></span>|<span data-ttu-id="9426c-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="9426c-186">Boolean</span></span>|<span data-ttu-id="9426c-187">Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="9426c-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="9426c-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="9426c-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-189">Boolean</span></span>|<span data-ttu-id="9426c-190">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="9426c-191">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="9426c-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="9426c-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-192">Boolean</span></span>|<span data-ttu-id="9426c-193">Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="9426c-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="9426c-194">compliantAppsList</span></span>|<span data-ttu-id="9426c-195">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9426c-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9426c-196">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="9426c-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="9426c-197">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9426c-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9426c-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="9426c-198">compliantAppListType</span></span>|[<span data-ttu-id="9426c-199">appListType</span><span class="sxs-lookup"><span data-stu-id="9426c-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9426c-200">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="9426c-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="9426c-201">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="9426c-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9426c-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="9426c-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="9426c-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-203">Boolean</span></span>|<span data-ttu-id="9426c-204">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9426c-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-205">locationServicesBlocked</span></span>|<span data-ttu-id="9426c-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9426c-206">Boolean</span></span>|<span data-ttu-id="9426c-207">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="9426c-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="9426c-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="9426c-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-209">Boolean</span></span>|<span data-ttu-id="9426c-210">Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="9426c-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="9426c-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-212">Boolean</span></span>|<span data-ttu-id="9426c-213">Gibt an, ob der Google Play-Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="9426c-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="9426c-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="9426c-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-215">Boolean</span></span>|<span data-ttu-id="9426c-216">Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="9426c-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="9426c-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="9426c-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-218">Boolean</span></span>|<span data-ttu-id="9426c-219">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="9426c-220">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="9426c-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="9426c-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-221">Boolean</span></span>|<span data-ttu-id="9426c-222">Gibt an, ob das Ändern von Datum und Uhrzeit im KNOX-Modus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="9426c-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="9426c-223">kioskModeApps</span></span>|<span data-ttu-id="9426c-224">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9426c-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9426c-225">Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="9426c-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="9426c-226">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9426c-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9426c-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-227">nfcBlocked</span></span>|<span data-ttu-id="9426c-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-228">Boolean</span></span>|<span data-ttu-id="9426c-229">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="9426c-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="9426c-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="9426c-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-231">Boolean</span></span>|<span data-ttu-id="9426c-232">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="9426c-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="9426c-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="9426c-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-234">Boolean</span></span>|<span data-ttu-id="9426c-235">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="9426c-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9426c-236">passwordExpirationDays</span></span>|<span data-ttu-id="9426c-237">Int32</span><span class="sxs-lookup"><span data-stu-id="9426c-237">Int32</span></span>|<span data-ttu-id="9426c-238">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="9426c-238">Number of days before the password expires.</span></span> <span data-ttu-id="9426c-239">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="9426c-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9426c-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9426c-240">passwordMinimumLength</span></span>|<span data-ttu-id="9426c-241">Int32</span><span class="sxs-lookup"><span data-stu-id="9426c-241">Int32</span></span>|<span data-ttu-id="9426c-242">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="9426c-242">Minimum length of passwords.</span></span> <span data-ttu-id="9426c-243">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="9426c-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9426c-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9426c-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9426c-245">Int32</span><span class="sxs-lookup"><span data-stu-id="9426c-245">Int32</span></span>|<span data-ttu-id="9426c-246">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="9426c-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9426c-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9426c-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9426c-248">Int32</span><span class="sxs-lookup"><span data-stu-id="9426c-248">Int32</span></span>|<span data-ttu-id="9426c-249">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="9426c-249">Number of previous passwords to block.</span></span> <span data-ttu-id="9426c-250">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="9426c-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9426c-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9426c-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9426c-252">Int32</span><span class="sxs-lookup"><span data-stu-id="9426c-252">Int32</span></span>|<span data-ttu-id="9426c-253">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9426c-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="9426c-254">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="9426c-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9426c-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9426c-255">passwordRequiredType</span></span>|[<span data-ttu-id="9426c-256">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9426c-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="9426c-257">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="9426c-257">Type of password that is required.</span></span> <span data-ttu-id="9426c-258">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="9426c-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="9426c-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9426c-259">passwordRequired</span></span>|<span data-ttu-id="9426c-260">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-260">Boolean</span></span>|<span data-ttu-id="9426c-261">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9426c-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="9426c-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-262">powerOffBlocked</span></span>|<span data-ttu-id="9426c-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-263">Boolean</span></span>|<span data-ttu-id="9426c-264">Gibt an, ob das Ausschalten des Geräts blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="9426c-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-265">factoryResetBlocked</span></span>|<span data-ttu-id="9426c-266">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-266">Boolean</span></span>|<span data-ttu-id="9426c-267">Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.</span><span class="sxs-lookup"><span data-stu-id="9426c-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="9426c-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-268">screenCaptureBlocked</span></span>|<span data-ttu-id="9426c-269">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-269">Boolean</span></span>|<span data-ttu-id="9426c-270">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="9426c-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="9426c-271">deviceSharingAllowed</span></span>|<span data-ttu-id="9426c-272">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-272">Boolean</span></span>|<span data-ttu-id="9426c-273">Gibt an, ob der Gerätefreigabemodus zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="9426c-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="9426c-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="9426c-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="9426c-275">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-275">Boolean</span></span>|<span data-ttu-id="9426c-276">Gibt an, ob die Google-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="9426c-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="9426c-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="9426c-278">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-278">Boolean</span></span>|<span data-ttu-id="9426c-279">Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="9426c-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="9426c-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="9426c-281">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-281">Boolean</span></span>|<span data-ttu-id="9426c-282">Gibt an, ob eine Geräteverschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9426c-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="9426c-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="9426c-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="9426c-284">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-284">Boolean</span></span>|<span data-ttu-id="9426c-285">Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9426c-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="9426c-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="9426c-287">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-287">Boolean</span></span>|<span data-ttu-id="9426c-288">Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="9426c-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-289">voiceDialingBlocked</span></span>|<span data-ttu-id="9426c-290">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-290">Boolean</span></span>|<span data-ttu-id="9426c-291">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="9426c-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="9426c-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="9426c-293">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-293">Boolean</span></span>|<span data-ttu-id="9426c-294">Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="9426c-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="9426c-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="9426c-296">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-296">Boolean</span></span>|<span data-ttu-id="9426c-297">Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="9426c-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="9426c-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="9426c-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="9426c-299">Boolean</span></span>|<span data-ttu-id="9426c-300">Gibt an, ob JavaScript im Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="9426c-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-301">webBrowserBlocked</span></span>|<span data-ttu-id="9426c-302">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-302">Boolean</span></span>|<span data-ttu-id="9426c-303">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="9426c-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9426c-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="9426c-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9426c-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="9426c-306">Cookieeinstellungen des Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="9426c-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="9426c-307">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="9426c-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="9426c-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="9426c-308">wiFiBlocked</span></span>|<span data-ttu-id="9426c-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="9426c-309">Boolean</span></span>|<span data-ttu-id="9426c-310">Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9426c-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="9426c-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="9426c-311">appsInstallAllowList</span></span>|<span data-ttu-id="9426c-312">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9426c-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9426c-313">Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="9426c-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="9426c-314">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9426c-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9426c-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="9426c-315">appsLaunchBlockList</span></span>|<span data-ttu-id="9426c-316">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9426c-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9426c-317">Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="9426c-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="9426c-318">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9426c-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9426c-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="9426c-319">appsHideList</span></span>|<span data-ttu-id="9426c-320">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9426c-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9426c-321">Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9426c-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="9426c-322">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9426c-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9426c-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="9426c-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="9426c-324">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9426c-324">Boolean</span></span>|<span data-ttu-id="9426c-325">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="9426c-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="9426c-326">Antwort</span><span class="sxs-lookup"><span data-stu-id="9426c-326">Response</span></span>
<span data-ttu-id="9426c-327">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9426c-327">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9426c-328">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9426c-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="9426c-329">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9426c-329">Request</span></span>
<span data-ttu-id="9426c-330">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9426c-330">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3161

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="9426c-331">Antwort</span><span class="sxs-lookup"><span data-stu-id="9426c-331">Response</span></span>
<span data-ttu-id="9426c-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9426c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```




