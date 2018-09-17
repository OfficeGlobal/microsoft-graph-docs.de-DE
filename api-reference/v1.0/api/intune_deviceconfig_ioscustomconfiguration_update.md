# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="5aaa9-101">Aktualisieren von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5aaa9-101">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="5aaa9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5aaa9-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-103">Update the properties of a [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5aaa9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5aaa9-104">Prerequisites</span></span>
<span data-ttu-id="5aaa9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5aaa9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5aaa9-107">Permission type</span></span>|<span data-ttu-id="5aaa9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5aaa9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5aaa9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5aaa9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5aaa9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aaa9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5aaa9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5aaa9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5aaa9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5aaa9-112">Not supported.</span></span>|
|<span data-ttu-id="5aaa9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5aaa9-113">Application</span></span>|<span data-ttu-id="5aaa9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5aaa9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5aaa9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5aaa9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5aaa9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5aaa9-116">Request headers</span></span>
|<span data-ttu-id="5aaa9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5aaa9-117">Header</span></span>|<span data-ttu-id="5aaa9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5aaa9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5aaa9-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5aaa9-119">Authorization</span></span>|<span data-ttu-id="5aaa9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5aaa9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5aaa9-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5aaa9-121">Accept</span></span>|<span data-ttu-id="5aaa9-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="5aaa9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aaa9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5aaa9-123">Request body</span></span>
<span data-ttu-id="5aaa9-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-124">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="5aaa9-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-125">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="5aaa9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5aaa9-126">Property</span></span>|<span data-ttu-id="5aaa9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5aaa9-127">Type</span></span>|<span data-ttu-id="5aaa9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5aaa9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aaa9-129">ID</span><span class="sxs-lookup"><span data-stu-id="5aaa9-129">id</span></span>|<span data-ttu-id="5aaa9-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aaa9-130">String</span></span>|<span data-ttu-id="5aaa9-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5aaa9-131">Key of the entity.</span></span> <span data-ttu-id="5aaa9-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aaa9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5aaa9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5aaa9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aaa9-134">DateTimeOffset</span></span>|<span data-ttu-id="5aaa9-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-135">DateTime the object was last modified.</span></span> <span data-ttu-id="5aaa9-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aaa9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5aaa9-137">createdDateTime</span></span>|<span data-ttu-id="5aaa9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aaa9-138">DateTimeOffset</span></span>|<span data-ttu-id="5aaa9-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-139">DateTime the object was created.</span></span> <span data-ttu-id="5aaa9-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aaa9-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5aaa9-141">description</span></span>|<span data-ttu-id="5aaa9-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aaa9-142">String</span></span>|<span data-ttu-id="5aaa9-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5aaa9-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aaa9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5aaa9-145">displayName</span></span>|<span data-ttu-id="5aaa9-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aaa9-146">String</span></span>|<span data-ttu-id="5aaa9-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5aaa9-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aaa9-149">Version</span><span class="sxs-lookup"><span data-stu-id="5aaa9-149">version</span></span>|<span data-ttu-id="5aaa9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5aaa9-150">Int32</span></span>|<span data-ttu-id="5aaa9-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-151">Version of the device configuration.</span></span> <span data-ttu-id="5aaa9-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa9-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aaa9-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="5aaa9-153">payloadName</span></span>|<span data-ttu-id="5aaa9-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aaa9-154">String</span></span>|<span data-ttu-id="5aaa9-155">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="5aaa9-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="5aaa9-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="5aaa9-156">payloadFileName</span></span>|<span data-ttu-id="5aaa9-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aaa9-157">String</span></span>|<span data-ttu-id="5aaa9-158">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="5aaa9-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="5aaa9-159">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="5aaa9-159">\*.xml).</span></span>|
|<span data-ttu-id="5aaa9-160">payload</span><span class="sxs-lookup"><span data-stu-id="5aaa9-160">payload</span></span>|<span data-ttu-id="5aaa9-161">Binär</span><span class="sxs-lookup"><span data-stu-id="5aaa9-161">Binary</span></span>|<span data-ttu-id="5aaa9-162">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="5aaa9-162">Payload.</span></span> <span data-ttu-id="5aaa9-163">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="5aaa9-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="5aaa9-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="5aaa9-164">Response</span></span>
<span data-ttu-id="5aaa9-165">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-165">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aaa9-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5aaa9-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="5aaa9-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5aaa9-167">Request</span></span>
<span data-ttu-id="5aaa9-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 282

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="5aaa9-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="5aaa9-169">Response</span></span>
<span data-ttu-id="5aaa9-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5aaa9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```








