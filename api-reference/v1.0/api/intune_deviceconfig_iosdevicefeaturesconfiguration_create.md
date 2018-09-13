# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="a5748-101">Erstellen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a5748-101">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a5748-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a5748-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5748-103">Diese Methode erstellt ein neues Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-103">Create a new [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5748-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5748-104">Prerequisites</span></span>
<span data-ttu-id="a5748-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5748-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5748-107">Permission type</span></span>|<span data-ttu-id="a5748-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5748-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5748-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5748-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a5748-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5748-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5748-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5748-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5748-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5748-112">Not supported.</span></span>|
|<span data-ttu-id="a5748-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5748-113">Application</span></span>|<span data-ttu-id="a5748-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5748-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5748-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5748-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a5748-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5748-116">Request headers</span></span>
|<span data-ttu-id="a5748-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5748-117">Header</span></span>|<span data-ttu-id="a5748-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a5748-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5748-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a5748-119">Authorization</span></span>|<span data-ttu-id="a5748-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5748-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5748-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="a5748-121">Accept</span></span>|<span data-ttu-id="a5748-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="a5748-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5748-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5748-123">Request body</span></span>
<span data-ttu-id="a5748-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="a5748-124">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="a5748-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a5748-125">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="a5748-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5748-126">Property</span></span>|<span data-ttu-id="a5748-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a5748-127">Type</span></span>|<span data-ttu-id="a5748-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5748-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5748-129">ID</span><span class="sxs-lookup"><span data-stu-id="a5748-129">id</span></span>|<span data-ttu-id="a5748-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5748-130">String</span></span>|<span data-ttu-id="a5748-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a5748-131">Key of the entity.</span></span> <span data-ttu-id="a5748-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5748-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5748-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a5748-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5748-134">DateTimeOffset</span></span>|<span data-ttu-id="a5748-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5748-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a5748-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5748-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5748-137">createdDateTime</span></span>|<span data-ttu-id="a5748-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5748-138">DateTimeOffset</span></span>|<span data-ttu-id="a5748-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5748-139">DateTime the object was created.</span></span> <span data-ttu-id="a5748-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5748-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5748-141">description</span></span>|<span data-ttu-id="a5748-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5748-142">String</span></span>|<span data-ttu-id="a5748-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a5748-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5748-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5748-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a5748-145">displayName</span></span>|<span data-ttu-id="a5748-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5748-146">String</span></span>|<span data-ttu-id="a5748-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a5748-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5748-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5748-149">Version</span><span class="sxs-lookup"><span data-stu-id="a5748-149">version</span></span>|<span data-ttu-id="a5748-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a5748-150">Int32</span></span>|<span data-ttu-id="a5748-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5748-151">Version of the device configuration.</span></span> <span data-ttu-id="a5748-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5748-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5748-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="a5748-153">assetTagTemplate</span></span>|<span data-ttu-id="a5748-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5748-154">String</span></span>|<span data-ttu-id="a5748-155">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a5748-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="a5748-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="a5748-156">lockScreenFootnote</span></span>|<span data-ttu-id="a5748-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5748-157">String</span></span>|<span data-ttu-id="a5748-158">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="a5748-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="a5748-159">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="a5748-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="a5748-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="a5748-160">homeScreenDockIcons</span></span>|<span data-ttu-id="a5748-161">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a5748-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a5748-162">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a5748-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="a5748-163">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5748-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a5748-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="a5748-164">homeScreenPages</span></span>|<span data-ttu-id="a5748-165">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="a5748-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="a5748-166">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="a5748-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="a5748-167">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5748-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a5748-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="a5748-168">notificationSettings</span></span>|<span data-ttu-id="a5748-169">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a5748-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="a5748-170">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="a5748-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="a5748-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a5748-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a5748-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5748-172">Response</span></span>
<span data-ttu-id="a5748-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a5748-173">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5748-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5748-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5748-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5748-175">Request</span></span>
<span data-ttu-id="a5748-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5748-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2052

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="a5748-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5748-177">Response</span></span>
<span data-ttu-id="a5748-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5748-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








