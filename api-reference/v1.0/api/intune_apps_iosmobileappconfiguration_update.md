# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="bcde6-101">IosMobileAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bcde6-101">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="bcde6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bcde6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcde6-103">Aktualisieren der Eigenschaften eines [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bcde6-103">Update the properties of a [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcde6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bcde6-104">Prerequisites</span></span>
<span data-ttu-id="bcde6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bcde6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bcde6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bcde6-107">Permission type</span></span>|<span data-ttu-id="bcde6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bcde6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcde6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bcde6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bcde6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcde6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bcde6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bcde6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcde6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcde6-112">Not supported.</span></span>|
|<span data-ttu-id="bcde6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bcde6-113">Application</span></span>|<span data-ttu-id="bcde6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcde6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcde6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcde6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bcde6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bcde6-116">Request headers</span></span>
|<span data-ttu-id="bcde6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bcde6-117">Header</span></span>|<span data-ttu-id="bcde6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="bcde6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcde6-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bcde6-119">Authorization</span></span>|<span data-ttu-id="bcde6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bcde6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcde6-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="bcde6-121">Accept</span></span>|<span data-ttu-id="bcde6-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="bcde6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcde6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bcde6-123">Request body</span></span>
<span data-ttu-id="bcde6-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="bcde6-124">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="bcde6-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bcde6-125">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="bcde6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bcde6-126">Property</span></span>|<span data-ttu-id="bcde6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="bcde6-127">Type</span></span>|<span data-ttu-id="bcde6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcde6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcde6-129">ID</span><span class="sxs-lookup"><span data-stu-id="bcde6-129">id</span></span>|<span data-ttu-id="bcde6-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bcde6-130">String</span></span>|<span data-ttu-id="bcde6-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="bcde6-131">Key of the entity.</span></span> <span data-ttu-id="bcde6-132">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="bcde6-133">targetedMobileApps</span></span>|<span data-ttu-id="bcde6-134">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bcde6-134">String collection</span></span>|<span data-ttu-id="bcde6-135">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="bcde6-135">the associated app.</span></span> <span data-ttu-id="bcde6-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bcde6-137">createdDateTime</span></span>|<span data-ttu-id="bcde6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcde6-138">DateTimeOffset</span></span>|<span data-ttu-id="bcde6-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bcde6-139">DateTime the object was created.</span></span> <span data-ttu-id="bcde6-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcde6-141">description</span></span>|<span data-ttu-id="bcde6-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bcde6-142">String</span></span>|<span data-ttu-id="bcde6-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bcde6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bcde6-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcde6-145">lastModifiedDateTime</span></span>|<span data-ttu-id="bcde6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcde6-146">DateTimeOffset</span></span>|<span data-ttu-id="bcde6-147">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bcde6-147">DateTime the object was last modified.</span></span> <span data-ttu-id="bcde6-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-149">displayName</span><span class="sxs-lookup"><span data-stu-id="bcde6-149">displayName</span></span>|<span data-ttu-id="bcde6-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bcde6-150">String</span></span>|<span data-ttu-id="bcde6-151">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bcde6-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bcde6-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-153">version</span><span class="sxs-lookup"><span data-stu-id="bcde6-153">version</span></span>|<span data-ttu-id="bcde6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="bcde6-154">Int32</span></span>|<span data-ttu-id="bcde6-155">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bcde6-155">Version of the device configuration.</span></span> <span data-ttu-id="bcde6-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcde6-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bcde6-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="bcde6-157">encodedSettingXml</span></span>|<span data-ttu-id="bcde6-158">Binär</span><span class="sxs-lookup"><span data-stu-id="bcde6-158">Binary</span></span>|<span data-ttu-id="bcde6-159">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="bcde6-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="bcde6-160">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="bcde6-160">settings</span></span>|<span data-ttu-id="bcde6-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bcde6-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="bcde6-162">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="bcde6-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="bcde6-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcde6-163">Response</span></span>
<span data-ttu-id="bcde6-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bcde6-164">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcde6-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bcde6-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcde6-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcde6-166">Request</span></span>
<span data-ttu-id="bcde6-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bcde6-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bcde6-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcde6-168">Response</span></span>
<span data-ttu-id="bcde6-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcde6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```








