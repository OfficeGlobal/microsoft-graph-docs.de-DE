# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e04e9-101">Aktualisieren von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e04e9-101">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e04e9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e04e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e04e9-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-103">Update the properties of a [calendar](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e04e9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e04e9-104">Prerequisites</span></span>
<span data-ttu-id="e04e9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e04e9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e04e9-107">Permission type</span></span>|<span data-ttu-id="e04e9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e04e9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e04e9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e04e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e04e9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04e9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e04e9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e04e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e04e9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e04e9-112">Not supported.</span></span>|
|<span data-ttu-id="e04e9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e04e9-113">Application</span></span>|<span data-ttu-id="e04e9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e04e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e04e9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e04e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e04e9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e04e9-116">Request headers</span></span>
|<span data-ttu-id="e04e9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e04e9-117">Header</span></span>|<span data-ttu-id="e04e9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e04e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e04e9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e04e9-119">Authorization</span></span>|<span data-ttu-id="e04e9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e04e9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e04e9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e04e9-121">Accept</span></span>|<span data-ttu-id="e04e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e04e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e04e9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e04e9-123">Request body</span></span>
<span data-ttu-id="e04e9-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="e04e9-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="e04e9-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e04e9-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="e04e9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e04e9-126">Property</span></span>|<span data-ttu-id="e04e9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e04e9-127">Type</span></span>|<span data-ttu-id="e04e9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e04e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e04e9-129">id</span><span class="sxs-lookup"><span data-stu-id="e04e9-129">id</span></span>|<span data-ttu-id="e04e9-130">String</span><span class="sxs-lookup"><span data-stu-id="e04e9-130">String</span></span>|<span data-ttu-id="e04e9-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="e04e9-131">Key of the setting.</span></span> <span data-ttu-id="e04e9-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e04e9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e04e9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e04e9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e04e9-134">DateTimeOffset</span></span>|<span data-ttu-id="e04e9-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e04e9-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="e04e9-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e04e9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e04e9-137">createdDateTime</span></span>|<span data-ttu-id="e04e9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e04e9-138">DateTimeOffset</span></span>|<span data-ttu-id="e04e9-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e04e9-139">DateTime the object was created.</span></span> <span data-ttu-id="e04e9-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e04e9-141">description</span><span class="sxs-lookup"><span data-stu-id="e04e9-141">description</span></span>|<span data-ttu-id="e04e9-142">String</span><span class="sxs-lookup"><span data-stu-id="e04e9-142">String</span></span>|<span data-ttu-id="e04e9-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e04e9-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e04e9-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e04e9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e04e9-145">displayName</span></span>|<span data-ttu-id="e04e9-146">String</span><span class="sxs-lookup"><span data-stu-id="e04e9-146">String</span></span>|<span data-ttu-id="e04e9-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e04e9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e04e9-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e04e9-149">version</span><span class="sxs-lookup"><span data-stu-id="e04e9-149">version</span></span>|<span data-ttu-id="e04e9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e04e9-150">Int32</span></span>|<span data-ttu-id="e04e9-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e04e9-151">Version of the device configuration.</span></span> <span data-ttu-id="e04e9-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e04e9-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e04e9-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="e04e9-153">Response</span></span>
<span data-ttu-id="e04e9-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e04e9-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e04e9-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e04e9-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="e04e9-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e04e9-156">Request</span></span>
<span data-ttu-id="e04e9-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e04e9-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 163

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="e04e9-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="e04e9-158">Response</span></span>
<span data-ttu-id="e04e9-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e04e9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```



