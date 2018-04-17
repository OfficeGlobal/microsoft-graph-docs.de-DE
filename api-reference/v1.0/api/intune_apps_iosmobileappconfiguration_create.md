# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="3f1a3-101">iosMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="3f1a3-101">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="3f1a3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f1a3-103">Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-103">Create a new [managedMobileApp](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f1a3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3f1a3-104">Prerequisites</span></span>
<span data-ttu-id="3f1a3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3f1a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3f1a3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f1a3-107">Permission type</span></span>|<span data-ttu-id="3f1a3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f1a3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3f1a3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f1a3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3f1a3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f1a3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f1a3-112">Not supported.</span></span>|
|<span data-ttu-id="3f1a3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3f1a3-113">Application</span></span>|<span data-ttu-id="3f1a3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f1a3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f1a3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f1a3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f1a3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f1a3-116">Request headers</span></span>
|<span data-ttu-id="3f1a3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3f1a3-117">Header</span></span>|<span data-ttu-id="3f1a3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3f1a3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f1a3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f1a3-119">Authorization</span></span>|<span data-ttu-id="3f1a3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3f1a3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f1a3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3f1a3-121">Accept</span></span>|<span data-ttu-id="3f1a3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3f1a3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f1a3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3f1a3-123">Request body</span></span>
<span data-ttu-id="3f1a3-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs iosMobileAppConfiguration an.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="3f1a3-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="3f1a3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3f1a3-126">Property</span></span>|<span data-ttu-id="3f1a3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3f1a3-127">Type</span></span>|<span data-ttu-id="3f1a3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f1a3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f1a3-129">id</span><span class="sxs-lookup"><span data-stu-id="3f1a3-129">id</span></span>|<span data-ttu-id="3f1a3-130">String</span><span class="sxs-lookup"><span data-stu-id="3f1a3-130">String</span></span>|<span data-ttu-id="3f1a3-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-131">Key of the entity.</span></span> <span data-ttu-id="3f1a3-132">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3f1a3-133">targetedMobileApps</span></span>|<span data-ttu-id="3f1a3-134">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3f1a3-134">String collection</span></span>|<span data-ttu-id="3f1a3-135">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-135">the associated app.</span></span> <span data-ttu-id="3f1a3-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f1a3-137">createdDateTime</span></span>|<span data-ttu-id="3f1a3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f1a3-138">DateTimeOffset</span></span>|<span data-ttu-id="3f1a3-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-139">DateTime the object was created.</span></span> <span data-ttu-id="3f1a3-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-141">description</span><span class="sxs-lookup"><span data-stu-id="3f1a3-141">description</span></span>|<span data-ttu-id="3f1a3-142">String</span><span class="sxs-lookup"><span data-stu-id="3f1a3-142">String</span></span>|<span data-ttu-id="3f1a3-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3f1a3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f1a3-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f1a3-145">lastModifiedDateTime</span></span>|<span data-ttu-id="3f1a3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f1a3-146">DateTimeOffset</span></span>|<span data-ttu-id="3f1a3-147">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-147">DateTime the object was last modified.</span></span> <span data-ttu-id="3f1a3-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="3f1a3-149">displayName</span></span>|<span data-ttu-id="3f1a3-150">String</span><span class="sxs-lookup"><span data-stu-id="3f1a3-150">String</span></span>|<span data-ttu-id="3f1a3-151">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3f1a3-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f1a3-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-153">version</span><span class="sxs-lookup"><span data-stu-id="3f1a3-153">version</span></span>|<span data-ttu-id="3f1a3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3f1a3-154">Int32</span></span>|<span data-ttu-id="3f1a3-155">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-155">Version of the device configuration.</span></span> <span data-ttu-id="3f1a3-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f1a3-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3f1a3-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="3f1a3-157">encodedSettingXml</span></span>|<span data-ttu-id="3f1a3-158">Binary</span><span class="sxs-lookup"><span data-stu-id="3f1a3-158">Binary</span></span>|<span data-ttu-id="3f1a3-159">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="3f1a3-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="3f1a3-160">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="3f1a3-160">settings</span></span>|<span data-ttu-id="3f1a3-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3f1a3-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="3f1a3-162">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="3f1a3-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="3f1a3-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f1a3-163">Response</span></span>
<span data-ttu-id="3f1a3-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-164">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f1a3-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f1a3-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f1a3-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f1a3-166">Request</span></span>
<span data-ttu-id="3f1a3-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 598

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="3f1a3-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f1a3-168">Response</span></span>
<span data-ttu-id="3f1a3-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f1a3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



