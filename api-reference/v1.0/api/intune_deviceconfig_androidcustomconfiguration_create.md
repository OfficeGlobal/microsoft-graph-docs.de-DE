# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="ae9b7-101">Erstellen von „androidCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ae9b7-101">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="ae9b7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae9b7-103">Diese Methode erstellt ein neues Objekt des Typs [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae9b7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae9b7-104">Prerequisites</span></span>
<span data-ttu-id="ae9b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae9b7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae9b7-107">Permission type</span></span>|<span data-ttu-id="ae9b7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae9b7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae9b7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae9b7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ae9b7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae9b7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae9b7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae9b7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae9b7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae9b7-112">Not supported.</span></span>|
|<span data-ttu-id="ae9b7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae9b7-113">Application</span></span>|<span data-ttu-id="ae9b7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae9b7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae9b7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae9b7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ae9b7-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae9b7-116">Request headers</span></span>
|<span data-ttu-id="ae9b7-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ae9b7-117">Header</span></span>|<span data-ttu-id="ae9b7-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ae9b7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae9b7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae9b7-119">Authorization</span></span>|<span data-ttu-id="ae9b7-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae9b7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae9b7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ae9b7-121">Accept</span></span>|<span data-ttu-id="ae9b7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ae9b7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae9b7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae9b7-123">Request body</span></span>
<span data-ttu-id="ae9b7-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ae9b7-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ae9b7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae9b7-126">Property</span></span>|<span data-ttu-id="ae9b7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ae9b7-127">Type</span></span>|<span data-ttu-id="ae9b7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae9b7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae9b7-129">id</span><span class="sxs-lookup"><span data-stu-id="ae9b7-129">id</span></span>|<span data-ttu-id="ae9b7-130">String</span><span class="sxs-lookup"><span data-stu-id="ae9b7-130">String</span></span>|<span data-ttu-id="ae9b7-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-131">Key of the setting.</span></span> <span data-ttu-id="ae9b7-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae9b7-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae9b7-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ae9b7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae9b7-134">DateTimeOffset</span></span>|<span data-ttu-id="ae9b7-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="ae9b7-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae9b7-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae9b7-137">createdDateTime</span></span>|<span data-ttu-id="ae9b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae9b7-138">DateTimeOffset</span></span>|<span data-ttu-id="ae9b7-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-139">DateTime the object was created.</span></span> <span data-ttu-id="ae9b7-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae9b7-141">description</span><span class="sxs-lookup"><span data-stu-id="ae9b7-141">description</span></span>|<span data-ttu-id="ae9b7-142">String</span><span class="sxs-lookup"><span data-stu-id="ae9b7-142">String</span></span>|<span data-ttu-id="ae9b7-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae9b7-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae9b7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ae9b7-145">displayName</span></span>|<span data-ttu-id="ae9b7-146">String</span><span class="sxs-lookup"><span data-stu-id="ae9b7-146">String</span></span>|<span data-ttu-id="ae9b7-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae9b7-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae9b7-149">version</span><span class="sxs-lookup"><span data-stu-id="ae9b7-149">version</span></span>|<span data-ttu-id="ae9b7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ae9b7-150">Int32</span></span>|<span data-ttu-id="ae9b7-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-151">Version of the device configuration.</span></span> <span data-ttu-id="ae9b7-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae9b7-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae9b7-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ae9b7-153">omaSettings</span></span>|<span data-ttu-id="ae9b7-154">Collection von Objekten des Typs [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae9b7-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="ae9b7-155">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-155">OMA settings.</span></span> <span data-ttu-id="ae9b7-156">Diese Collection darf maximal 1.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ae9b7-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae9b7-157">Response</span></span>
<span data-ttu-id="ae9b7-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae9b7-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae9b7-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae9b7-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae9b7-160">Request</span></span>
<span data-ttu-id="ae9b7-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="ae9b7-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae9b7-162">Response</span></span>
<span data-ttu-id="ae9b7-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae9b7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



