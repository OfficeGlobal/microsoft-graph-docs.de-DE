# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="dc550-101">Aktualisieren von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="dc550-101">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="dc550-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dc550-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc550-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="dc550-103">Update the properties of a [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc550-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dc550-104">Prerequisites</span></span>
<span data-ttu-id="dc550-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dc550-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc550-107">Permission type</span></span>|<span data-ttu-id="dc550-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc550-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc550-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc550-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dc550-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc550-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc550-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc550-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc550-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc550-112">Not supported.</span></span>|
|<span data-ttu-id="dc550-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc550-113">Application</span></span>|<span data-ttu-id="dc550-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc550-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc550-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc550-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="dc550-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc550-116">Request headers</span></span>
|<span data-ttu-id="dc550-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dc550-117">Header</span></span>|<span data-ttu-id="dc550-118">Wert</span><span class="sxs-lookup"><span data-stu-id="dc550-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc550-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dc550-119">Authorization</span></span>|<span data-ttu-id="dc550-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dc550-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc550-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="dc550-121">Accept</span></span>|<span data-ttu-id="dc550-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="dc550-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc550-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc550-123">Request body</span></span>
<span data-ttu-id="dc550-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="dc550-124">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="dc550-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="dc550-125">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="dc550-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc550-126">Property</span></span>|<span data-ttu-id="dc550-127">Typ</span><span class="sxs-lookup"><span data-stu-id="dc550-127">Type</span></span>|<span data-ttu-id="dc550-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc550-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc550-129">ID</span><span class="sxs-lookup"><span data-stu-id="dc550-129">id</span></span>|<span data-ttu-id="dc550-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc550-130">String</span></span>|<span data-ttu-id="dc550-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dc550-131">Key of the entity.</span></span>|
|<span data-ttu-id="dc550-132">settingName</span><span class="sxs-lookup"><span data-stu-id="dc550-132">settingName</span></span>|<span data-ttu-id="dc550-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc550-133">String</span></span>|<span data-ttu-id="dc550-134">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-134">Name of the setting</span></span>|
|<span data-ttu-id="dc550-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="dc550-135">instancePath</span></span>|<span data-ttu-id="dc550-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc550-136">String</span></span>|<span data-ttu-id="dc550-137">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="dc550-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="dc550-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-138">unknownDeviceCount</span></span>|<span data-ttu-id="dc550-139">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-139">Int32</span></span>|<span data-ttu-id="dc550-140">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="dc550-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="dc550-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-142">Int32</span></span>|<span data-ttu-id="dc550-143">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="dc550-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-144">compliantDeviceCount</span></span>|<span data-ttu-id="dc550-145">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-145">Int32</span></span>|<span data-ttu-id="dc550-146">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="dc550-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-147">remediatedDeviceCount</span></span>|<span data-ttu-id="dc550-148">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-148">Int32</span></span>|<span data-ttu-id="dc550-149">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="dc550-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="dc550-151">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-151">Int32</span></span>|<span data-ttu-id="dc550-152">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="dc550-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-153">errorDeviceCount</span></span>|<span data-ttu-id="dc550-154">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-154">Int32</span></span>|<span data-ttu-id="dc550-155">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-155">Device error count for the setting</span></span>|
|<span data-ttu-id="dc550-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc550-156">conflictDeviceCount</span></span>|<span data-ttu-id="dc550-157">Int32</span><span class="sxs-lookup"><span data-stu-id="dc550-157">Int32</span></span>|<span data-ttu-id="dc550-158">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="dc550-158">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="dc550-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc550-159">Response</span></span>
<span data-ttu-id="dc550-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dc550-160">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc550-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc550-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc550-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc550-162">Request</span></span>
<span data-ttu-id="dc550-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc550-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 296

{
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="dc550-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc550-164">Response</span></span>
<span data-ttu-id="dc550-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc550-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```








