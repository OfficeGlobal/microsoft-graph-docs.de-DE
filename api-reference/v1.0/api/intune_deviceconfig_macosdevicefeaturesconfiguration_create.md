# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="5a76e-101">Erstellen von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5a76e-101">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="5a76e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a76e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a76e-103">Diese Methode erstellt ein neues Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-103">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a76e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a76e-104">Prerequisites</span></span>
<span data-ttu-id="5a76e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a76e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a76e-107">Permission type</span></span>|<span data-ttu-id="5a76e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a76e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a76e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a76e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a76e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a76e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a76e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a76e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a76e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a76e-112">Not supported.</span></span>|
|<span data-ttu-id="5a76e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a76e-113">Application</span></span>|<span data-ttu-id="5a76e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a76e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a76e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a76e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a76e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a76e-116">Request headers</span></span>
|<span data-ttu-id="5a76e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a76e-117">Header</span></span>|<span data-ttu-id="5a76e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5a76e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a76e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a76e-119">Authorization</span></span>|<span data-ttu-id="5a76e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a76e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a76e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5a76e-121">Accept</span></span>|<span data-ttu-id="5a76e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a76e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a76e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a76e-123">Request body</span></span>
<span data-ttu-id="5a76e-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="5a76e-124">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="5a76e-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5a76e-125">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="5a76e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a76e-126">Property</span></span>|<span data-ttu-id="5a76e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5a76e-127">Type</span></span>|<span data-ttu-id="5a76e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a76e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a76e-129">id</span><span class="sxs-lookup"><span data-stu-id="5a76e-129">id</span></span>|<span data-ttu-id="5a76e-130">String</span><span class="sxs-lookup"><span data-stu-id="5a76e-130">String</span></span>|<span data-ttu-id="5a76e-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5a76e-131">Key of the entity.</span></span> <span data-ttu-id="5a76e-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a76e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a76e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5a76e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a76e-134">DateTimeOffset</span></span>|<span data-ttu-id="5a76e-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a76e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="5a76e-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a76e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a76e-137">createdDateTime</span></span>|<span data-ttu-id="5a76e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a76e-138">DateTimeOffset</span></span>|<span data-ttu-id="5a76e-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a76e-139">DateTime the object was created.</span></span> <span data-ttu-id="5a76e-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a76e-141">description</span><span class="sxs-lookup"><span data-stu-id="5a76e-141">description</span></span>|<span data-ttu-id="5a76e-142">String</span><span class="sxs-lookup"><span data-stu-id="5a76e-142">String</span></span>|<span data-ttu-id="5a76e-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5a76e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5a76e-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a76e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5a76e-145">displayName</span></span>|<span data-ttu-id="5a76e-146">String</span><span class="sxs-lookup"><span data-stu-id="5a76e-146">String</span></span>|<span data-ttu-id="5a76e-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5a76e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5a76e-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a76e-149">version</span><span class="sxs-lookup"><span data-stu-id="5a76e-149">version</span></span>|<span data-ttu-id="5a76e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5a76e-150">Int32</span></span>|<span data-ttu-id="5a76e-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5a76e-151">Version of the device configuration.</span></span> <span data-ttu-id="5a76e-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a76e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5a76e-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a76e-153">Response</span></span>
<span data-ttu-id="5a76e-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5a76e-154">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a76e-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a76e-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a76e-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a76e-156">Request</span></span>
<span data-ttu-id="5a76e-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a76e-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="5a76e-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a76e-158">Response</span></span>
<span data-ttu-id="5a76e-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a76e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



