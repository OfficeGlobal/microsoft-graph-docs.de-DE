# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="a5dfa-101">iosGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a5dfa-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a5dfa-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5dfa-103">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5dfa-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5dfa-104">Prerequisites</span></span>
<span data-ttu-id="a5dfa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5dfa-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5dfa-107">Permission type</span></span>|<span data-ttu-id="a5dfa-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5dfa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5dfa-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5dfa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a5dfa-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5dfa-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5dfa-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5dfa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5dfa-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5dfa-112">Not supported.</span></span>|
|<span data-ttu-id="a5dfa-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-113">Application</span></span>|<span data-ttu-id="a5dfa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5dfa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5dfa-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a5dfa-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5dfa-116">Request headers</span></span>
|<span data-ttu-id="a5dfa-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5dfa-117">Header</span></span>|<span data-ttu-id="a5dfa-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a5dfa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5dfa-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-119">Authorization</span></span>|<span data-ttu-id="a5dfa-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5dfa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5dfa-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a5dfa-121">Accept</span></span>|<span data-ttu-id="a5dfa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a5dfa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5dfa-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5dfa-123">Request body</span></span>
<span data-ttu-id="a5dfa-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a5dfa-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="a5dfa-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5dfa-126">Property</span></span>|<span data-ttu-id="a5dfa-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a5dfa-127">Type</span></span>|<span data-ttu-id="a5dfa-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5dfa-129">id</span><span class="sxs-lookup"><span data-stu-id="a5dfa-129">id</span></span>|<span data-ttu-id="a5dfa-130">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-130">String</span></span>|<span data-ttu-id="a5dfa-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-131">Key of the entity.</span></span> <span data-ttu-id="a5dfa-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5dfa-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5dfa-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a5dfa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5dfa-134">DateTimeOffset</span></span>|<span data-ttu-id="a5dfa-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a5dfa-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5dfa-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5dfa-137">createdDateTime</span></span>|<span data-ttu-id="a5dfa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5dfa-138">DateTimeOffset</span></span>|<span data-ttu-id="a5dfa-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-139">DateTime the object was created.</span></span> <span data-ttu-id="a5dfa-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5dfa-141">description</span><span class="sxs-lookup"><span data-stu-id="a5dfa-141">description</span></span>|<span data-ttu-id="a5dfa-142">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-142">String</span></span>|<span data-ttu-id="a5dfa-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5dfa-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5dfa-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a5dfa-145">displayName</span></span>|<span data-ttu-id="a5dfa-146">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-146">String</span></span>|<span data-ttu-id="a5dfa-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5dfa-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5dfa-149">Version</span><span class="sxs-lookup"><span data-stu-id="a5dfa-149">version</span></span>|<span data-ttu-id="a5dfa-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-150">Int32</span></span>|<span data-ttu-id="a5dfa-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-151">Version of the device configuration.</span></span> <span data-ttu-id="a5dfa-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5dfa-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-153">accountBlockModification</span></span>|<span data-ttu-id="a5dfa-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-154">Boolean</span></span>|<span data-ttu-id="a5dfa-155">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="a5dfa-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="a5dfa-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-157">Boolean</span></span>|<span data-ttu-id="a5dfa-158">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-159">airDropBlocked</span></span>|<span data-ttu-id="a5dfa-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-160">Boolean</span></span>|<span data-ttu-id="a5dfa-161">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="a5dfa-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="a5dfa-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-163">Boolean</span></span>|<span data-ttu-id="a5dfa-164">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="a5dfa-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="a5dfa-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-166">Boolean</span></span>|<span data-ttu-id="a5dfa-167">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="a5dfa-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="a5dfa-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="a5dfa-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-169">Boolean</span></span>|<span data-ttu-id="a5dfa-170">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="a5dfa-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="a5dfa-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-172">Boolean</span></span>|<span data-ttu-id="a5dfa-173">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="a5dfa-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-174">appleNewsBlocked</span></span>|<span data-ttu-id="a5dfa-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-175">Boolean</span></span>|<span data-ttu-id="a5dfa-176">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="a5dfa-177">appsSingleAppModeList</span></span>|<span data-ttu-id="a5dfa-178">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="a5dfa-179">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="a5dfa-180">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-180">Supervised only.</span></span> <span data-ttu-id="a5dfa-181">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-181">iOS 7.0 and later.</span></span> <span data-ttu-id="a5dfa-182">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a5dfa-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="a5dfa-183">appsVisibilityList</span></span>|<span data-ttu-id="a5dfa-184">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="a5dfa-185">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="a5dfa-186">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a5dfa-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="a5dfa-187">appsVisibilityListType</span></span>|<span data-ttu-id="a5dfa-188">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-188">String</span></span>|<span data-ttu-id="a5dfa-189">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="a5dfa-190">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a5dfa-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="a5dfa-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="a5dfa-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-192">Boolean</span></span>|<span data-ttu-id="a5dfa-193">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-194">appStoreBlocked</span></span>|<span data-ttu-id="a5dfa-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-195">Boolean</span></span>|<span data-ttu-id="a5dfa-196">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="a5dfa-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="a5dfa-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="a5dfa-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-198">Boolean</span></span>|<span data-ttu-id="a5dfa-199">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="a5dfa-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a5dfa-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="a5dfa-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-201">Boolean</span></span>|<span data-ttu-id="a5dfa-202">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="a5dfa-203">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a5dfa-204">appStoreRequirePassword</span></span>|<span data-ttu-id="a5dfa-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-205">Boolean</span></span>|<span data-ttu-id="a5dfa-206">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="a5dfa-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-207">bluetoothBlockModification</span></span>|<span data-ttu-id="a5dfa-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-208">Boolean</span></span>|<span data-ttu-id="a5dfa-209">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-210">cameraBlocked</span></span>|<span data-ttu-id="a5dfa-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-211">Boolean</span></span>|<span data-ttu-id="a5dfa-212">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="a5dfa-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="a5dfa-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="a5dfa-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-214">Boolean</span></span>|<span data-ttu-id="a5dfa-215">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="a5dfa-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="a5dfa-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="a5dfa-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-217">Boolean</span></span>|<span data-ttu-id="a5dfa-218">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="a5dfa-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="a5dfa-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-220">Boolean</span></span>|<span data-ttu-id="a5dfa-221">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="a5dfa-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="a5dfa-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-223">Boolean</span></span>|<span data-ttu-id="a5dfa-224">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="a5dfa-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="a5dfa-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="a5dfa-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-226">Boolean</span></span>|<span data-ttu-id="a5dfa-227">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="a5dfa-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="a5dfa-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="a5dfa-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-229">Boolean</span></span>|<span data-ttu-id="a5dfa-230">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="a5dfa-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="a5dfa-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="a5dfa-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-232">Boolean</span></span>|<span data-ttu-id="a5dfa-233">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="a5dfa-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="a5dfa-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-235">Boolean</span></span>|<span data-ttu-id="a5dfa-236">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="a5dfa-237">compliantAppsList</span></span>|<span data-ttu-id="a5dfa-238">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="a5dfa-239">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="a5dfa-240">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a5dfa-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="a5dfa-241">compliantAppListType</span></span>|<span data-ttu-id="a5dfa-242">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-242">String</span></span>|<span data-ttu-id="a5dfa-243">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="a5dfa-244">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a5dfa-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="a5dfa-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="a5dfa-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-246">Boolean</span></span>|<span data-ttu-id="a5dfa-247">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-248">definitionLookupBlocked</span></span>|<span data-ttu-id="a5dfa-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-249">Boolean</span></span>|<span data-ttu-id="a5dfa-250">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="a5dfa-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="a5dfa-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="a5dfa-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-252">Boolean</span></span>|<span data-ttu-id="a5dfa-253">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="a5dfa-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="a5dfa-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-255">Boolean</span></span>|<span data-ttu-id="a5dfa-256">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-257">deviceBlockNameModification</span></span>|<span data-ttu-id="a5dfa-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-258">Boolean</span></span>|<span data-ttu-id="a5dfa-259">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="a5dfa-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="a5dfa-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-261">Boolean</span></span>|<span data-ttu-id="a5dfa-262">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="a5dfa-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="a5dfa-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-264">Boolean</span></span>|<span data-ttu-id="a5dfa-265">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="a5dfa-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="a5dfa-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="a5dfa-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-267">Boolean</span></span>|<span data-ttu-id="a5dfa-268">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="a5dfa-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="a5dfa-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="a5dfa-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-270">Boolean</span></span>|<span data-ttu-id="a5dfa-271">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="a5dfa-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="a5dfa-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="a5dfa-273">Zeichenfolge-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-273">String collection</span></span>|<span data-ttu-id="a5dfa-274">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="a5dfa-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="a5dfa-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="a5dfa-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-276">Boolean</span></span>|<span data-ttu-id="a5dfa-277">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="a5dfa-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="a5dfa-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-279">Boolean</span></span>|<span data-ttu-id="a5dfa-280">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="a5dfa-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-281">faceTimeBlocked</span></span>|<span data-ttu-id="a5dfa-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-282">Boolean</span></span>|<span data-ttu-id="a5dfa-283">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="a5dfa-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="a5dfa-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-285">Boolean</span></span>|<span data-ttu-id="a5dfa-286">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="a5dfa-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="a5dfa-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-288">Boolean</span></span>|<span data-ttu-id="a5dfa-289">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="a5dfa-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="a5dfa-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="a5dfa-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-291">Boolean</span></span>|<span data-ttu-id="a5dfa-292">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="a5dfa-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-293">gameCenterBlocked</span></span>|<span data-ttu-id="a5dfa-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-294">Boolean</span></span>|<span data-ttu-id="a5dfa-295">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-296">hostPairingBlocked</span></span>|<span data-ttu-id="a5dfa-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-297">Boolean</span></span>|<span data-ttu-id="a5dfa-298">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="a5dfa-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-300">Boolean</span></span>|<span data-ttu-id="a5dfa-301">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="a5dfa-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="a5dfa-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-303">Boolean</span></span>|<span data-ttu-id="a5dfa-304">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="a5dfa-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="a5dfa-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="a5dfa-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-306">Boolean</span></span>|<span data-ttu-id="a5dfa-307">Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="a5dfa-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="a5dfa-308">iCloudBlockBackup</span></span>|<span data-ttu-id="a5dfa-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-309">Boolean</span></span>|<span data-ttu-id="a5dfa-310">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="a5dfa-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="a5dfa-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="a5dfa-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-312">Boolean</span></span>|<span data-ttu-id="a5dfa-313">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="a5dfa-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="a5dfa-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="a5dfa-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-315">Boolean</span></span>|<span data-ttu-id="a5dfa-316">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="a5dfa-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="a5dfa-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="a5dfa-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-318">Boolean</span></span>|<span data-ttu-id="a5dfa-319">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="a5dfa-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="a5dfa-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="a5dfa-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-321">Boolean</span></span>|<span data-ttu-id="a5dfa-322">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="a5dfa-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="a5dfa-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="a5dfa-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-324">Boolean</span></span>|<span data-ttu-id="a5dfa-325">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="a5dfa-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="a5dfa-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="a5dfa-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-327">Boolean</span></span>|<span data-ttu-id="a5dfa-328">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="a5dfa-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="a5dfa-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="a5dfa-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-330">Boolean</span></span>|<span data-ttu-id="a5dfa-331">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. </span><span class="sxs-lookup"><span data-stu-id="a5dfa-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="a5dfa-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="a5dfa-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="a5dfa-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-333">Boolean</span></span>|<span data-ttu-id="a5dfa-334">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="a5dfa-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="a5dfa-335">iTunesBlockRadio</span></span>|<span data-ttu-id="a5dfa-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-336">Boolean</span></span>|<span data-ttu-id="a5dfa-337">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="a5dfa-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="a5dfa-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-339">Boolean</span></span>|<span data-ttu-id="a5dfa-340">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="a5dfa-341">keyboardBlockDictation</span></span>|<span data-ttu-id="a5dfa-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-342">Boolean</span></span>|<span data-ttu-id="a5dfa-343">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="a5dfa-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="a5dfa-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-345">Boolean</span></span>|<span data-ttu-id="a5dfa-346">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="a5dfa-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="a5dfa-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-348">Boolean</span></span>|<span data-ttu-id="a5dfa-349">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="a5dfa-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="a5dfa-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-351">Boolean</span></span>|<span data-ttu-id="a5dfa-352">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="a5dfa-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="a5dfa-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-354">Boolean</span></span>|<span data-ttu-id="a5dfa-355">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="a5dfa-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="a5dfa-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-357">Boolean</span></span>|<span data-ttu-id="a5dfa-358">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="a5dfa-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="a5dfa-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-360">Boolean</span></span>|<span data-ttu-id="a5dfa-361">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="a5dfa-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="a5dfa-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-363">Boolean</span></span>|<span data-ttu-id="a5dfa-364">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="a5dfa-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="a5dfa-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-366">Boolean</span></span>|<span data-ttu-id="a5dfa-367">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="a5dfa-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="a5dfa-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-369">Boolean</span></span>|<span data-ttu-id="a5dfa-370">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="a5dfa-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="a5dfa-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-372">Boolean</span></span>|<span data-ttu-id="a5dfa-373">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="a5dfa-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="a5dfa-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-375">Boolean</span></span>|<span data-ttu-id="a5dfa-376">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="a5dfa-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="a5dfa-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-378">Boolean</span></span>|<span data-ttu-id="a5dfa-379">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="a5dfa-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="a5dfa-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-381">Boolean</span></span>|<span data-ttu-id="a5dfa-382">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="a5dfa-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="a5dfa-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-384">Boolean</span></span>|<span data-ttu-id="a5dfa-385">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a5dfa-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="a5dfa-387">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-387">String</span></span>|<span data-ttu-id="a5dfa-388">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="a5dfa-389">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="a5dfa-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="a5dfa-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="a5dfa-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-391">Boolean</span></span>|<span data-ttu-id="a5dfa-392">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="a5dfa-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="a5dfa-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-394">Boolean</span></span>|<span data-ttu-id="a5dfa-395">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="a5dfa-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="a5dfa-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-397">Boolean</span></span>|<span data-ttu-id="a5dfa-398">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="a5dfa-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="a5dfa-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-400">Boolean</span></span>|<span data-ttu-id="a5dfa-401">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="a5dfa-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="a5dfa-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-403">Boolean</span></span>|<span data-ttu-id="a5dfa-404">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="a5dfa-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="a5dfa-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="a5dfa-406">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-406">String</span></span>|<span data-ttu-id="a5dfa-407">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="a5dfa-408">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="a5dfa-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="a5dfa-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="a5dfa-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-410">Boolean</span></span>|<span data-ttu-id="a5dfa-411">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="a5dfa-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="a5dfa-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="a5dfa-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-413">Boolean</span></span>|<span data-ttu-id="a5dfa-414">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="a5dfa-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="a5dfa-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="a5dfa-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-416">Boolean</span></span>|<span data-ttu-id="a5dfa-417">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="a5dfa-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="a5dfa-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="a5dfa-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-419">Boolean</span></span>|<span data-ttu-id="a5dfa-420">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="a5dfa-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a5dfa-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="a5dfa-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a5dfa-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="a5dfa-423">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="a5dfa-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="a5dfa-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="a5dfa-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="a5dfa-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="a5dfa-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="a5dfa-426">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="a5dfa-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="a5dfa-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a5dfa-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="a5dfa-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a5dfa-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="a5dfa-429">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="a5dfa-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="a5dfa-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="a5dfa-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="a5dfa-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="a5dfa-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="a5dfa-432">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="a5dfa-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="a5dfa-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a5dfa-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="a5dfa-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a5dfa-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="a5dfa-435">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="a5dfa-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="a5dfa-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a5dfa-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="a5dfa-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a5dfa-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="a5dfa-438">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="a5dfa-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="a5dfa-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="a5dfa-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="a5dfa-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="a5dfa-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="a5dfa-441">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="a5dfa-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="a5dfa-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a5dfa-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="a5dfa-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a5dfa-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="a5dfa-444">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="a5dfa-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="a5dfa-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a5dfa-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="a5dfa-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a5dfa-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="a5dfa-447">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="a5dfa-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="a5dfa-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="a5dfa-448">networkUsageRules</span></span>|<span data-ttu-id="a5dfa-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="a5dfa-450">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="a5dfa-451">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a5dfa-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="a5dfa-452">mediaContentRatingApps</span></span>|<span data-ttu-id="a5dfa-453">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-453">String</span></span>|<span data-ttu-id="a5dfa-454">Bewertungseinstellungen für Medieninhalte für Apps. Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-454">Media content rating settings for Apps Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="a5dfa-455">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-455">messagesBlocked</span></span>|<span data-ttu-id="a5dfa-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-456">Boolean</span></span>|<span data-ttu-id="a5dfa-457">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-457">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="a5dfa-458">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-458">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="a5dfa-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-459">Boolean</span></span>|<span data-ttu-id="a5dfa-460">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-460">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-461">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a5dfa-461">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="a5dfa-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-462">Boolean</span></span>|<span data-ttu-id="a5dfa-463">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-463">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a5dfa-464">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-464">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="a5dfa-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-465">Boolean</span></span>|<span data-ttu-id="a5dfa-466">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-466">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="a5dfa-467">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-467">passcodeBlockModification</span></span>|<span data-ttu-id="a5dfa-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-468">Boolean</span></span>|<span data-ttu-id="a5dfa-469">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-469">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-470">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a5dfa-470">passcodeBlockSimple</span></span>|<span data-ttu-id="a5dfa-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-471">Boolean</span></span>|<span data-ttu-id="a5dfa-472">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-472">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="a5dfa-473">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a5dfa-473">passcodeExpirationDays</span></span>|<span data-ttu-id="a5dfa-474">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-474">Int32</span></span>|<span data-ttu-id="a5dfa-475">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-475">Number of days before the passcode expires.</span></span> <span data-ttu-id="a5dfa-476">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-476">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a5dfa-477">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a5dfa-477">passcodeMinimumLength</span></span>|<span data-ttu-id="a5dfa-478">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-478">Int32</span></span>|<span data-ttu-id="a5dfa-479">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-479">Minimum length of passcode.</span></span> <span data-ttu-id="a5dfa-480">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-480">Valid values 4 to 14</span></span>|
|<span data-ttu-id="a5dfa-481">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a5dfa-481">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a5dfa-482">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-482">Int32</span></span>|<span data-ttu-id="a5dfa-483">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-483">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="a5dfa-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a5dfa-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a5dfa-485">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-485">Int32</span></span>|<span data-ttu-id="a5dfa-486">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-486">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a5dfa-487">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a5dfa-487">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="a5dfa-488">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-488">Int32</span></span>|<span data-ttu-id="a5dfa-489">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="a5dfa-489">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="a5dfa-490">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-490">Valid values 0 to 4</span></span>|
|<span data-ttu-id="a5dfa-491">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="a5dfa-491">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="a5dfa-492">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-492">Int32</span></span>|<span data-ttu-id="a5dfa-493">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-493">Number of previous passcodes to block.</span></span> <span data-ttu-id="a5dfa-494">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-494">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a5dfa-495">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="a5dfa-495">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="a5dfa-496">Int32</span><span class="sxs-lookup"><span data-stu-id="a5dfa-496">Int32</span></span>|<span data-ttu-id="a5dfa-497">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-497">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="a5dfa-498">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-498">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a5dfa-499">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="a5dfa-499">passcodeRequiredType</span></span>|<span data-ttu-id="a5dfa-500">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-500">String</span></span>|<span data-ttu-id="a5dfa-501">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-501">Type of passcode that is required.</span></span> <span data-ttu-id="a5dfa-502">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-502">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a5dfa-503">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="a5dfa-503">passcodeRequired</span></span>|<span data-ttu-id="a5dfa-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-504">Boolean</span></span>|<span data-ttu-id="a5dfa-505">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-505">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="a5dfa-506">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-506">podcastsBlocked</span></span>|<span data-ttu-id="a5dfa-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-507">Boolean</span></span>|<span data-ttu-id="a5dfa-508">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-508">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="a5dfa-509">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="a5dfa-509">safariBlockAutofill</span></span>|<span data-ttu-id="a5dfa-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-510">Boolean</span></span>|<span data-ttu-id="a5dfa-511">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-511">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="a5dfa-512">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="a5dfa-512">safariBlockJavaScript</span></span>|<span data-ttu-id="a5dfa-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-513">Boolean</span></span>|<span data-ttu-id="a5dfa-514">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-514">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="a5dfa-515">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="a5dfa-515">safariBlockPopups</span></span>|<span data-ttu-id="a5dfa-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-516">Boolean</span></span>|<span data-ttu-id="a5dfa-517">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-517">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="a5dfa-518">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-518">safariBlocked</span></span>|<span data-ttu-id="a5dfa-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-519">Boolean</span></span>|<span data-ttu-id="a5dfa-520">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-520">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="a5dfa-521">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="a5dfa-521">safariCookieSettings</span></span>|<span data-ttu-id="a5dfa-522">String</span><span class="sxs-lookup"><span data-stu-id="a5dfa-522">String</span></span>|<span data-ttu-id="a5dfa-523">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-523">Cookie settings for Safari.</span></span> <span data-ttu-id="a5dfa-524">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-524">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="a5dfa-525">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="a5dfa-525">safariManagedDomains</span></span>|<span data-ttu-id="a5dfa-526">Zeichenfolge-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-526">String collection</span></span>|<span data-ttu-id="a5dfa-527">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-527">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="a5dfa-528">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="a5dfa-528">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="a5dfa-529">Zeichenfolge-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-529">String collection</span></span>|<span data-ttu-id="a5dfa-530">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-530">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="a5dfa-531">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5dfa-531">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5dfa-532">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="a5dfa-532">safariRequireFraudWarning</span></span>|<span data-ttu-id="a5dfa-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-533">Boolean</span></span>|<span data-ttu-id="a5dfa-534">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-534">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="a5dfa-535">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-535">screenCaptureBlocked</span></span>|<span data-ttu-id="a5dfa-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-536">Boolean</span></span>|<span data-ttu-id="a5dfa-537">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-537">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="a5dfa-538">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-538">siriBlocked</span></span>|<span data-ttu-id="a5dfa-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-539">Boolean</span></span>|<span data-ttu-id="a5dfa-540">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-540">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="a5dfa-541">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-541">siriBlockedWhenLocked</span></span>|<span data-ttu-id="a5dfa-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-542">Boolean</span></span>|<span data-ttu-id="a5dfa-543">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-543">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="a5dfa-544">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="a5dfa-544">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="a5dfa-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-545">Boolean</span></span>|<span data-ttu-id="a5dfa-546">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-546">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="a5dfa-547">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="a5dfa-547">siriRequireProfanityFilter</span></span>|<span data-ttu-id="a5dfa-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-548">Boolean</span></span>|<span data-ttu-id="a5dfa-549">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-549">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="a5dfa-550">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="a5dfa-550">spotlightBlockInternetResults</span></span>|<span data-ttu-id="a5dfa-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-551">Boolean</span></span>|<span data-ttu-id="a5dfa-552">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-552">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="a5dfa-553">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="a5dfa-553">voiceDialingBlocked</span></span>|<span data-ttu-id="a5dfa-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-554">Boolean</span></span>|<span data-ttu-id="a5dfa-555">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-555">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="a5dfa-556">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5dfa-556">wallpaperBlockModification</span></span>|<span data-ttu-id="a5dfa-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-557">Boolean</span></span>|<span data-ttu-id="a5dfa-558">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-558">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="a5dfa-559">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="a5dfa-559">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="a5dfa-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5dfa-560">Boolean</span></span>|<span data-ttu-id="a5dfa-561">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-561">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="a5dfa-562">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5dfa-562">Response</span></span>
<span data-ttu-id="a5dfa-563">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-563">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5dfa-564">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5dfa-564">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5dfa-565">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5dfa-565">Request</span></span>
<span data-ttu-id="a5dfa-566">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-566">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7773

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="a5dfa-567">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5dfa-567">Response</span></span>
<span data-ttu-id="a5dfa-p125">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5dfa-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7949

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



