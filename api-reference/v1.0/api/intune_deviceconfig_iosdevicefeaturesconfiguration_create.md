# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="9ed48-101">Erstellen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="9ed48-101">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="9ed48-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ed48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ed48-103">Diese Methode erstellt ein neues Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-103">Create a new [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ed48-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ed48-104">Prerequisites</span></span>
<span data-ttu-id="9ed48-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ed48-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ed48-107">Permission type</span></span>|<span data-ttu-id="9ed48-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ed48-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ed48-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ed48-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9ed48-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed48-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ed48-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ed48-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ed48-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ed48-112">Not supported.</span></span>|
|<span data-ttu-id="9ed48-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ed48-113">Application</span></span>|<span data-ttu-id="9ed48-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ed48-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ed48-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ed48-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ed48-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ed48-116">Request headers</span></span>
|<span data-ttu-id="9ed48-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ed48-117">Header</span></span>|<span data-ttu-id="9ed48-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9ed48-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ed48-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed48-119">Authorization</span></span>|<span data-ttu-id="9ed48-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ed48-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ed48-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9ed48-121">Accept</span></span>|<span data-ttu-id="9ed48-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9ed48-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ed48-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ed48-123">Request body</span></span>
<span data-ttu-id="9ed48-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="9ed48-124">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="9ed48-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9ed48-125">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="9ed48-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ed48-126">Property</span></span>|<span data-ttu-id="9ed48-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9ed48-127">Type</span></span>|<span data-ttu-id="9ed48-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ed48-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed48-129">id</span><span class="sxs-lookup"><span data-stu-id="9ed48-129">id</span></span>|<span data-ttu-id="9ed48-130">String</span><span class="sxs-lookup"><span data-stu-id="9ed48-130">String</span></span>|<span data-ttu-id="9ed48-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="9ed48-131">Key of the entity.</span></span> <span data-ttu-id="9ed48-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ed48-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed48-133">lastModifiedDateTime</span></span>|<span data-ttu-id="9ed48-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed48-134">DateTimeOffset</span></span>|<span data-ttu-id="9ed48-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ed48-135">DateTime the object was last modified.</span></span> <span data-ttu-id="9ed48-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ed48-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed48-137">createdDateTime</span></span>|<span data-ttu-id="9ed48-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed48-138">DateTimeOffset</span></span>|<span data-ttu-id="9ed48-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ed48-139">DateTime the object was created.</span></span> <span data-ttu-id="9ed48-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ed48-141">description</span><span class="sxs-lookup"><span data-stu-id="9ed48-141">description</span></span>|<span data-ttu-id="9ed48-142">String</span><span class="sxs-lookup"><span data-stu-id="9ed48-142">String</span></span>|<span data-ttu-id="9ed48-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9ed48-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ed48-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ed48-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9ed48-145">displayName</span></span>|<span data-ttu-id="9ed48-146">String</span><span class="sxs-lookup"><span data-stu-id="9ed48-146">String</span></span>|<span data-ttu-id="9ed48-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9ed48-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ed48-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ed48-149">version</span><span class="sxs-lookup"><span data-stu-id="9ed48-149">version</span></span>|<span data-ttu-id="9ed48-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9ed48-150">Int32</span></span>|<span data-ttu-id="9ed48-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ed48-151">Version of the device configuration.</span></span> <span data-ttu-id="9ed48-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ed48-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ed48-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="9ed48-153">assetTagTemplate</span></span>|<span data-ttu-id="9ed48-154">String</span><span class="sxs-lookup"><span data-stu-id="9ed48-154">String</span></span>|<span data-ttu-id="9ed48-155">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9ed48-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="9ed48-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="9ed48-156">lockScreenFootnote</span></span>|<span data-ttu-id="9ed48-157">String</span><span class="sxs-lookup"><span data-stu-id="9ed48-157">String</span></span>|<span data-ttu-id="9ed48-158">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9ed48-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="9ed48-159">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="9ed48-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="9ed48-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="9ed48-160">homeScreenDockIcons</span></span>|<span data-ttu-id="9ed48-161">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="9ed48-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="9ed48-162">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9ed48-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="9ed48-163">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9ed48-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9ed48-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="9ed48-164">homeScreenPages</span></span>|<span data-ttu-id="9ed48-165">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="9ed48-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="9ed48-166">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="9ed48-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="9ed48-167">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9ed48-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9ed48-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="9ed48-168">notificationSettings</span></span>|<span data-ttu-id="9ed48-169">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9ed48-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="9ed48-170">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="9ed48-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="9ed48-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9ed48-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="9ed48-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ed48-172">Response</span></span>
<span data-ttu-id="9ed48-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ed48-173">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ed48-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ed48-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ed48-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ed48-175">Request</span></span>
<span data-ttu-id="9ed48-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ed48-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="9ed48-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ed48-177">Response</span></span>
<span data-ttu-id="9ed48-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ed48-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



