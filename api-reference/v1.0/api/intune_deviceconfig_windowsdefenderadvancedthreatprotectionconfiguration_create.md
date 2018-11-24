# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="71fee-101">Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="71fee-101">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="71fee-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71fee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71fee-103">Diese Methode erstellt ein neues Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-103">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71fee-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71fee-104">Prerequisites</span></span>
<span data-ttu-id="71fee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71fee-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71fee-107">Permission type</span></span>|<span data-ttu-id="71fee-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71fee-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71fee-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71fee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71fee-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fee-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71fee-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71fee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71fee-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71fee-112">Not supported.</span></span>|
|<span data-ttu-id="71fee-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71fee-113">Application</span></span>|<span data-ttu-id="71fee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71fee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71fee-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71fee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71fee-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71fee-116">Request headers</span></span>
|<span data-ttu-id="71fee-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71fee-117">Header</span></span>|<span data-ttu-id="71fee-118">Wert</span><span class="sxs-lookup"><span data-stu-id="71fee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71fee-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="71fee-119">Authorization</span></span>|<span data-ttu-id="71fee-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71fee-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71fee-121">Accept</span><span class="sxs-lookup"><span data-stu-id="71fee-121">Accept</span></span>|<span data-ttu-id="71fee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="71fee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fee-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71fee-123">Request body</span></span>
<span data-ttu-id="71fee-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="71fee-124">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="71fee-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="71fee-125">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="71fee-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71fee-126">Property</span></span>|<span data-ttu-id="71fee-127">Typ</span><span class="sxs-lookup"><span data-stu-id="71fee-127">Type</span></span>|<span data-ttu-id="71fee-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71fee-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71fee-129">id</span><span class="sxs-lookup"><span data-stu-id="71fee-129">id</span></span>|<span data-ttu-id="71fee-130">String</span><span class="sxs-lookup"><span data-stu-id="71fee-130">String</span></span>|<span data-ttu-id="71fee-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="71fee-131">Key of the entity.</span></span> <span data-ttu-id="71fee-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71fee-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71fee-133">lastModifiedDateTime</span></span>|<span data-ttu-id="71fee-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fee-134">DateTimeOffset</span></span>|<span data-ttu-id="71fee-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="71fee-135">DateTime the object was last modified.</span></span> <span data-ttu-id="71fee-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71fee-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71fee-137">createdDateTime</span></span>|<span data-ttu-id="71fee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fee-138">DateTimeOffset</span></span>|<span data-ttu-id="71fee-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="71fee-139">DateTime the object was created.</span></span> <span data-ttu-id="71fee-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71fee-141">description</span><span class="sxs-lookup"><span data-stu-id="71fee-141">description</span></span>|<span data-ttu-id="71fee-142">String</span><span class="sxs-lookup"><span data-stu-id="71fee-142">String</span></span>|<span data-ttu-id="71fee-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="71fee-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71fee-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71fee-145">displayName</span><span class="sxs-lookup"><span data-stu-id="71fee-145">displayName</span></span>|<span data-ttu-id="71fee-146">String</span><span class="sxs-lookup"><span data-stu-id="71fee-146">String</span></span>|<span data-ttu-id="71fee-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="71fee-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71fee-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71fee-149">version</span><span class="sxs-lookup"><span data-stu-id="71fee-149">version</span></span>|<span data-ttu-id="71fee-150">Int32</span><span class="sxs-lookup"><span data-stu-id="71fee-150">Int32</span></span>|<span data-ttu-id="71fee-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="71fee-151">Version of the device configuration.</span></span> <span data-ttu-id="71fee-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71fee-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="71fee-153">allowSampleSharing</span></span>|<span data-ttu-id="71fee-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="71fee-154">Boolean</span></span>|<span data-ttu-id="71fee-155">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="71fee-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="71fee-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="71fee-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="71fee-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="71fee-157">Boolean</span></span>|<span data-ttu-id="71fee-158">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="71fee-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="71fee-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="71fee-159">Response</span></span>
<span data-ttu-id="71fee-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="71fee-160">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71fee-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71fee-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="71fee-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71fee-162">Request</span></span>
<span data-ttu-id="71fee-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71fee-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="71fee-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="71fee-164">Response</span></span>
<span data-ttu-id="71fee-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71fee-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



