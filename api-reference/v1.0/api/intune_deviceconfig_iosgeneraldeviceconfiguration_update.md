# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ff0f3-101">iosGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ff0f3-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ff0f3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff0f3-103">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff0f3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff0f3-104">Prerequisites</span></span>
<span data-ttu-id="ff0f3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff0f3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff0f3-107">Permission type</span></span>|<span data-ttu-id="ff0f3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff0f3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff0f3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff0f3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ff0f3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0f3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff0f3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff0f3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff0f3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff0f3-112">Not supported.</span></span>|
|<span data-ttu-id="ff0f3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-113">Application</span></span>|<span data-ttu-id="ff0f3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff0f3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff0f3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff0f3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff0f3-116">Request headers</span></span>
|<span data-ttu-id="ff0f3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff0f3-117">Header</span></span>|<span data-ttu-id="ff0f3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ff0f3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff0f3-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-119">Authorization</span></span>|<span data-ttu-id="ff0f3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff0f3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff0f3-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ff0f3-121">Accept</span></span>|<span data-ttu-id="ff0f3-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="ff0f3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff0f3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff0f3-123">Request body</span></span>
<span data-ttu-id="ff0f3-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ff0f3-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ff0f3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff0f3-126">Property</span></span>|<span data-ttu-id="ff0f3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ff0f3-127">Type</span></span>|<span data-ttu-id="ff0f3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0f3-129">ID</span><span class="sxs-lookup"><span data-stu-id="ff0f3-129">id</span></span>|<span data-ttu-id="ff0f3-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0f3-130">String</span></span>|<span data-ttu-id="ff0f3-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ff0f3-131">Key of the entity.</span></span> <span data-ttu-id="ff0f3-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff0f3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0f3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ff0f3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0f3-134">DateTimeOffset</span></span>|<span data-ttu-id="ff0f3-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-135">DateTime the object was last modified.</span></span> <span data-ttu-id="ff0f3-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff0f3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0f3-137">createdDateTime</span></span>|<span data-ttu-id="ff0f3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0f3-138">DateTimeOffset</span></span>|<span data-ttu-id="ff0f3-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-139">DateTime the object was created.</span></span> <span data-ttu-id="ff0f3-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff0f3-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-141">description</span></span>|<span data-ttu-id="ff0f3-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0f3-142">String</span></span>|<span data-ttu-id="ff0f3-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff0f3-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff0f3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ff0f3-145">displayName</span></span>|<span data-ttu-id="ff0f3-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0f3-146">String</span></span>|<span data-ttu-id="ff0f3-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff0f3-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff0f3-149">Version</span><span class="sxs-lookup"><span data-stu-id="ff0f3-149">version</span></span>|<span data-ttu-id="ff0f3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-150">Int32</span></span>|<span data-ttu-id="ff0f3-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-151">Version of the device configuration.</span></span> <span data-ttu-id="ff0f3-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff0f3-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-153">accountBlockModification</span></span>|<span data-ttu-id="ff0f3-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-154">Boolean</span></span>|<span data-ttu-id="ff0f3-155">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ff0f3-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ff0f3-157">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-157">Boolean</span></span>|<span data-ttu-id="ff0f3-158">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-159">airDropBlocked</span></span>|<span data-ttu-id="ff0f3-160">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-160">Boolean</span></span>|<span data-ttu-id="ff0f3-161">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ff0f3-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ff0f3-163">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-163">Boolean</span></span>|<span data-ttu-id="ff0f3-164">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ff0f3-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ff0f3-166">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-166">Boolean</span></span>|<span data-ttu-id="ff0f3-167">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ff0f3-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ff0f3-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="ff0f3-169">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-169">Boolean</span></span>|<span data-ttu-id="ff0f3-170">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ff0f3-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ff0f3-172">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-172">Boolean</span></span>|<span data-ttu-id="ff0f3-173">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ff0f3-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-174">appleNewsBlocked</span></span>|<span data-ttu-id="ff0f3-175">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-175">Boolean</span></span>|<span data-ttu-id="ff0f3-176">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ff0f3-177">appsSingleAppModeList</span></span>|<span data-ttu-id="ff0f3-178">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ff0f3-179">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ff0f3-180">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-180">Supervised only.</span></span> <span data-ttu-id="ff0f3-181">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-181">iOS 7.0 and later.</span></span> <span data-ttu-id="ff0f3-182">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ff0f3-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ff0f3-183">appsVisibilityList</span></span>|<span data-ttu-id="ff0f3-184">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ff0f3-185">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ff0f3-186">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ff0f3-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-187">appsVisibilityListType</span></span>|[<span data-ttu-id="ff0f3-188">appListType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="ff0f3-189">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ff0f3-190">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ff0f3-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ff0f3-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ff0f3-192">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-192">Boolean</span></span>|<span data-ttu-id="ff0f3-193">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-194">appStoreBlocked</span></span>|<span data-ttu-id="ff0f3-195">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-195">Boolean</span></span>|<span data-ttu-id="ff0f3-196">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="ff0f3-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ff0f3-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ff0f3-198">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-198">Boolean</span></span>|<span data-ttu-id="ff0f3-199">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ff0f3-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ff0f3-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ff0f3-201">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-201">Boolean</span></span>|<span data-ttu-id="ff0f3-202">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ff0f3-203">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ff0f3-204">appStoreRequirePassword</span></span>|<span data-ttu-id="ff0f3-205">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-205">Boolean</span></span>|<span data-ttu-id="ff0f3-206">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ff0f3-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-207">bluetoothBlockModification</span></span>|<span data-ttu-id="ff0f3-208">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-208">Boolean</span></span>|<span data-ttu-id="ff0f3-209">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-210">cameraBlocked</span></span>|<span data-ttu-id="ff0f3-211">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-211">Boolean</span></span>|<span data-ttu-id="ff0f3-212">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ff0f3-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ff0f3-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ff0f3-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ff0f3-214">Boolean</span></span>|<span data-ttu-id="ff0f3-215">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ff0f3-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ff0f3-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ff0f3-217">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-217">Boolean</span></span>|<span data-ttu-id="ff0f3-218">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ff0f3-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ff0f3-220">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-220">Boolean</span></span>|<span data-ttu-id="ff0f3-221">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ff0f3-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ff0f3-223">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-223">Boolean</span></span>|<span data-ttu-id="ff0f3-224">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ff0f3-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ff0f3-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ff0f3-226">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-226">Boolean</span></span>|<span data-ttu-id="ff0f3-227">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ff0f3-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ff0f3-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ff0f3-229">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-229">Boolean</span></span>|<span data-ttu-id="ff0f3-230">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ff0f3-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ff0f3-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ff0f3-232">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-232">Boolean</span></span>|<span data-ttu-id="ff0f3-233">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ff0f3-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ff0f3-235">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-235">Boolean</span></span>|<span data-ttu-id="ff0f3-236">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ff0f3-237">compliantAppsList</span></span>|<span data-ttu-id="ff0f3-238">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ff0f3-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ff0f3-239">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ff0f3-240">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ff0f3-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-241">compliantAppListType</span></span>|[<span data-ttu-id="ff0f3-242">appListType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="ff0f3-243">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ff0f3-244">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ff0f3-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ff0f3-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ff0f3-246">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-246">Boolean</span></span>|<span data-ttu-id="ff0f3-247">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-248">definitionLookupBlocked</span></span>|<span data-ttu-id="ff0f3-249">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-249">Boolean</span></span>|<span data-ttu-id="ff0f3-250">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ff0f3-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ff0f3-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ff0f3-252">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-252">Boolean</span></span>|<span data-ttu-id="ff0f3-253">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ff0f3-255">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-255">Boolean</span></span>|<span data-ttu-id="ff0f3-256">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-257">deviceBlockNameModification</span></span>|<span data-ttu-id="ff0f3-258">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-258">Boolean</span></span>|<span data-ttu-id="ff0f3-259">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ff0f3-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ff0f3-261">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-261">Boolean</span></span>|<span data-ttu-id="ff0f3-262">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ff0f3-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ff0f3-264">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-264">Boolean</span></span>|<span data-ttu-id="ff0f3-265">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ff0f3-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ff0f3-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ff0f3-267">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-267">Boolean</span></span>|<span data-ttu-id="ff0f3-268">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ff0f3-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ff0f3-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ff0f3-270">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-270">Boolean</span></span>|<span data-ttu-id="ff0f3-271">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ff0f3-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ff0f3-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="ff0f3-273">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ff0f3-273">String collection</span></span>|<span data-ttu-id="ff0f3-274">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ff0f3-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ff0f3-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ff0f3-276">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-276">Boolean</span></span>|<span data-ttu-id="ff0f3-277">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ff0f3-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ff0f3-279">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-279">Boolean</span></span>|<span data-ttu-id="ff0f3-280">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="ff0f3-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-281">faceTimeBlocked</span></span>|<span data-ttu-id="ff0f3-282">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-282">Boolean</span></span>|<span data-ttu-id="ff0f3-283">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="ff0f3-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="ff0f3-285">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-285">Boolean</span></span>|<span data-ttu-id="ff0f3-286">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ff0f3-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ff0f3-288">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-288">Boolean</span></span>|<span data-ttu-id="ff0f3-289">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="ff0f3-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ff0f3-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ff0f3-291">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-291">Boolean</span></span>|<span data-ttu-id="ff0f3-292">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="ff0f3-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-293">gameCenterBlocked</span></span>|<span data-ttu-id="ff0f3-294">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-294">Boolean</span></span>|<span data-ttu-id="ff0f3-295">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-296">hostPairingBlocked</span></span>|<span data-ttu-id="ff0f3-297">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-297">Boolean</span></span>|<span data-ttu-id="ff0f3-298">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="ff0f3-300">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-300">Boolean</span></span>|<span data-ttu-id="ff0f3-301">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ff0f3-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ff0f3-303">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-303">Boolean</span></span>|<span data-ttu-id="ff0f3-304">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ff0f3-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ff0f3-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ff0f3-306">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-306">Boolean</span></span>|<span data-ttu-id="ff0f3-307">Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ff0f3-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ff0f3-308">iCloudBlockBackup</span></span>|<span data-ttu-id="ff0f3-309">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-309">Boolean</span></span>|<span data-ttu-id="ff0f3-310">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="ff0f3-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ff0f3-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ff0f3-312">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-312">Boolean</span></span>|<span data-ttu-id="ff0f3-313">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ff0f3-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ff0f3-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ff0f3-315">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-315">Boolean</span></span>|<span data-ttu-id="ff0f3-316">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ff0f3-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ff0f3-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ff0f3-318">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-318">Boolean</span></span>|<span data-ttu-id="ff0f3-319">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ff0f3-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ff0f3-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ff0f3-321">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-321">Boolean</span></span>|<span data-ttu-id="ff0f3-322">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ff0f3-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ff0f3-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ff0f3-324">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-324">Boolean</span></span>|<span data-ttu-id="ff0f3-325">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ff0f3-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ff0f3-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ff0f3-327">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-327">Boolean</span></span>|<span data-ttu-id="ff0f3-328">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ff0f3-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ff0f3-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ff0f3-330">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-330">Boolean</span></span>|<span data-ttu-id="ff0f3-331">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="ff0f3-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ff0f3-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="ff0f3-333">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-333">Boolean</span></span>|<span data-ttu-id="ff0f3-334">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ff0f3-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ff0f3-335">iTunesBlockRadio</span></span>|<span data-ttu-id="ff0f3-336">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-336">Boolean</span></span>|<span data-ttu-id="ff0f3-337">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ff0f3-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ff0f3-339">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-339">Boolean</span></span>|<span data-ttu-id="ff0f3-340">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ff0f3-341">keyboardBlockDictation</span></span>|<span data-ttu-id="ff0f3-342">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-342">Boolean</span></span>|<span data-ttu-id="ff0f3-343">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ff0f3-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="ff0f3-345">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-345">Boolean</span></span>|<span data-ttu-id="ff0f3-346">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ff0f3-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ff0f3-348">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-348">Boolean</span></span>|<span data-ttu-id="ff0f3-349">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ff0f3-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ff0f3-351">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-351">Boolean</span></span>|<span data-ttu-id="ff0f3-352">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ff0f3-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ff0f3-354">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-354">Boolean</span></span>|<span data-ttu-id="ff0f3-355">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ff0f3-357">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-357">Boolean</span></span>|<span data-ttu-id="ff0f3-358">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ff0f3-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ff0f3-360">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-360">Boolean</span></span>|<span data-ttu-id="ff0f3-361">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ff0f3-363">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-363">Boolean</span></span>|<span data-ttu-id="ff0f3-364">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ff0f3-366">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-366">Boolean</span></span>|<span data-ttu-id="ff0f3-367">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ff0f3-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ff0f3-369">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-369">Boolean</span></span>|<span data-ttu-id="ff0f3-370">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ff0f3-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ff0f3-372">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-372">Boolean</span></span>|<span data-ttu-id="ff0f3-373">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ff0f3-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ff0f3-375">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-375">Boolean</span></span>|<span data-ttu-id="ff0f3-376">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ff0f3-378">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-378">Boolean</span></span>|<span data-ttu-id="ff0f3-379">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ff0f3-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ff0f3-381">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-381">Boolean</span></span>|<span data-ttu-id="ff0f3-382">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ff0f3-384">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-384">Boolean</span></span>|<span data-ttu-id="ff0f3-385">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ff0f3-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ff0f3-387">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0f3-387">String</span></span>|<span data-ttu-id="ff0f3-388">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ff0f3-389">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ff0f3-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="ff0f3-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="ff0f3-391">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0f3-391">String</span></span>|<span data-ttu-id="ff0f3-392">ID für integrierte Apps für die Verwendung im Kioskmodus.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="ff0f3-393">Wird verwendet, wenn KioskModeManagedAppId und KioskModeAppStoreUrl nicht festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="ff0f3-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ff0f3-395">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-395">Boolean</span></span>|<span data-ttu-id="ff0f3-396">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ff0f3-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ff0f3-398">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-398">Boolean</span></span>|<span data-ttu-id="ff0f3-399">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ff0f3-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ff0f3-401">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-401">Boolean</span></span>|<span data-ttu-id="ff0f3-402">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ff0f3-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ff0f3-404">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-404">Boolean</span></span>|<span data-ttu-id="ff0f3-405">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ff0f3-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="ff0f3-407">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-407">Boolean</span></span>|<span data-ttu-id="ff0f3-408">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ff0f3-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ff0f3-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="ff0f3-410">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff0f3-410">String</span></span>|<span data-ttu-id="ff0f3-411">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ff0f3-412">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ff0f3-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ff0f3-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ff0f3-414">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-414">Boolean</span></span>|<span data-ttu-id="ff0f3-415">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ff0f3-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ff0f3-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ff0f3-417">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-417">Boolean</span></span>|<span data-ttu-id="ff0f3-418">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ff0f3-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ff0f3-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ff0f3-420">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-420">Boolean</span></span>|<span data-ttu-id="ff0f3-421">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ff0f3-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ff0f3-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ff0f3-423">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-423">Boolean</span></span>|<span data-ttu-id="ff0f3-424">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ff0f3-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ff0f3-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ff0f3-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ff0f3-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="ff0f3-427">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="ff0f3-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ff0f3-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ff0f3-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ff0f3-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ff0f3-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="ff0f3-430">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="ff0f3-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ff0f3-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ff0f3-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ff0f3-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ff0f3-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="ff0f3-433">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="ff0f3-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="ff0f3-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ff0f3-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ff0f3-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ff0f3-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="ff0f3-436">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="ff0f3-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ff0f3-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ff0f3-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ff0f3-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ff0f3-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="ff0f3-439">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="ff0f3-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ff0f3-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ff0f3-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ff0f3-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ff0f3-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="ff0f3-442">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="ff0f3-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ff0f3-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ff0f3-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ff0f3-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ff0f3-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="ff0f3-445">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="ff0f3-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ff0f3-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ff0f3-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ff0f3-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ff0f3-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="ff0f3-448">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="ff0f3-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ff0f3-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ff0f3-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ff0f3-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ff0f3-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="ff0f3-451">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="ff0f3-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ff0f3-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ff0f3-452">networkUsageRules</span></span>|<span data-ttu-id="ff0f3-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ff0f3-454">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ff0f3-455">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ff0f3-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ff0f3-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="ff0f3-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="ff0f3-458">Medieninhalt-Bewertungseinstellungen für Apps.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-458">Media content rating settings for Canada</span></span> <span data-ttu-id="ff0f3-459">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ff0f3-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-460">messagesBlocked</span></span>|<span data-ttu-id="ff0f3-461">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-461">Boolean</span></span>|<span data-ttu-id="ff0f3-462">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ff0f3-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ff0f3-464">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-464">Boolean</span></span>|<span data-ttu-id="ff0f3-465">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ff0f3-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ff0f3-467">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-467">Boolean</span></span>|<span data-ttu-id="ff0f3-468">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ff0f3-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ff0f3-470">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-470">Boolean</span></span>|<span data-ttu-id="ff0f3-471">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ff0f3-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-472">passcodeBlockModification</span></span>|<span data-ttu-id="ff0f3-473">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-473">Boolean</span></span>|<span data-ttu-id="ff0f3-474">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ff0f3-475">passcodeBlockSimple</span></span>|<span data-ttu-id="ff0f3-476">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-476">Boolean</span></span>|<span data-ttu-id="ff0f3-477">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ff0f3-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ff0f3-478">passcodeExpirationDays</span></span>|<span data-ttu-id="ff0f3-479">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-479">Int32</span></span>|<span data-ttu-id="ff0f3-480">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="ff0f3-481">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ff0f3-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ff0f3-482">passcodeMinimumLength</span></span>|<span data-ttu-id="ff0f3-483">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-483">Int32</span></span>|<span data-ttu-id="ff0f3-484">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-484">Minimum length of passcode.</span></span> <span data-ttu-id="ff0f3-485">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ff0f3-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ff0f3-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ff0f3-487">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-487">Int32</span></span>|<span data-ttu-id="ff0f3-488">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ff0f3-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ff0f3-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ff0f3-490">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-490">Int32</span></span>|<span data-ttu-id="ff0f3-491">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ff0f3-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ff0f3-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ff0f3-493">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-493">Int32</span></span>|<span data-ttu-id="ff0f3-494">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="ff0f3-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ff0f3-495">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ff0f3-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ff0f3-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ff0f3-497">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-497">Int32</span></span>|<span data-ttu-id="ff0f3-498">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="ff0f3-499">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ff0f3-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ff0f3-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ff0f3-501">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0f3-501">Int32</span></span>|<span data-ttu-id="ff0f3-502">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ff0f3-503">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ff0f3-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-504">passcodeRequiredType</span></span>|[<span data-ttu-id="ff0f3-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ff0f3-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="ff0f3-506">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-506">Type of passcode that is required.</span></span> <span data-ttu-id="ff0f3-507">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ff0f3-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ff0f3-508">passcodeRequired</span></span>|<span data-ttu-id="ff0f3-509">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-509">Boolean</span></span>|<span data-ttu-id="ff0f3-510">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ff0f3-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-511">podcastsBlocked</span></span>|<span data-ttu-id="ff0f3-512">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-512">Boolean</span></span>|<span data-ttu-id="ff0f3-513">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ff0f3-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ff0f3-514">safariBlockAutofill</span></span>|<span data-ttu-id="ff0f3-515">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-515">Boolean</span></span>|<span data-ttu-id="ff0f3-516">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ff0f3-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ff0f3-517">safariBlockJavaScript</span></span>|<span data-ttu-id="ff0f3-518">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-518">Boolean</span></span>|<span data-ttu-id="ff0f3-519">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ff0f3-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ff0f3-520">safariBlockPopups</span></span>|<span data-ttu-id="ff0f3-521">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-521">Boolean</span></span>|<span data-ttu-id="ff0f3-522">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ff0f3-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-523">safariBlocked</span></span>|<span data-ttu-id="ff0f3-524">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-524">Boolean</span></span>|<span data-ttu-id="ff0f3-525">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="ff0f3-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-526">safariCookieSettings</span></span>|[<span data-ttu-id="ff0f3-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ff0f3-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="ff0f3-528">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-528">Cookie settings for Safari.</span></span> <span data-ttu-id="ff0f3-529">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ff0f3-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ff0f3-530">safariManagedDomains</span></span>|<span data-ttu-id="ff0f3-531">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-531">String collection</span></span>|<span data-ttu-id="ff0f3-532">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ff0f3-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ff0f3-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ff0f3-534">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-534">String collection</span></span>|<span data-ttu-id="ff0f3-535">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ff0f3-536">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ff0f3-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ff0f3-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ff0f3-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="ff0f3-538">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-538">Boolean</span></span>|<span data-ttu-id="ff0f3-539">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ff0f3-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-540">screenCaptureBlocked</span></span>|<span data-ttu-id="ff0f3-541">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-541">Boolean</span></span>|<span data-ttu-id="ff0f3-542">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ff0f3-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-543">siriBlocked</span></span>|<span data-ttu-id="ff0f3-544">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-544">Boolean</span></span>|<span data-ttu-id="ff0f3-545">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ff0f3-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ff0f3-547">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-547">Boolean</span></span>|<span data-ttu-id="ff0f3-548">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ff0f3-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ff0f3-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ff0f3-550">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-550">Boolean</span></span>|<span data-ttu-id="ff0f3-551">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ff0f3-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ff0f3-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ff0f3-553">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-553">Boolean</span></span>|<span data-ttu-id="ff0f3-554">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ff0f3-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ff0f3-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ff0f3-556">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-556">Boolean</span></span>|<span data-ttu-id="ff0f3-557">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ff0f3-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ff0f3-558">voiceDialingBlocked</span></span>|<span data-ttu-id="ff0f3-559">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-559">Boolean</span></span>|<span data-ttu-id="ff0f3-560">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ff0f3-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ff0f3-561">wallpaperBlockModification</span></span>|<span data-ttu-id="ff0f3-562">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-562">Boolean</span></span>|<span data-ttu-id="ff0f3-563">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ff0f3-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ff0f3-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ff0f3-565">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff0f3-565">Boolean</span></span>|<span data-ttu-id="ff0f3-566">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="ff0f3-567">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff0f3-567">Response</span></span>
<span data-ttu-id="ff0f3-568">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-568">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff0f3-569">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff0f3-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff0f3-570">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff0f3-570">Request</span></span>
<span data-ttu-id="ff0f3-571">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-571">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7837

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

### <a name="response"></a><span data-ttu-id="ff0f3-572">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff0f3-572">Response</span></span>
<span data-ttu-id="ff0f3-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff0f3-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








