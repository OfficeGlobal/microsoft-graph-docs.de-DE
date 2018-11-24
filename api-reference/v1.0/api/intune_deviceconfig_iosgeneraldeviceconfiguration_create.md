# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="b4220-101">iosGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="b4220-101">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b4220-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4220-103">Erstellen Sie ein neues [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b4220-103">Create a new [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4220-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4220-104">Prerequisites</span></span>
<span data-ttu-id="b4220-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4220-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4220-107">Permission type</span></span>|<span data-ttu-id="b4220-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4220-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4220-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4220-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b4220-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4220-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4220-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4220-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4220-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4220-112">Not supported.</span></span>|
|<span data-ttu-id="b4220-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4220-113">Application</span></span>|<span data-ttu-id="b4220-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4220-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4220-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4220-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4220-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4220-116">Request headers</span></span>
|<span data-ttu-id="b4220-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4220-117">Header</span></span>|<span data-ttu-id="b4220-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4220-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4220-119">Authorization</span></span>|<span data-ttu-id="b4220-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4220-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4220-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4220-121">Accept</span></span>|<span data-ttu-id="b4220-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b4220-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4220-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4220-123">Request body</span></span>
<span data-ttu-id="b4220-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosGeneralDeviceConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b4220-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="b4220-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="b4220-125">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="b4220-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4220-126">Property</span></span>|<span data-ttu-id="b4220-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b4220-127">Type</span></span>|<span data-ttu-id="b4220-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4220-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4220-129">id</span><span class="sxs-lookup"><span data-stu-id="b4220-129">id</span></span>|<span data-ttu-id="b4220-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4220-130">String</span></span>|<span data-ttu-id="b4220-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4220-131">Key of the entity.</span></span> <span data-ttu-id="b4220-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4220-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4220-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b4220-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4220-134">DateTimeOffset</span></span>|<span data-ttu-id="b4220-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4220-135">DateTime the object was last modified.</span></span> <span data-ttu-id="b4220-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4220-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4220-137">createdDateTime</span></span>|<span data-ttu-id="b4220-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4220-138">DateTimeOffset</span></span>|<span data-ttu-id="b4220-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4220-139">DateTime the object was created.</span></span> <span data-ttu-id="b4220-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4220-141">description</span><span class="sxs-lookup"><span data-stu-id="b4220-141">description</span></span>|<span data-ttu-id="b4220-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4220-142">String</span></span>|<span data-ttu-id="b4220-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4220-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4220-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4220-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b4220-145">displayName</span></span>|<span data-ttu-id="b4220-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4220-146">String</span></span>|<span data-ttu-id="b4220-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4220-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4220-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4220-149">Version</span><span class="sxs-lookup"><span data-stu-id="b4220-149">version</span></span>|<span data-ttu-id="b4220-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-150">Int32</span></span>|<span data-ttu-id="b4220-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b4220-151">Version of the device configuration.</span></span> <span data-ttu-id="b4220-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4220-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4220-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="b4220-153">accountBlockModification</span></span>|<span data-ttu-id="b4220-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-154">Boolean</span></span>|<span data-ttu-id="b4220-155">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="b4220-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="b4220-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-157">Boolean</span></span>|<span data-ttu-id="b4220-158">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="b4220-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-159">airDropBlocked</span></span>|<span data-ttu-id="b4220-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-160">Boolean</span></span>|<span data-ttu-id="b4220-161">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="b4220-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="b4220-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-163">Boolean</span></span>|<span data-ttu-id="b4220-164">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="b4220-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="b4220-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-166">Boolean</span></span>|<span data-ttu-id="b4220-167">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="b4220-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="b4220-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="b4220-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="b4220-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-169">Boolean</span></span>|<span data-ttu-id="b4220-170">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="b4220-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="b4220-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-172">Boolean</span></span>|<span data-ttu-id="b4220-173">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="b4220-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-174">appleNewsBlocked</span></span>|<span data-ttu-id="b4220-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-175">Boolean</span></span>|<span data-ttu-id="b4220-176">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="b4220-177">appsSingleAppModeList</span></span>|<span data-ttu-id="b4220-178">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b4220-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4220-179">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="b4220-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="b4220-180">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="b4220-180">Supervised only.</span></span> <span data-ttu-id="b4220-181">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="b4220-181">iOS 7.0 and later.</span></span> <span data-ttu-id="b4220-182">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4220-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b4220-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="b4220-183">appsVisibilityList</span></span>|<span data-ttu-id="b4220-184">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b4220-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4220-185">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="b4220-186">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4220-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b4220-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="b4220-187">appsVisibilityListType</span></span>|[<span data-ttu-id="b4220-188">appListType</span><span class="sxs-lookup"><span data-stu-id="b4220-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="b4220-189">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="b4220-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="b4220-190">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b4220-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b4220-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="b4220-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="b4220-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-192">Boolean</span></span>|<span data-ttu-id="b4220-193">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-194">appStoreBlocked</span></span>|<span data-ttu-id="b4220-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-195">Boolean</span></span>|<span data-ttu-id="b4220-196">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="b4220-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="b4220-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="b4220-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-198">Boolean</span></span>|<span data-ttu-id="b4220-199">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="b4220-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="b4220-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b4220-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="b4220-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-201">Boolean</span></span>|<span data-ttu-id="b4220-202">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="b4220-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="b4220-203">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="b4220-204">appStoreRequirePassword</span></span>|<span data-ttu-id="b4220-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-205">Boolean</span></span>|<span data-ttu-id="b4220-206">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="b4220-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="b4220-207">bluetoothBlockModification</span></span>|<span data-ttu-id="b4220-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-208">Boolean</span></span>|<span data-ttu-id="b4220-209">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="b4220-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-210">cameraBlocked</span></span>|<span data-ttu-id="b4220-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-211">Boolean</span></span>|<span data-ttu-id="b4220-212">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="b4220-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b4220-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b4220-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b4220-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-214">Boolean</span></span>|<span data-ttu-id="b4220-215">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b4220-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="b4220-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="b4220-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-217">Boolean</span></span>|<span data-ttu-id="b4220-218">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="b4220-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="b4220-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="b4220-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-220">Boolean</span></span>|<span data-ttu-id="b4220-221">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="b4220-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="b4220-223">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-223">Boolean</span></span>|<span data-ttu-id="b4220-224">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="b4220-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b4220-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b4220-226">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-226">Boolean</span></span>|<span data-ttu-id="b4220-227">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b4220-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="b4220-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="b4220-229">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-229">Boolean</span></span>|<span data-ttu-id="b4220-230">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b4220-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="b4220-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b4220-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b4220-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-232">Boolean</span></span>|<span data-ttu-id="b4220-233">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b4220-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b4220-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b4220-235">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-235">Boolean</span></span>|<span data-ttu-id="b4220-236">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b4220-237">compliantAppsList</span></span>|<span data-ttu-id="b4220-238">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b4220-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4220-239">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="b4220-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b4220-240">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4220-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b4220-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b4220-241">compliantAppListType</span></span>|[<span data-ttu-id="b4220-242">appListType</span><span class="sxs-lookup"><span data-stu-id="b4220-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="b4220-243">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="b4220-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b4220-244">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b4220-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b4220-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="b4220-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="b4220-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-246">Boolean</span></span>|<span data-ttu-id="b4220-247">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-248">definitionLookupBlocked</span></span>|<span data-ttu-id="b4220-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-249">Boolean</span></span>|<span data-ttu-id="b4220-250">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="b4220-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="b4220-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="b4220-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-252">Boolean</span></span>|<span data-ttu-id="b4220-253">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="b4220-255">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-255">Boolean</span></span>|<span data-ttu-id="b4220-256">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="b4220-257">deviceBlockNameModification</span></span>|<span data-ttu-id="b4220-258">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-258">Boolean</span></span>|<span data-ttu-id="b4220-259">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b4220-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b4220-261">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-261">Boolean</span></span>|<span data-ttu-id="b4220-262">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b4220-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="b4220-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="b4220-264">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-264">Boolean</span></span>|<span data-ttu-id="b4220-265">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="b4220-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="b4220-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="b4220-267">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-267">Boolean</span></span>|<span data-ttu-id="b4220-268">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b4220-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="b4220-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="b4220-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="b4220-270">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-270">Boolean</span></span>|<span data-ttu-id="b4220-271">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b4220-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="b4220-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b4220-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="b4220-273">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4220-273">String collection</span></span>|<span data-ttu-id="b4220-274">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="b4220-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b4220-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="b4220-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="b4220-276">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-276">Boolean</span></span>|<span data-ttu-id="b4220-277">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="b4220-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="b4220-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="b4220-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="b4220-279">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-279">Boolean</span></span>|<span data-ttu-id="b4220-280">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="b4220-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="b4220-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-281">faceTimeBlocked</span></span>|<span data-ttu-id="b4220-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-282">Boolean</span></span>|<span data-ttu-id="b4220-283">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="b4220-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="b4220-285">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-285">Boolean</span></span>|<span data-ttu-id="b4220-286">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="b4220-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="b4220-288">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-288">Boolean</span></span>|<span data-ttu-id="b4220-289">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="b4220-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="b4220-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="b4220-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="b4220-291">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-291">Boolean</span></span>|<span data-ttu-id="b4220-292">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="b4220-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-293">gameCenterBlocked</span></span>|<span data-ttu-id="b4220-294">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-294">Boolean</span></span>|<span data-ttu-id="b4220-295">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-296">hostPairingBlocked</span></span>|<span data-ttu-id="b4220-297">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-297">Boolean</span></span>|<span data-ttu-id="b4220-298">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="b4220-300">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-300">Boolean</span></span>|<span data-ttu-id="b4220-301">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="b4220-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="b4220-303">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-303">Boolean</span></span>|<span data-ttu-id="b4220-304">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="b4220-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="b4220-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b4220-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b4220-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4220-306">Boolean</span></span>|<span data-ttu-id="b4220-307">Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.</span><span class="sxs-lookup"><span data-stu-id="b4220-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="b4220-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b4220-308">iCloudBlockBackup</span></span>|<span data-ttu-id="b4220-309">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-309">Boolean</span></span>|<span data-ttu-id="b4220-310">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="b4220-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b4220-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b4220-312">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-312">Boolean</span></span>|<span data-ttu-id="b4220-313">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="b4220-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="b4220-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="b4220-315">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-315">Boolean</span></span>|<span data-ttu-id="b4220-316">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="b4220-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b4220-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b4220-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-318">Boolean</span></span>|<span data-ttu-id="b4220-319">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b4220-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="b4220-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="b4220-321">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-321">Boolean</span></span>|<span data-ttu-id="b4220-322">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="b4220-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="b4220-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="b4220-324">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-324">Boolean</span></span>|<span data-ttu-id="b4220-325">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="b4220-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="b4220-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="b4220-327">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-327">Boolean</span></span>|<span data-ttu-id="b4220-328">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="b4220-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="b4220-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="b4220-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="b4220-330">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-330">Boolean</span></span>|<span data-ttu-id="b4220-331">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. </span><span class="sxs-lookup"><span data-stu-id="b4220-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="b4220-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b4220-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="b4220-333">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-333">Boolean</span></span>|<span data-ttu-id="b4220-334">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b4220-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="b4220-335">iTunesBlockRadio</span></span>|<span data-ttu-id="b4220-336">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-336">Boolean</span></span>|<span data-ttu-id="b4220-337">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b4220-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="b4220-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="b4220-339">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-339">Boolean</span></span>|<span data-ttu-id="b4220-340">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b4220-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b4220-341">keyboardBlockDictation</span></span>|<span data-ttu-id="b4220-342">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-342">Boolean</span></span>|<span data-ttu-id="b4220-343">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b4220-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="b4220-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="b4220-345">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-345">Boolean</span></span>|<span data-ttu-id="b4220-346">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b4220-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="b4220-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="b4220-348">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-348">Boolean</span></span>|<span data-ttu-id="b4220-349">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="b4220-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="b4220-351">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-351">Boolean</span></span>|<span data-ttu-id="b4220-352">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b4220-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="b4220-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="b4220-354">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-354">Boolean</span></span>|<span data-ttu-id="b4220-355">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="b4220-357">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-357">Boolean</span></span>|<span data-ttu-id="b4220-358">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="b4220-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="b4220-360">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-360">Boolean</span></span>|<span data-ttu-id="b4220-361">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="b4220-363">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-363">Boolean</span></span>|<span data-ttu-id="b4220-364">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b4220-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="b4220-366">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-366">Boolean</span></span>|<span data-ttu-id="b4220-367">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b4220-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="b4220-369">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-369">Boolean</span></span>|<span data-ttu-id="b4220-370">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="b4220-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="b4220-372">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-372">Boolean</span></span>|<span data-ttu-id="b4220-373">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b4220-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="b4220-375">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-375">Boolean</span></span>|<span data-ttu-id="b4220-376">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="b4220-378">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-378">Boolean</span></span>|<span data-ttu-id="b4220-379">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b4220-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="b4220-381">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-381">Boolean</span></span>|<span data-ttu-id="b4220-382">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="b4220-384">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-384">Boolean</span></span>|<span data-ttu-id="b4220-385">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b4220-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="b4220-387">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4220-387">String</span></span>|<span data-ttu-id="b4220-388">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="b4220-389">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="b4220-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="b4220-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="b4220-391">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4220-391">String</span></span>|<span data-ttu-id="b4220-392">ID für integrierte apps im Kioskmodus verwenden.</span><span class="sxs-lookup"><span data-stu-id="b4220-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="b4220-393">Verwendet, wenn KioskModeManagedAppId und KioskModeAppStoreUrl nicht festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b4220-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="b4220-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="b4220-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="b4220-395">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-395">Boolean</span></span>|<span data-ttu-id="b4220-396">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="b4220-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="b4220-398">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-398">Boolean</span></span>|<span data-ttu-id="b4220-399">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="b4220-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="b4220-401">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-401">Boolean</span></span>|<span data-ttu-id="b4220-402">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="b4220-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="b4220-404">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-404">Boolean</span></span>|<span data-ttu-id="b4220-405">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b4220-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="b4220-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="b4220-407">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-407">Boolean</span></span>|<span data-ttu-id="b4220-408">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="b4220-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="b4220-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="b4220-410">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4220-410">String</span></span>|<span data-ttu-id="b4220-411">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="b4220-412">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="b4220-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="b4220-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="b4220-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="b4220-414">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-414">Boolean</span></span>|<span data-ttu-id="b4220-415">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="b4220-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="b4220-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="b4220-417">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-417">Boolean</span></span>|<span data-ttu-id="b4220-418">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="b4220-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="b4220-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="b4220-420">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-420">Boolean</span></span>|<span data-ttu-id="b4220-421">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="b4220-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="b4220-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="b4220-423">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-423">Boolean</span></span>|<span data-ttu-id="b4220-424">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="b4220-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b4220-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="b4220-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b4220-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="b4220-427">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="b4220-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="b4220-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b4220-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="b4220-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b4220-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="b4220-430">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="b4220-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="b4220-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b4220-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="b4220-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b4220-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="b4220-433">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="b4220-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="b4220-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b4220-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="b4220-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b4220-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="b4220-436">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="b4220-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="b4220-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b4220-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="b4220-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b4220-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="b4220-439">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="b4220-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="b4220-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b4220-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="b4220-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b4220-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="b4220-442">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="b4220-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="b4220-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b4220-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="b4220-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b4220-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="b4220-445">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="b4220-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="b4220-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b4220-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="b4220-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b4220-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="b4220-448">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="b4220-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="b4220-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b4220-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="b4220-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b4220-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="b4220-451">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="b4220-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="b4220-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="b4220-452">networkUsageRules</span></span>|<span data-ttu-id="b4220-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b4220-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="b4220-454">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="b4220-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="b4220-455">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4220-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b4220-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="b4220-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="b4220-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="b4220-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="b4220-458">Media content Bewertung Einstellungen für Apps.</span><span class="sxs-lookup"><span data-stu-id="b4220-458">Media content rating settings for Apps.</span></span> <span data-ttu-id="b4220-459">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="b4220-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="b4220-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-460">messagesBlocked</span></span>|<span data-ttu-id="b4220-461">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-461">Boolean</span></span>|<span data-ttu-id="b4220-462">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="b4220-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="b4220-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="b4220-464">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-464">Boolean</span></span>|<span data-ttu-id="b4220-465">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b4220-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b4220-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="b4220-467">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-467">Boolean</span></span>|<span data-ttu-id="b4220-468">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b4220-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="b4220-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="b4220-470">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-470">Boolean</span></span>|<span data-ttu-id="b4220-471">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="b4220-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="b4220-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="b4220-472">passcodeBlockModification</span></span>|<span data-ttu-id="b4220-473">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-473">Boolean</span></span>|<span data-ttu-id="b4220-474">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b4220-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b4220-475">passcodeBlockSimple</span></span>|<span data-ttu-id="b4220-476">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-476">Boolean</span></span>|<span data-ttu-id="b4220-477">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="b4220-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b4220-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b4220-478">passcodeExpirationDays</span></span>|<span data-ttu-id="b4220-479">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-479">Int32</span></span>|<span data-ttu-id="b4220-480">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="b4220-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="b4220-481">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="b4220-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b4220-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b4220-482">passcodeMinimumLength</span></span>|<span data-ttu-id="b4220-483">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-483">Int32</span></span>|<span data-ttu-id="b4220-484">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="b4220-484">Minimum length of passcode.</span></span> <span data-ttu-id="b4220-485">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="b4220-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b4220-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b4220-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b4220-487">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-487">Int32</span></span>|<span data-ttu-id="b4220-488">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b4220-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b4220-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b4220-490">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-490">Int32</span></span>|<span data-ttu-id="b4220-491">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="b4220-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b4220-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b4220-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b4220-493">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-493">Int32</span></span>|<span data-ttu-id="b4220-494">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="b4220-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="b4220-495">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="b4220-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b4220-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b4220-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b4220-497">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-497">Int32</span></span>|<span data-ttu-id="b4220-498">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="b4220-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="b4220-499">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="b4220-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b4220-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="b4220-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="b4220-501">Int32</span><span class="sxs-lookup"><span data-stu-id="b4220-501">Int32</span></span>|<span data-ttu-id="b4220-502">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="b4220-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="b4220-503">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="b4220-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b4220-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b4220-504">passcodeRequiredType</span></span>|[<span data-ttu-id="b4220-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b4220-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="b4220-506">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="b4220-506">Type of passcode that is required.</span></span> <span data-ttu-id="b4220-507">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b4220-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b4220-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b4220-508">passcodeRequired</span></span>|<span data-ttu-id="b4220-509">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-509">Boolean</span></span>|<span data-ttu-id="b4220-510">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b4220-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-511">podcastsBlocked</span></span>|<span data-ttu-id="b4220-512">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-512">Boolean</span></span>|<span data-ttu-id="b4220-513">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="b4220-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b4220-514">safariBlockAutofill</span></span>|<span data-ttu-id="b4220-515">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-515">Boolean</span></span>|<span data-ttu-id="b4220-516">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="b4220-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b4220-517">safariBlockJavaScript</span></span>|<span data-ttu-id="b4220-518">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-518">Boolean</span></span>|<span data-ttu-id="b4220-519">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="b4220-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b4220-520">safariBlockPopups</span></span>|<span data-ttu-id="b4220-521">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-521">Boolean</span></span>|<span data-ttu-id="b4220-522">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b4220-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="b4220-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-523">safariBlocked</span></span>|<span data-ttu-id="b4220-524">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-524">Boolean</span></span>|<span data-ttu-id="b4220-525">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="b4220-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-526">safariCookieSettings</span></span>|[<span data-ttu-id="b4220-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b4220-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="b4220-528">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="b4220-528">Cookie settings for Safari.</span></span> <span data-ttu-id="b4220-529">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="b4220-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="b4220-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="b4220-530">safariManagedDomains</span></span>|<span data-ttu-id="b4220-531">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4220-531">String collection</span></span>|<span data-ttu-id="b4220-532">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="b4220-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="b4220-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="b4220-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="b4220-534">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b4220-534">String collection</span></span>|<span data-ttu-id="b4220-535">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="b4220-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="b4220-536">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b4220-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b4220-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b4220-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="b4220-538">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-538">Boolean</span></span>|<span data-ttu-id="b4220-539">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="b4220-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-540">screenCaptureBlocked</span></span>|<span data-ttu-id="b4220-541">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-541">Boolean</span></span>|<span data-ttu-id="b4220-542">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="b4220-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b4220-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-543">siriBlocked</span></span>|<span data-ttu-id="b4220-544">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-544">Boolean</span></span>|<span data-ttu-id="b4220-545">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="b4220-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="b4220-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="b4220-547">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-547">Boolean</span></span>|<span data-ttu-id="b4220-548">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="b4220-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="b4220-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="b4220-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="b4220-550">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-550">Boolean</span></span>|<span data-ttu-id="b4220-551">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="b4220-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="b4220-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="b4220-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="b4220-553">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-553">Boolean</span></span>|<span data-ttu-id="b4220-554">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="b4220-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="b4220-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b4220-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b4220-556">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-556">Boolean</span></span>|<span data-ttu-id="b4220-557">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="b4220-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="b4220-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b4220-558">voiceDialingBlocked</span></span>|<span data-ttu-id="b4220-559">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-559">Boolean</span></span>|<span data-ttu-id="b4220-560">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4220-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b4220-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="b4220-561">wallpaperBlockModification</span></span>|<span data-ttu-id="b4220-562">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-562">Boolean</span></span>|<span data-ttu-id="b4220-563">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b4220-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="b4220-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="b4220-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="b4220-565">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4220-565">Boolean</span></span>|<span data-ttu-id="b4220-566">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b4220-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="b4220-567">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4220-567">Response</span></span>
<span data-ttu-id="b4220-568">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4220-568">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4220-569">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4220-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4220-570">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4220-570">Request</span></span>
<span data-ttu-id="b4220-571">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4220-571">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
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

### <a name="response"></a><span data-ttu-id="b4220-572">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4220-572">Response</span></span>
<span data-ttu-id="b4220-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4220-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8013

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
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
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



