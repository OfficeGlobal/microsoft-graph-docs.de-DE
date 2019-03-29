---
title: Erstellen von „androidGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f529c74d841daff02c508cd50db888f6d4a4f958
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976449"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="6bdb6-103">Erstellen von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="6bdb6-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6bdb6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bdb6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bdb6-106">Diese Methode erstellt ein neues Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bdb6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6bdb6-107">Prerequisites</span></span>
<span data-ttu-id="6bdb6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bdb6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6bdb6-110">Permission type</span></span>|<span data-ttu-id="6bdb6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bdb6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6bdb6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bdb6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bdb6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bdb6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bdb6-115">Not supported.</span></span>|
|<span data-ttu-id="6bdb6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6bdb6-116">Application</span></span>|<span data-ttu-id="6bdb6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6bdb6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bdb6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bdb6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6bdb6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6bdb6-119">Request headers</span></span>
|<span data-ttu-id="6bdb6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6bdb6-120">Header</span></span>|<span data-ttu-id="6bdb6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bdb6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bdb6-122">Authorization</span></span>|<span data-ttu-id="6bdb6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6bdb6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bdb6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6bdb6-124">Accept</span></span>|<span data-ttu-id="6bdb6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6bdb6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bdb6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6bdb6-126">Request body</span></span>
<span data-ttu-id="6bdb6-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="6bdb6-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="6bdb6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6bdb6-129">Property</span></span>|<span data-ttu-id="6bdb6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6bdb6-130">Type</span></span>|<span data-ttu-id="6bdb6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bdb6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bdb6-132">id</span><span class="sxs-lookup"><span data-stu-id="6bdb6-132">id</span></span>|<span data-ttu-id="6bdb6-133">String</span><span class="sxs-lookup"><span data-stu-id="6bdb6-133">String</span></span>|<span data-ttu-id="6bdb6-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6bdb6-134">Key of the entity.</span></span> <span data-ttu-id="6bdb6-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdb6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6bdb6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bdb6-137">DateTimeOffset</span></span>|<span data-ttu-id="6bdb6-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6bdb6-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="6bdb6-140">roleScopeTagIds</span></span>|<span data-ttu-id="6bdb6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6bdb6-141">String collection</span></span>|<span data-ttu-id="6bdb6-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6bdb6-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6bdb6-144">supportsScopeTags</span></span>|<span data-ttu-id="6bdb6-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-145">Boolean</span></span>|<span data-ttu-id="6bdb6-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6bdb6-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6bdb6-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6bdb6-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-149">This property is read-only.</span></span> <span data-ttu-id="6bdb6-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdb6-151">createdDateTime</span></span>|<span data-ttu-id="6bdb6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bdb6-152">DateTimeOffset</span></span>|<span data-ttu-id="6bdb6-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-153">DateTime the object was created.</span></span> <span data-ttu-id="6bdb6-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-155">description</span><span class="sxs-lookup"><span data-stu-id="6bdb6-155">description</span></span>|<span data-ttu-id="6bdb6-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6bdb6-156">String</span></span>|<span data-ttu-id="6bdb6-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bdb6-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6bdb6-159">displayName</span></span>|<span data-ttu-id="6bdb6-160">String</span><span class="sxs-lookup"><span data-stu-id="6bdb6-160">String</span></span>|<span data-ttu-id="6bdb6-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bdb6-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-163">Version</span><span class="sxs-lookup"><span data-stu-id="6bdb6-163">version</span></span>|<span data-ttu-id="6bdb6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdb6-164">Int32</span></span>|<span data-ttu-id="6bdb6-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-165">Version of the device configuration.</span></span> <span data-ttu-id="6bdb6-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdb6-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="6bdb6-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="6bdb6-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-168">Boolean</span></span>|<span data-ttu-id="6bdb6-169">Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="6bdb6-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="6bdb6-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="6bdb6-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-171">Boolean</span></span>|<span data-ttu-id="6bdb6-172">Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="6bdb6-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="6bdb6-173">appsBlockYouTube</span></span>|<span data-ttu-id="6bdb6-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-174">Boolean</span></span>|<span data-ttu-id="6bdb6-175">Gibt an, ob die YouTube-App blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="6bdb6-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-176">bluetoothBlocked</span></span>|<span data-ttu-id="6bdb6-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-177">Boolean</span></span>|<span data-ttu-id="6bdb6-178">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="6bdb6-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-179">cameraBlocked</span></span>|<span data-ttu-id="6bdb6-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-180">Boolean</span></span>|<span data-ttu-id="6bdb6-181">Gibt an, ob die Verwendung der Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="6bdb6-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="6bdb6-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="6bdb6-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-183">Boolean</span></span>|<span data-ttu-id="6bdb6-184">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="6bdb6-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="6bdb6-185">cellularBlockMessaging</span></span>|<span data-ttu-id="6bdb6-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-186">Boolean</span></span>|<span data-ttu-id="6bdb6-187">Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="6bdb6-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="6bdb6-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="6bdb6-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-189">Boolean</span></span>|<span data-ttu-id="6bdb6-190">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="6bdb6-191">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="6bdb6-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="6bdb6-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-192">Boolean</span></span>|<span data-ttu-id="6bdb6-193">Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="6bdb6-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6bdb6-194">compliantAppsList</span></span>|<span data-ttu-id="6bdb6-195">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6bdb6-196">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="6bdb6-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6bdb6-197">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6bdb6-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6bdb6-198">compliantAppListType</span></span>|[<span data-ttu-id="6bdb6-199">appListType</span><span class="sxs-lookup"><span data-stu-id="6bdb6-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6bdb6-200">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="6bdb6-201">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6bdb6-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="6bdb6-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="6bdb6-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-203">Boolean</span></span>|<span data-ttu-id="6bdb6-204">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="6bdb6-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-205">locationServicesBlocked</span></span>|<span data-ttu-id="6bdb6-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-206">Boolean</span></span>|<span data-ttu-id="6bdb6-207">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="6bdb6-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="6bdb6-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="6bdb6-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-209">Boolean</span></span>|<span data-ttu-id="6bdb6-210">Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="6bdb6-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="6bdb6-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-212">Boolean</span></span>|<span data-ttu-id="6bdb6-213">Gibt an, ob der Google Play-Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="6bdb6-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="6bdb6-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="6bdb6-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-215">Boolean</span></span>|<span data-ttu-id="6bdb6-216">Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="6bdb6-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="6bdb6-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="6bdb6-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bdb6-218">Boolean</span></span>|<span data-ttu-id="6bdb6-219">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="6bdb6-220">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="6bdb6-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="6bdb6-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-221">Boolean</span></span>|<span data-ttu-id="6bdb6-222">Gibt an, ob das Ändern von Datum und Uhrzeit im KNOX-Modus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="6bdb6-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="6bdb6-223">kioskModeApps</span></span>|<span data-ttu-id="6bdb6-224">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6bdb6-225">Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="6bdb6-226">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bdb6-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-227">nfcBlocked</span></span>|<span data-ttu-id="6bdb6-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-228">Boolean</span></span>|<span data-ttu-id="6bdb6-229">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="6bdb6-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6bdb6-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6bdb6-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-231">Boolean</span></span>|<span data-ttu-id="6bdb6-232">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6bdb6-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6bdb6-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="6bdb6-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-234">Boolean</span></span>|<span data-ttu-id="6bdb6-235">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6bdb6-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6bdb6-236">passwordExpirationDays</span></span>|<span data-ttu-id="6bdb6-237">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdb6-237">Int32</span></span>|<span data-ttu-id="6bdb6-238">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-238">Number of days before the password expires.</span></span> <span data-ttu-id="6bdb6-239">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6bdb6-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6bdb6-240">passwordMinimumLength</span></span>|<span data-ttu-id="6bdb6-241">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdb6-241">Int32</span></span>|<span data-ttu-id="6bdb6-242">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="6bdb6-242">Minimum length of passwords.</span></span> <span data-ttu-id="6bdb6-243">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6bdb6-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6bdb6-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6bdb6-245">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdb6-245">Int32</span></span>|<span data-ttu-id="6bdb6-246">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6bdb6-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6bdb6-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6bdb6-248">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdb6-248">Int32</span></span>|<span data-ttu-id="6bdb6-249">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-249">Number of previous passwords to block.</span></span> <span data-ttu-id="6bdb6-250">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6bdb6-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6bdb6-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6bdb6-252">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdb6-252">Int32</span></span>|<span data-ttu-id="6bdb6-253">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="6bdb6-254">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="6bdb6-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6bdb6-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6bdb6-255">passwordRequiredType</span></span>|[<span data-ttu-id="6bdb6-256">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6bdb6-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="6bdb6-257">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-257">Type of password that is required.</span></span> <span data-ttu-id="6bdb6-258">Mögliche Werte: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="6bdb6-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6bdb6-259">passwordRequired</span></span>|<span data-ttu-id="6bdb6-260">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-260">Boolean</span></span>|<span data-ttu-id="6bdb6-261">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="6bdb6-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-262">powerOffBlocked</span></span>|<span data-ttu-id="6bdb6-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-263">Boolean</span></span>|<span data-ttu-id="6bdb6-264">Gibt an, ob das Ausschalten des Geräts blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="6bdb6-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-265">factoryResetBlocked</span></span>|<span data-ttu-id="6bdb6-266">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-266">Boolean</span></span>|<span data-ttu-id="6bdb6-267">Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="6bdb6-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-268">screenCaptureBlocked</span></span>|<span data-ttu-id="6bdb6-269">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-269">Boolean</span></span>|<span data-ttu-id="6bdb6-270">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="6bdb6-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="6bdb6-271">deviceSharingAllowed</span></span>|<span data-ttu-id="6bdb6-272">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-272">Boolean</span></span>|<span data-ttu-id="6bdb6-273">Gibt an, ob der Gerätefreigabemodus zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="6bdb6-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="6bdb6-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="6bdb6-275">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-275">Boolean</span></span>|<span data-ttu-id="6bdb6-276">Gibt an, ob die Google-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="6bdb6-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="6bdb6-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="6bdb6-278">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-278">Boolean</span></span>|<span data-ttu-id="6bdb6-279">Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="6bdb6-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="6bdb6-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="6bdb6-281">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-281">Boolean</span></span>|<span data-ttu-id="6bdb6-282">Gibt an, ob eine Geräteverschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="6bdb6-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="6bdb6-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="6bdb6-284">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-284">Boolean</span></span>|<span data-ttu-id="6bdb6-285">Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="6bdb6-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="6bdb6-287">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-287">Boolean</span></span>|<span data-ttu-id="6bdb6-288">Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="6bdb6-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-289">voiceDialingBlocked</span></span>|<span data-ttu-id="6bdb6-290">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-290">Boolean</span></span>|<span data-ttu-id="6bdb6-291">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="6bdb6-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="6bdb6-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="6bdb6-293">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-293">Boolean</span></span>|<span data-ttu-id="6bdb6-294">Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="6bdb6-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6bdb6-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="6bdb6-296">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-296">Boolean</span></span>|<span data-ttu-id="6bdb6-297">Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="6bdb6-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="6bdb6-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="6bdb6-299">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-299">Boolean</span></span>|<span data-ttu-id="6bdb6-300">Gibt an, ob JavaScript im Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="6bdb6-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-301">webBrowserBlocked</span></span>|<span data-ttu-id="6bdb6-302">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6bdb6-302">Boolean</span></span>|<span data-ttu-id="6bdb6-303">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="6bdb6-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6bdb6-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="6bdb6-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6bdb6-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="6bdb6-306">Cookieeinstellungen des Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="6bdb6-307">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="6bdb6-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="6bdb6-308">wiFiBlocked</span></span>|<span data-ttu-id="6bdb6-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bdb6-309">Boolean</span></span>|<span data-ttu-id="6bdb6-310">Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="6bdb6-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="6bdb6-311">appsInstallAllowList</span></span>|<span data-ttu-id="6bdb6-312">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6bdb6-313">Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="6bdb6-314">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bdb6-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="6bdb6-315">appsLaunchBlockList</span></span>|<span data-ttu-id="6bdb6-316">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6bdb6-317">Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="6bdb6-318">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bdb6-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="6bdb6-319">appsHideList</span></span>|<span data-ttu-id="6bdb6-320">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb6-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6bdb6-321">Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="6bdb6-322">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bdb6-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6bdb6-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="6bdb6-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bdb6-324">Boolean</span></span>|<span data-ttu-id="6bdb6-325">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="6bdb6-326">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bdb6-326">Response</span></span>
<span data-ttu-id="6bdb6-327">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-327">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bdb6-328">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6bdb6-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bdb6-329">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6bdb6-329">Request</span></span>
<span data-ttu-id="6bdb6-330">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6bdb6-331">Antwort</span><span class="sxs-lookup"><span data-stu-id="6bdb6-331">Response</span></span>
<span data-ttu-id="6bdb6-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6bdb6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




