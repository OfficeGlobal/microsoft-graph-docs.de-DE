# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="ad83d-101">Aktualisieren von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ad83d-101">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="ad83d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ad83d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad83d-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad83d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ad83d-104">Prerequisites</span></span>
<span data-ttu-id="ad83d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad83d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ad83d-107">Permission type</span></span>|<span data-ttu-id="ad83d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ad83d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad83d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ad83d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad83d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad83d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad83d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ad83d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad83d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad83d-112">Not supported.</span></span>|
|<span data-ttu-id="ad83d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ad83d-113">Application</span></span>|<span data-ttu-id="ad83d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad83d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad83d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad83d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ad83d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad83d-116">Request headers</span></span>
|<span data-ttu-id="ad83d-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ad83d-117">Header</span></span>|<span data-ttu-id="ad83d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ad83d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad83d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad83d-119">Authorization</span></span>|<span data-ttu-id="ad83d-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ad83d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad83d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad83d-121">Accept</span></span>|<span data-ttu-id="ad83d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad83d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad83d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad83d-123">Request body</span></span>
<span data-ttu-id="ad83d-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="ad83d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="ad83d-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ad83d-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ad83d-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad83d-126">Property</span></span>|<span data-ttu-id="ad83d-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ad83d-127">Type</span></span>|<span data-ttu-id="ad83d-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad83d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad83d-129">id</span><span class="sxs-lookup"><span data-stu-id="ad83d-129">id</span></span>|<span data-ttu-id="ad83d-130">String</span><span class="sxs-lookup"><span data-stu-id="ad83d-130">String</span></span>|<span data-ttu-id="ad83d-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="ad83d-131">Key of the setting.</span></span> <span data-ttu-id="ad83d-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad83d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad83d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ad83d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad83d-134">DateTimeOffset</span></span>|<span data-ttu-id="ad83d-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad83d-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="ad83d-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad83d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad83d-137">createdDateTime</span></span>|<span data-ttu-id="ad83d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad83d-138">DateTimeOffset</span></span>|<span data-ttu-id="ad83d-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad83d-139">DateTime the object was created.</span></span> <span data-ttu-id="ad83d-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad83d-141">description</span><span class="sxs-lookup"><span data-stu-id="ad83d-141">description</span></span>|<span data-ttu-id="ad83d-142">String</span><span class="sxs-lookup"><span data-stu-id="ad83d-142">String</span></span>|<span data-ttu-id="ad83d-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ad83d-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad83d-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad83d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ad83d-145">displayName</span></span>|<span data-ttu-id="ad83d-146">String</span><span class="sxs-lookup"><span data-stu-id="ad83d-146">String</span></span>|<span data-ttu-id="ad83d-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ad83d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad83d-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad83d-149">version</span><span class="sxs-lookup"><span data-stu-id="ad83d-149">version</span></span>|<span data-ttu-id="ad83d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ad83d-150">Int32</span></span>|<span data-ttu-id="ad83d-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad83d-151">Version of the device configuration.</span></span> <span data-ttu-id="ad83d-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad83d-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad83d-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="ad83d-153">allowSampleSharing</span></span>|<span data-ttu-id="ad83d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad83d-154">Boolean</span></span>|<span data-ttu-id="ad83d-155">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="ad83d-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="ad83d-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="ad83d-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="ad83d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad83d-157">Boolean</span></span>|<span data-ttu-id="ad83d-158">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="ad83d-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="ad83d-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad83d-159">Response</span></span>
<span data-ttu-id="ad83d-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ad83d-160">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad83d-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad83d-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad83d-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad83d-162">Request</span></span>
<span data-ttu-id="ad83d-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ad83d-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 240

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="ad83d-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad83d-164">Response</span></span>
<span data-ttu-id="ad83d-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad83d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



