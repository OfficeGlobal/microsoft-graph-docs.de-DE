# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="1f812-101">Erstellen von „windowsPhone81CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="1f812-101">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="1f812-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1f812-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f812-103">Diese Methode erstellt ein neues Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f812-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f812-104">Prerequisites</span></span>
<span data-ttu-id="1f812-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f812-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f812-107">Permission type</span></span>|<span data-ttu-id="1f812-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f812-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f812-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f812-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1f812-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f812-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f812-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f812-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f812-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f812-112">Not supported.</span></span>|
|<span data-ttu-id="1f812-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f812-113">Application</span></span>|<span data-ttu-id="1f812-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f812-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f812-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f812-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f812-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f812-116">Request headers</span></span>
|<span data-ttu-id="1f812-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f812-117">Header</span></span>|<span data-ttu-id="1f812-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1f812-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f812-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f812-119">Authorization</span></span>|<span data-ttu-id="1f812-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f812-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f812-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1f812-121">Accept</span></span>|<span data-ttu-id="1f812-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1f812-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f812-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f812-123">Request body</span></span>
<span data-ttu-id="1f812-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsPhone81CustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="1f812-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1f812-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsPhone81CustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="1f812-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="1f812-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f812-126">Property</span></span>|<span data-ttu-id="1f812-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1f812-127">Type</span></span>|<span data-ttu-id="1f812-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f812-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f812-129">id</span><span class="sxs-lookup"><span data-stu-id="1f812-129">id</span></span>|<span data-ttu-id="1f812-130">String</span><span class="sxs-lookup"><span data-stu-id="1f812-130">String</span></span>|<span data-ttu-id="1f812-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="1f812-131">Key of the setting.</span></span> <span data-ttu-id="1f812-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f812-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f812-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1f812-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f812-134">DateTimeOffset</span></span>|<span data-ttu-id="1f812-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f812-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="1f812-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f812-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f812-137">createdDateTime</span></span>|<span data-ttu-id="1f812-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f812-138">DateTimeOffset</span></span>|<span data-ttu-id="1f812-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f812-139">DateTime the object was created.</span></span> <span data-ttu-id="1f812-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f812-141">description</span><span class="sxs-lookup"><span data-stu-id="1f812-141">description</span></span>|<span data-ttu-id="1f812-142">String</span><span class="sxs-lookup"><span data-stu-id="1f812-142">String</span></span>|<span data-ttu-id="1f812-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1f812-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f812-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f812-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1f812-145">displayName</span></span>|<span data-ttu-id="1f812-146">String</span><span class="sxs-lookup"><span data-stu-id="1f812-146">String</span></span>|<span data-ttu-id="1f812-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1f812-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f812-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f812-149">version</span><span class="sxs-lookup"><span data-stu-id="1f812-149">version</span></span>|<span data-ttu-id="1f812-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1f812-150">Int32</span></span>|<span data-ttu-id="1f812-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1f812-151">Version of the device configuration.</span></span> <span data-ttu-id="1f812-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f812-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f812-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="1f812-153">omaSettings</span></span>|<span data-ttu-id="1f812-154">Collection von Objekten des Typs [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1f812-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="1f812-155">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="1f812-155">OMA settings.</span></span> <span data-ttu-id="1f812-156">Diese Collection darf maximal 1.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="1f812-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1f812-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f812-157">Response</span></span>
<span data-ttu-id="1f812-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1f812-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f812-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f812-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f812-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f812-160">Request</span></span>
<span data-ttu-id="1f812-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f812-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="1f812-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f812-162">Response</span></span>
<span data-ttu-id="1f812-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f812-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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



