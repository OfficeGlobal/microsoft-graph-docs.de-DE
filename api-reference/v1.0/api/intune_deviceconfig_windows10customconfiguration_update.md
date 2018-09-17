# <a name="update-windows10customconfiguration"></a><span data-ttu-id="da005-101">Aktualisieren von „windows10CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="da005-101">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="da005-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da005-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da005-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-103">Update the properties of a [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da005-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da005-104">Prerequisites</span></span>
<span data-ttu-id="da005-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da005-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da005-107">Permission type</span></span>|<span data-ttu-id="da005-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da005-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da005-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da005-109">Delegated (work or school account)</span></span>|<span data-ttu-id="da005-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da005-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da005-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da005-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da005-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da005-112">Not supported.</span></span>|
|<span data-ttu-id="da005-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da005-113">Application</span></span>|<span data-ttu-id="da005-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da005-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da005-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da005-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="da005-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da005-116">Request headers</span></span>
|<span data-ttu-id="da005-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="da005-117">Header</span></span>|<span data-ttu-id="da005-118">Wert</span><span class="sxs-lookup"><span data-stu-id="da005-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da005-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="da005-119">Authorization</span></span>|<span data-ttu-id="da005-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da005-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da005-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="da005-121">Accept</span></span>|<span data-ttu-id="da005-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="da005-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da005-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da005-123">Request body</span></span>
<span data-ttu-id="da005-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="da005-124">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="da005-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="da005-125">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span></span>

|<span data-ttu-id="da005-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da005-126">Property</span></span>|<span data-ttu-id="da005-127">Typ</span><span class="sxs-lookup"><span data-stu-id="da005-127">Type</span></span>|<span data-ttu-id="da005-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da005-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da005-129">ID</span><span class="sxs-lookup"><span data-stu-id="da005-129">id</span></span>|<span data-ttu-id="da005-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da005-130">String</span></span>|<span data-ttu-id="da005-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="da005-131">Key of the entity.</span></span> <span data-ttu-id="da005-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da005-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da005-133">lastModifiedDateTime</span></span>|<span data-ttu-id="da005-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da005-134">DateTimeOffset</span></span>|<span data-ttu-id="da005-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="da005-135">DateTime the object was last modified.</span></span> <span data-ttu-id="da005-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da005-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da005-137">createdDateTime</span></span>|<span data-ttu-id="da005-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da005-138">DateTimeOffset</span></span>|<span data-ttu-id="da005-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="da005-139">DateTime the object was created.</span></span> <span data-ttu-id="da005-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da005-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da005-141">description</span></span>|<span data-ttu-id="da005-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da005-142">String</span></span>|<span data-ttu-id="da005-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="da005-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da005-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da005-145">displayName</span><span class="sxs-lookup"><span data-stu-id="da005-145">displayName</span></span>|<span data-ttu-id="da005-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da005-146">String</span></span>|<span data-ttu-id="da005-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="da005-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da005-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da005-149">Version</span><span class="sxs-lookup"><span data-stu-id="da005-149">version</span></span>|<span data-ttu-id="da005-150">Int32</span><span class="sxs-lookup"><span data-stu-id="da005-150">Int32</span></span>|<span data-ttu-id="da005-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="da005-151">Version of the device configuration.</span></span> <span data-ttu-id="da005-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da005-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da005-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="da005-153">omaSettings</span></span>|<span data-ttu-id="da005-154">Collection von Objekten des Typs [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="da005-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="da005-155">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="da005-155">OMA settings.</span></span> <span data-ttu-id="da005-156">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="da005-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="da005-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="da005-157">Response</span></span>
<span data-ttu-id="da005-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da005-158">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da005-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da005-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="da005-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da005-160">Request</span></span>
<span data-ttu-id="da005-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da005-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 401

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="da005-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="da005-162">Response</span></span>
<span data-ttu-id="da005-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da005-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```








