# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="3e557-101">Aktualisieren von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3e557-101">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="3e557-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e557-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e557-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-103">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e557-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e557-104">Prerequisites</span></span>
<span data-ttu-id="3e557-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e557-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e557-107">Permission type</span></span>|<span data-ttu-id="3e557-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e557-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e557-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e557-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3e557-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e557-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e557-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e557-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e557-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e557-112">Not supported.</span></span>|
|<span data-ttu-id="3e557-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e557-113">Application</span></span>|<span data-ttu-id="3e557-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e557-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e557-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e557-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3e557-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e557-116">Request headers</span></span>
|<span data-ttu-id="3e557-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3e557-117">Header</span></span>|<span data-ttu-id="3e557-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3e557-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e557-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e557-119">Authorization</span></span>|<span data-ttu-id="3e557-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e557-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e557-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3e557-121">Accept</span></span>|<span data-ttu-id="3e557-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3e557-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e557-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e557-123">Request body</span></span>
<span data-ttu-id="3e557-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="3e557-124">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="3e557-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3e557-125">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="3e557-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e557-126">Property</span></span>|<span data-ttu-id="3e557-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3e557-127">Type</span></span>|<span data-ttu-id="3e557-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e557-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e557-129">id</span><span class="sxs-lookup"><span data-stu-id="3e557-129">id</span></span>|<span data-ttu-id="3e557-130">String</span><span class="sxs-lookup"><span data-stu-id="3e557-130">String</span></span>|<span data-ttu-id="3e557-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3e557-131">Key of the entity.</span></span> <span data-ttu-id="3e557-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e557-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e557-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3e557-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e557-134">DateTimeOffset</span></span>|<span data-ttu-id="3e557-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e557-135">DateTime the object was last modified.</span></span> <span data-ttu-id="3e557-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e557-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e557-137">createdDateTime</span></span>|<span data-ttu-id="3e557-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e557-138">DateTimeOffset</span></span>|<span data-ttu-id="3e557-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e557-139">DateTime the object was created.</span></span> <span data-ttu-id="3e557-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e557-141">description</span><span class="sxs-lookup"><span data-stu-id="3e557-141">description</span></span>|<span data-ttu-id="3e557-142">String</span><span class="sxs-lookup"><span data-stu-id="3e557-142">String</span></span>|<span data-ttu-id="3e557-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3e557-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e557-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e557-145">displayName</span><span class="sxs-lookup"><span data-stu-id="3e557-145">displayName</span></span>|<span data-ttu-id="3e557-146">String</span><span class="sxs-lookup"><span data-stu-id="3e557-146">String</span></span>|<span data-ttu-id="3e557-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3e557-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e557-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e557-149">version</span><span class="sxs-lookup"><span data-stu-id="3e557-149">version</span></span>|<span data-ttu-id="3e557-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3e557-150">Int32</span></span>|<span data-ttu-id="3e557-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e557-151">Version of the device configuration.</span></span> <span data-ttu-id="3e557-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e557-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e557-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="3e557-153">allowSampleSharing</span></span>|<span data-ttu-id="3e557-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e557-154">Boolean</span></span>|<span data-ttu-id="3e557-155">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="3e557-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="3e557-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="3e557-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="3e557-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e557-157">Boolean</span></span>|<span data-ttu-id="3e557-158">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="3e557-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="3e557-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e557-159">Response</span></span>
<span data-ttu-id="3e557-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3e557-160">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e557-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e557-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e557-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e557-162">Request</span></span>
<span data-ttu-id="3e557-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e557-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="3e557-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e557-164">Response</span></span>
<span data-ttu-id="3e557-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e557-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



