---
title: Erstellen von „androidGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 779b93ce25eb9fe5044a166a78ac7d02ab77201c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842441"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="bf02b-103">Erstellen von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="bf02b-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="bf02b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf02b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf02b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf02b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bf02b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf02b-107">Diese Methode erstellt ein neues Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-107">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf02b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bf02b-108">Prerequisites</span></span>
<span data-ttu-id="bf02b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf02b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf02b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf02b-111">Permission type</span></span>|<span data-ttu-id="bf02b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf02b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf02b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf02b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf02b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf02b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf02b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf02b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf02b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf02b-116">Not supported.</span></span>|
|<span data-ttu-id="bf02b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf02b-117">Application</span></span>|<span data-ttu-id="bf02b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf02b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf02b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf02b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bf02b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf02b-120">Request headers</span></span>
|<span data-ttu-id="bf02b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bf02b-121">Header</span></span>|<span data-ttu-id="bf02b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bf02b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf02b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf02b-123">Authorization</span></span>|<span data-ttu-id="bf02b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bf02b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf02b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bf02b-125">Accept</span></span>|<span data-ttu-id="bf02b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf02b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf02b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf02b-127">Request body</span></span>
<span data-ttu-id="bf02b-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="bf02b-128">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="bf02b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-129">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="bf02b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf02b-130">Property</span></span>|<span data-ttu-id="bf02b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bf02b-131">Type</span></span>|<span data-ttu-id="bf02b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf02b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf02b-133">id</span><span class="sxs-lookup"><span data-stu-id="bf02b-133">id</span></span>|<span data-ttu-id="bf02b-134">String</span><span class="sxs-lookup"><span data-stu-id="bf02b-134">String</span></span>|<span data-ttu-id="bf02b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bf02b-135">Key of the entity.</span></span> <span data-ttu-id="bf02b-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf02b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bf02b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf02b-138">DateTimeOffset</span></span>|<span data-ttu-id="bf02b-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bf02b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bf02b-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bf02b-141">roleScopeTagIds</span></span>|<span data-ttu-id="bf02b-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="bf02b-142">String collection</span></span>|<span data-ttu-id="bf02b-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="bf02b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bf02b-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bf02b-145">supportsScopeTags</span></span>|<span data-ttu-id="bf02b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-146">Boolean</span></span>|<span data-ttu-id="bf02b-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf02b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bf02b-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="bf02b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bf02b-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="bf02b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bf02b-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bf02b-150">This property is read-only.</span></span> <span data-ttu-id="bf02b-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf02b-152">createdDateTime</span></span>|<span data-ttu-id="bf02b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf02b-153">DateTimeOffset</span></span>|<span data-ttu-id="bf02b-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bf02b-154">DateTime the object was created.</span></span> <span data-ttu-id="bf02b-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-156">description</span><span class="sxs-lookup"><span data-stu-id="bf02b-156">description</span></span>|<span data-ttu-id="bf02b-157">String</span><span class="sxs-lookup"><span data-stu-id="bf02b-157">String</span></span>|<span data-ttu-id="bf02b-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bf02b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bf02b-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bf02b-160">displayName</span></span>|<span data-ttu-id="bf02b-161">String</span><span class="sxs-lookup"><span data-stu-id="bf02b-161">String</span></span>|<span data-ttu-id="bf02b-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bf02b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bf02b-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-164">Version</span><span class="sxs-lookup"><span data-stu-id="bf02b-164">version</span></span>|<span data-ttu-id="bf02b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bf02b-165">Int32</span></span>|<span data-ttu-id="bf02b-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bf02b-166">Version of the device configuration.</span></span> <span data-ttu-id="bf02b-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf02b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf02b-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="bf02b-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="bf02b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-169">Boolean</span></span>|<span data-ttu-id="bf02b-170">Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="bf02b-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="bf02b-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="bf02b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-172">Boolean</span></span>|<span data-ttu-id="bf02b-173">Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="bf02b-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="bf02b-174">appsBlockYouTube</span></span>|<span data-ttu-id="bf02b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-175">Boolean</span></span>|<span data-ttu-id="bf02b-176">Gibt an, ob die YouTube-App blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="bf02b-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-177">bluetoothBlocked</span></span>|<span data-ttu-id="bf02b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-178">Boolean</span></span>|<span data-ttu-id="bf02b-179">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="bf02b-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-180">cameraBlocked</span></span>|<span data-ttu-id="bf02b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-181">Boolean</span></span>|<span data-ttu-id="bf02b-182">Gibt an, ob die Verwendung der Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="bf02b-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="bf02b-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="bf02b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-184">Boolean</span></span>|<span data-ttu-id="bf02b-185">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="bf02b-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="bf02b-186">cellularBlockMessaging</span></span>|<span data-ttu-id="bf02b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-187">Boolean</span></span>|<span data-ttu-id="bf02b-188">Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="bf02b-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="bf02b-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="bf02b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-190">Boolean</span></span>|<span data-ttu-id="bf02b-191">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="bf02b-192">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="bf02b-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="bf02b-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-193">Boolean</span></span>|<span data-ttu-id="bf02b-194">Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="bf02b-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="bf02b-195">compliantAppsList</span></span>|<span data-ttu-id="bf02b-196">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bf02b-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bf02b-197">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="bf02b-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="bf02b-198">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bf02b-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bf02b-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="bf02b-199">compliantAppListType</span></span>|[<span data-ttu-id="bf02b-200">appListType</span><span class="sxs-lookup"><span data-stu-id="bf02b-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="bf02b-201">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="bf02b-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="bf02b-202">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="bf02b-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="bf02b-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="bf02b-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="bf02b-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-204">Boolean</span></span>|<span data-ttu-id="bf02b-205">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="bf02b-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-206">locationServicesBlocked</span></span>|<span data-ttu-id="bf02b-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-207">Boolean</span></span>|<span data-ttu-id="bf02b-208">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="bf02b-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="bf02b-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="bf02b-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-210">Boolean</span></span>|<span data-ttu-id="bf02b-211">Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="bf02b-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="bf02b-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-213">Boolean</span></span>|<span data-ttu-id="bf02b-214">Gibt an, ob der Google Play-Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="bf02b-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="bf02b-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="bf02b-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-216">Boolean</span></span>|<span data-ttu-id="bf02b-217">Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="bf02b-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="bf02b-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="bf02b-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-219">Boolean</span></span>|<span data-ttu-id="bf02b-220">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="bf02b-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="bf02b-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="bf02b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-222">Boolean</span></span>|<span data-ttu-id="bf02b-223">Gibt an, ob veränderbaren Datum und Uhrzeit im Modus KNOX blockieren.</span><span class="sxs-lookup"><span data-stu-id="bf02b-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="bf02b-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="bf02b-224">kioskModeApps</span></span>|<span data-ttu-id="bf02b-225">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bf02b-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bf02b-226">Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="bf02b-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="bf02b-227">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bf02b-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bf02b-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-228">nfcBlocked</span></span>|<span data-ttu-id="bf02b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-229">Boolean</span></span>|<span data-ttu-id="bf02b-230">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="bf02b-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="bf02b-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="bf02b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-232">Boolean</span></span>|<span data-ttu-id="bf02b-233">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="bf02b-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="bf02b-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="bf02b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-235">Boolean</span></span>|<span data-ttu-id="bf02b-236">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="bf02b-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bf02b-237">passwordExpirationDays</span></span>|<span data-ttu-id="bf02b-238">Int32</span><span class="sxs-lookup"><span data-stu-id="bf02b-238">Int32</span></span>|<span data-ttu-id="bf02b-239">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="bf02b-239">Number of days before the password expires.</span></span> <span data-ttu-id="bf02b-240">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="bf02b-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bf02b-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bf02b-241">passwordMinimumLength</span></span>|<span data-ttu-id="bf02b-242">Int32</span><span class="sxs-lookup"><span data-stu-id="bf02b-242">Int32</span></span>|<span data-ttu-id="bf02b-243">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="bf02b-243">Minimum length of passwords.</span></span> <span data-ttu-id="bf02b-244">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="bf02b-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bf02b-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bf02b-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bf02b-246">Int32</span><span class="sxs-lookup"><span data-stu-id="bf02b-246">Int32</span></span>|<span data-ttu-id="bf02b-247">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="bf02b-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bf02b-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bf02b-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bf02b-249">Int32</span><span class="sxs-lookup"><span data-stu-id="bf02b-249">Int32</span></span>|<span data-ttu-id="bf02b-250">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-250">Number of previous passwords to block.</span></span> <span data-ttu-id="bf02b-251">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="bf02b-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bf02b-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bf02b-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bf02b-253">Int32</span><span class="sxs-lookup"><span data-stu-id="bf02b-253">Int32</span></span>|<span data-ttu-id="bf02b-254">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="bf02b-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="bf02b-255">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="bf02b-255">Valid values 4 to 11</span></span>|
|<span data-ttu-id="bf02b-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bf02b-256">passwordRequiredType</span></span>|[<span data-ttu-id="bf02b-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bf02b-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="bf02b-258">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="bf02b-258">Type of password that is required.</span></span> <span data-ttu-id="bf02b-259">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="bf02b-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="bf02b-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bf02b-260">passwordRequired</span></span>|<span data-ttu-id="bf02b-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-261">Boolean</span></span>|<span data-ttu-id="bf02b-262">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bf02b-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="bf02b-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-263">powerOffBlocked</span></span>|<span data-ttu-id="bf02b-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-264">Boolean</span></span>|<span data-ttu-id="bf02b-265">Gibt an, ob das Ausschalten des Geräts blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="bf02b-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-266">factoryResetBlocked</span></span>|<span data-ttu-id="bf02b-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-267">Boolean</span></span>|<span data-ttu-id="bf02b-268">Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.</span><span class="sxs-lookup"><span data-stu-id="bf02b-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="bf02b-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-269">screenCaptureBlocked</span></span>|<span data-ttu-id="bf02b-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-270">Boolean</span></span>|<span data-ttu-id="bf02b-271">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="bf02b-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="bf02b-272">deviceSharingAllowed</span></span>|<span data-ttu-id="bf02b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-273">Boolean</span></span>|<span data-ttu-id="bf02b-274">Gibt an, ob der Gerätefreigabemodus zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="bf02b-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="bf02b-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="bf02b-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="bf02b-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-276">Boolean</span></span>|<span data-ttu-id="bf02b-277">Gibt an, ob die Google-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="bf02b-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="bf02b-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="bf02b-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-279">Boolean</span></span>|<span data-ttu-id="bf02b-280">Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="bf02b-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="bf02b-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="bf02b-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-282">Boolean</span></span>|<span data-ttu-id="bf02b-283">Gibt an, ob eine Geräteverschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bf02b-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="bf02b-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="bf02b-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="bf02b-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-285">Boolean</span></span>|<span data-ttu-id="bf02b-286">Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bf02b-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="bf02b-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="bf02b-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-288">Boolean</span></span>|<span data-ttu-id="bf02b-289">Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="bf02b-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-290">voiceDialingBlocked</span></span>|<span data-ttu-id="bf02b-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-291">Boolean</span></span>|<span data-ttu-id="bf02b-292">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="bf02b-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="bf02b-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="bf02b-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-294">Boolean</span></span>|<span data-ttu-id="bf02b-295">Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="bf02b-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="bf02b-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="bf02b-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-297">Boolean</span></span>|<span data-ttu-id="bf02b-298">Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="bf02b-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="bf02b-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="bf02b-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-300">Boolean</span></span>|<span data-ttu-id="bf02b-301">Gibt an, ob JavaScript im Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="bf02b-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-302">webBrowserBlocked</span></span>|<span data-ttu-id="bf02b-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-303">Boolean</span></span>|<span data-ttu-id="bf02b-304">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="bf02b-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="bf02b-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="bf02b-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="bf02b-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="bf02b-307">Cookieeinstellungen des Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="bf02b-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="bf02b-308">Mögliche Werte sind: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited` und `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="bf02b-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="bf02b-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="bf02b-309">wiFiBlocked</span></span>|<span data-ttu-id="bf02b-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-310">Boolean</span></span>|<span data-ttu-id="bf02b-311">Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bf02b-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="bf02b-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="bf02b-312">appsInstallAllowList</span></span>|<span data-ttu-id="bf02b-313">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bf02b-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bf02b-314">Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="bf02b-315">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bf02b-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bf02b-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="bf02b-316">appsLaunchBlockList</span></span>|<span data-ttu-id="bf02b-317">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bf02b-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bf02b-318">Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="bf02b-319">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bf02b-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bf02b-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="bf02b-320">appsHideList</span></span>|<span data-ttu-id="bf02b-321">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bf02b-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bf02b-322">Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bf02b-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="bf02b-323">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bf02b-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bf02b-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="bf02b-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="bf02b-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf02b-325">Boolean</span></span>|<span data-ttu-id="bf02b-326">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="bf02b-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="bf02b-327">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf02b-327">Response</span></span>
<span data-ttu-id="bf02b-328">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bf02b-328">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf02b-329">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf02b-329">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf02b-330">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf02b-330">Request</span></span>
<span data-ttu-id="bf02b-331">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf02b-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3225

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="bf02b-332">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf02b-332">Response</span></span>
<span data-ttu-id="bf02b-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf02b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





