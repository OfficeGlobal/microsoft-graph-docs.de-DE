---
title: Erstellen von „androidGeneralDeviceConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs androidGeneralDeviceConfiguration.
ms.openlocfilehash: 78d47c3fb191a573bf963c6fea33ae9a974eeaf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063153"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="c32e3-103">Erstellen von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c32e3-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c32e3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c32e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c32e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c32e3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c32e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c32e3-107">Diese Methode erstellt ein neues Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-107">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c32e3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c32e3-108">Prerequisites</span></span>
<span data-ttu-id="c32e3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c32e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c32e3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c32e3-111">Permission type</span></span>|<span data-ttu-id="c32e3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c32e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c32e3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c32e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c32e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c32e3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c32e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c32e3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c32e3-116">Not supported.</span></span>|
|<span data-ttu-id="c32e3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c32e3-117">Application</span></span>|<span data-ttu-id="c32e3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c32e3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c32e3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c32e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c32e3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c32e3-120">Request headers</span></span>
|<span data-ttu-id="c32e3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c32e3-121">Header</span></span>|<span data-ttu-id="c32e3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c32e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c32e3-123">Authorization</span></span>|<span data-ttu-id="c32e3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c32e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c32e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c32e3-125">Accept</span></span>|<span data-ttu-id="c32e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c32e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c32e3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c32e3-127">Request body</span></span>
<span data-ttu-id="c32e3-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="c32e3-128">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c32e3-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-129">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c32e3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c32e3-130">Property</span></span>|<span data-ttu-id="c32e3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c32e3-131">Type</span></span>|<span data-ttu-id="c32e3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c32e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c32e3-133">id</span><span class="sxs-lookup"><span data-stu-id="c32e3-133">id</span></span>|<span data-ttu-id="c32e3-134">String</span><span class="sxs-lookup"><span data-stu-id="c32e3-134">String</span></span>|<span data-ttu-id="c32e3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c32e3-135">Key of the entity.</span></span> <span data-ttu-id="c32e3-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c32e3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c32e3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c32e3-138">DateTimeOffset</span></span>|<span data-ttu-id="c32e3-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c32e3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c32e3-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c32e3-141">roleScopeTagIds</span></span>|<span data-ttu-id="c32e3-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c32e3-142">String collection</span></span>|<span data-ttu-id="c32e3-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c32e3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c32e3-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c32e3-145">supportsScopeTags</span></span>|<span data-ttu-id="c32e3-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c32e3-146">Boolean</span></span>|<span data-ttu-id="c32e3-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c32e3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c32e3-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c32e3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c32e3-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c32e3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c32e3-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c32e3-150">This property is read-only.</span></span> <span data-ttu-id="c32e3-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c32e3-152">createdDateTime</span></span>|<span data-ttu-id="c32e3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c32e3-153">DateTimeOffset</span></span>|<span data-ttu-id="c32e3-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c32e3-154">DateTime the object was created.</span></span> <span data-ttu-id="c32e3-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-156">description</span><span class="sxs-lookup"><span data-stu-id="c32e3-156">description</span></span>|<span data-ttu-id="c32e3-157">String</span><span class="sxs-lookup"><span data-stu-id="c32e3-157">String</span></span>|<span data-ttu-id="c32e3-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c32e3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c32e3-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c32e3-160">displayName</span></span>|<span data-ttu-id="c32e3-161">String</span><span class="sxs-lookup"><span data-stu-id="c32e3-161">String</span></span>|<span data-ttu-id="c32e3-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c32e3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c32e3-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-164">Version</span><span class="sxs-lookup"><span data-stu-id="c32e3-164">version</span></span>|<span data-ttu-id="c32e3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c32e3-165">Int32</span></span>|<span data-ttu-id="c32e3-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c32e3-166">Version of the device configuration.</span></span> <span data-ttu-id="c32e3-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c32e3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c32e3-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="c32e3-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="c32e3-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-169">Boolean</span></span>|<span data-ttu-id="c32e3-170">Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="c32e3-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="c32e3-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="c32e3-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-172">Boolean</span></span>|<span data-ttu-id="c32e3-173">Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="c32e3-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="c32e3-174">appsBlockYouTube</span></span>|<span data-ttu-id="c32e3-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-175">Boolean</span></span>|<span data-ttu-id="c32e3-176">Gibt an, ob die YouTube-App blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="c32e3-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-177">bluetoothBlocked</span></span>|<span data-ttu-id="c32e3-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-178">Boolean</span></span>|<span data-ttu-id="c32e3-179">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="c32e3-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-180">cameraBlocked</span></span>|<span data-ttu-id="c32e3-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-181">Boolean</span></span>|<span data-ttu-id="c32e3-182">Gibt an, ob die Verwendung der Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="c32e3-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c32e3-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c32e3-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-184">Boolean</span></span>|<span data-ttu-id="c32e3-185">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c32e3-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="c32e3-186">cellularBlockMessaging</span></span>|<span data-ttu-id="c32e3-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-187">Boolean</span></span>|<span data-ttu-id="c32e3-188">Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="c32e3-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="c32e3-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="c32e3-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-190">Boolean</span></span>|<span data-ttu-id="c32e3-191">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="c32e3-192">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="c32e3-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="c32e3-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-193">Boolean</span></span>|<span data-ttu-id="c32e3-194">Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="c32e3-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c32e3-195">compliantAppsList</span></span>|<span data-ttu-id="c32e3-196">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c32e3-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c32e3-197">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="c32e3-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c32e3-198">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c32e3-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c32e3-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c32e3-199">compliantAppListType</span></span>|[<span data-ttu-id="c32e3-200">appListType</span><span class="sxs-lookup"><span data-stu-id="c32e3-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c32e3-201">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="c32e3-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="c32e3-202">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c32e3-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c32e3-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c32e3-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c32e3-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-204">Boolean</span></span>|<span data-ttu-id="c32e3-205">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c32e3-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-206">locationServicesBlocked</span></span>|<span data-ttu-id="c32e3-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-207">Boolean</span></span>|<span data-ttu-id="c32e3-208">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="c32e3-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="c32e3-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="c32e3-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-210">Boolean</span></span>|<span data-ttu-id="c32e3-211">Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="c32e3-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="c32e3-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-213">Boolean</span></span>|<span data-ttu-id="c32e3-214">Gibt an, ob der Google Play-Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="c32e3-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="c32e3-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="c32e3-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-216">Boolean</span></span>|<span data-ttu-id="c32e3-217">Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c32e3-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="c32e3-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="c32e3-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-219">Boolean</span></span>|<span data-ttu-id="c32e3-220">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c32e3-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="c32e3-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="c32e3-222">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c32e3-222">Boolean</span></span>|<span data-ttu-id="c32e3-223">Gibt an, ob veränderbaren Datum und Uhrzeit im Modus KNOX blockieren.</span><span class="sxs-lookup"><span data-stu-id="c32e3-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="c32e3-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="c32e3-224">kioskModeApps</span></span>|<span data-ttu-id="c32e3-225">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c32e3-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c32e3-226">Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="c32e3-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="c32e3-227">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c32e3-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c32e3-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-228">nfcBlocked</span></span>|<span data-ttu-id="c32e3-229">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-229">Boolean</span></span>|<span data-ttu-id="c32e3-230">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="c32e3-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c32e3-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c32e3-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-232">Boolean</span></span>|<span data-ttu-id="c32e3-233">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c32e3-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c32e3-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="c32e3-235">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-235">Boolean</span></span>|<span data-ttu-id="c32e3-236">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="c32e3-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c32e3-237">passwordExpirationDays</span></span>|<span data-ttu-id="c32e3-238">Int32</span><span class="sxs-lookup"><span data-stu-id="c32e3-238">Int32</span></span>|<span data-ttu-id="c32e3-239">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="c32e3-239">Number of days before the password expires.</span></span> <span data-ttu-id="c32e3-240">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="c32e3-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c32e3-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c32e3-241">passwordMinimumLength</span></span>|<span data-ttu-id="c32e3-242">Int32</span><span class="sxs-lookup"><span data-stu-id="c32e3-242">Int32</span></span>|<span data-ttu-id="c32e3-243">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="c32e3-243">Minimum length of passwords.</span></span> <span data-ttu-id="c32e3-244">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="c32e3-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c32e3-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c32e3-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c32e3-246">Int32</span><span class="sxs-lookup"><span data-stu-id="c32e3-246">Int32</span></span>|<span data-ttu-id="c32e3-247">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="c32e3-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c32e3-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c32e3-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c32e3-249">Int32</span><span class="sxs-lookup"><span data-stu-id="c32e3-249">Int32</span></span>|<span data-ttu-id="c32e3-250">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-250">Number of previous passwords to block.</span></span> <span data-ttu-id="c32e3-251">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="c32e3-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c32e3-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c32e3-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c32e3-253">Int32</span><span class="sxs-lookup"><span data-stu-id="c32e3-253">Int32</span></span>|<span data-ttu-id="c32e3-254">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c32e3-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="c32e3-255">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="c32e3-255">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c32e3-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c32e3-256">passwordRequiredType</span></span>|[<span data-ttu-id="c32e3-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c32e3-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c32e3-258">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="c32e3-258">Type of password that is required.</span></span> <span data-ttu-id="c32e3-259">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="c32e3-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c32e3-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c32e3-260">passwordRequired</span></span>|<span data-ttu-id="c32e3-261">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-261">Boolean</span></span>|<span data-ttu-id="c32e3-262">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c32e3-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="c32e3-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-263">powerOffBlocked</span></span>|<span data-ttu-id="c32e3-264">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-264">Boolean</span></span>|<span data-ttu-id="c32e3-265">Gibt an, ob das Ausschalten des Geräts blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="c32e3-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-266">factoryResetBlocked</span></span>|<span data-ttu-id="c32e3-267">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-267">Boolean</span></span>|<span data-ttu-id="c32e3-268">Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.</span><span class="sxs-lookup"><span data-stu-id="c32e3-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="c32e3-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-269">screenCaptureBlocked</span></span>|<span data-ttu-id="c32e3-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-270">Boolean</span></span>|<span data-ttu-id="c32e3-271">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="c32e3-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="c32e3-272">deviceSharingAllowed</span></span>|<span data-ttu-id="c32e3-273">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-273">Boolean</span></span>|<span data-ttu-id="c32e3-274">Gibt an, ob der Gerätefreigabemodus zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="c32e3-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="c32e3-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="c32e3-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="c32e3-276">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-276">Boolean</span></span>|<span data-ttu-id="c32e3-277">Gibt an, ob die Google-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="c32e3-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="c32e3-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="c32e3-279">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-279">Boolean</span></span>|<span data-ttu-id="c32e3-280">Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="c32e3-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="c32e3-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="c32e3-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-282">Boolean</span></span>|<span data-ttu-id="c32e3-283">Gibt an, ob eine Geräteverschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c32e3-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="c32e3-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="c32e3-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="c32e3-285">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-285">Boolean</span></span>|<span data-ttu-id="c32e3-286">Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c32e3-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="c32e3-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="c32e3-288">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-288">Boolean</span></span>|<span data-ttu-id="c32e3-289">Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="c32e3-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-290">voiceDialingBlocked</span></span>|<span data-ttu-id="c32e3-291">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-291">Boolean</span></span>|<span data-ttu-id="c32e3-292">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="c32e3-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c32e3-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="c32e3-294">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-294">Boolean</span></span>|<span data-ttu-id="c32e3-295">Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="c32e3-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c32e3-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="c32e3-297">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-297">Boolean</span></span>|<span data-ttu-id="c32e3-298">Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="c32e3-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c32e3-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="c32e3-300">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-300">Boolean</span></span>|<span data-ttu-id="c32e3-301">Gibt an, ob JavaScript im Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="c32e3-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-302">webBrowserBlocked</span></span>|<span data-ttu-id="c32e3-303">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-303">Boolean</span></span>|<span data-ttu-id="c32e3-304">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="c32e3-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c32e3-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="c32e3-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c32e3-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="c32e3-307">Cookieeinstellungen des Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="c32e3-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="c32e3-308">Mögliche Werte sind: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited` und `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="c32e3-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="c32e3-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="c32e3-309">wiFiBlocked</span></span>|<span data-ttu-id="c32e3-310">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-310">Boolean</span></span>|<span data-ttu-id="c32e3-311">Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c32e3-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="c32e3-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="c32e3-312">appsInstallAllowList</span></span>|<span data-ttu-id="c32e3-313">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c32e3-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c32e3-314">Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="c32e3-315">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c32e3-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c32e3-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="c32e3-316">appsLaunchBlockList</span></span>|<span data-ttu-id="c32e3-317">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c32e3-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c32e3-318">Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="c32e3-319">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c32e3-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c32e3-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="c32e3-320">appsHideList</span></span>|<span data-ttu-id="c32e3-321">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c32e3-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c32e3-322">Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c32e3-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="c32e3-323">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c32e3-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c32e3-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c32e3-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="c32e3-325">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c32e3-325">Boolean</span></span>|<span data-ttu-id="c32e3-326">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="c32e3-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="c32e3-327">Antwort</span><span class="sxs-lookup"><span data-stu-id="c32e3-327">Response</span></span>
<span data-ttu-id="c32e3-328">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c32e3-328">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c32e3-329">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c32e3-329">Example</span></span>
### <a name="request"></a><span data-ttu-id="c32e3-330">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c32e3-330">Request</span></span>
<span data-ttu-id="c32e3-331">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c32e3-331">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c32e3-332">Antwort</span><span class="sxs-lookup"><span data-stu-id="c32e3-332">Response</span></span>
<span data-ttu-id="c32e3-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c32e3-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





