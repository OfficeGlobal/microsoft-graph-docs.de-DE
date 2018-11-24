# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="635da-101">Aktualisieren von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="635da-101">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="635da-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="635da-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="635da-103">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="635da-103">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="635da-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="635da-104">Prerequisites</span></span>
<span data-ttu-id="635da-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="635da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="635da-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="635da-107">Permission type</span></span>|<span data-ttu-id="635da-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="635da-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="635da-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="635da-109">Delegated (work or school account)</span></span>|<span data-ttu-id="635da-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="635da-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="635da-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="635da-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="635da-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="635da-112">Not supported.</span></span>|
|<span data-ttu-id="635da-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="635da-113">Application</span></span>|<span data-ttu-id="635da-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="635da-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="635da-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="635da-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="635da-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="635da-116">Request headers</span></span>
|<span data-ttu-id="635da-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="635da-117">Header</span></span>|<span data-ttu-id="635da-118">Wert</span><span class="sxs-lookup"><span data-stu-id="635da-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="635da-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="635da-119">Authorization</span></span>|<span data-ttu-id="635da-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="635da-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="635da-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="635da-121">Accept</span></span>|<span data-ttu-id="635da-122">application/json</span><span class="sxs-lookup"><span data-stu-id="635da-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="635da-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="635da-123">Request body</span></span>
<span data-ttu-id="635da-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="635da-124">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="635da-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="635da-125">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="635da-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="635da-126">Property</span></span>|<span data-ttu-id="635da-127">Typ</span><span class="sxs-lookup"><span data-stu-id="635da-127">Type</span></span>|<span data-ttu-id="635da-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="635da-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="635da-129">id</span><span class="sxs-lookup"><span data-stu-id="635da-129">id</span></span>|<span data-ttu-id="635da-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="635da-130">String</span></span>|<span data-ttu-id="635da-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="635da-131">Key of the entity.</span></span> <span data-ttu-id="635da-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="635da-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="635da-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="635da-133">lastModifiedDateTime</span></span>|<span data-ttu-id="635da-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="635da-134">DateTimeOffset</span></span>|<span data-ttu-id="635da-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="635da-135">DateTime the object was last modified.</span></span> <span data-ttu-id="635da-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="635da-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="635da-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="635da-137">createdDateTime</span></span>|<span data-ttu-id="635da-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="635da-138">DateTimeOffset</span></span>|<span data-ttu-id="635da-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="635da-139">DateTime the object was created.</span></span> <span data-ttu-id="635da-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="635da-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="635da-141">description</span><span class="sxs-lookup"><span data-stu-id="635da-141">description</span></span>|<span data-ttu-id="635da-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="635da-142">String</span></span>|<span data-ttu-id="635da-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="635da-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="635da-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="635da-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="635da-145">displayName</span><span class="sxs-lookup"><span data-stu-id="635da-145">displayName</span></span>|<span data-ttu-id="635da-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="635da-146">String</span></span>|<span data-ttu-id="635da-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="635da-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="635da-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="635da-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="635da-149">Version</span><span class="sxs-lookup"><span data-stu-id="635da-149">version</span></span>|<span data-ttu-id="635da-150">Int32</span><span class="sxs-lookup"><span data-stu-id="635da-150">Int32</span></span>|<span data-ttu-id="635da-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="635da-151">Version of the device configuration.</span></span> <span data-ttu-id="635da-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="635da-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="635da-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="635da-153">assetTagTemplate</span></span>|<span data-ttu-id="635da-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="635da-154">String</span></span>|<span data-ttu-id="635da-155">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="635da-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="635da-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="635da-156">lockScreenFootnote</span></span>|<span data-ttu-id="635da-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="635da-157">String</span></span>|<span data-ttu-id="635da-158">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="635da-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="635da-159">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="635da-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="635da-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="635da-160">homeScreenDockIcons</span></span>|<span data-ttu-id="635da-161">Sammlung von Objekten des Typs [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="635da-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="635da-162">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="635da-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="635da-163">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="635da-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="635da-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="635da-164">homeScreenPages</span></span>|<span data-ttu-id="635da-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="635da-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="635da-166">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="635da-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="635da-167">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="635da-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="635da-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="635da-168">notificationSettings</span></span>|<span data-ttu-id="635da-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="635da-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="635da-170">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="635da-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="635da-171">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="635da-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="635da-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="635da-172">Response</span></span>
<span data-ttu-id="635da-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="635da-173">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="635da-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="635da-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="635da-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="635da-175">Request</span></span>
<span data-ttu-id="635da-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="635da-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="635da-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="635da-177">Response</span></span>
<span data-ttu-id="635da-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="635da-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```



