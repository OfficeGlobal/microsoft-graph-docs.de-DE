# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="5faca-101">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="5faca-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="5faca-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5faca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5faca-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5faca-103">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5faca-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5faca-104">Prerequisites</span></span>
<span data-ttu-id="5faca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5faca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5faca-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5faca-107">Permission type</span></span>|<span data-ttu-id="5faca-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5faca-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5faca-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5faca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5faca-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5faca-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5faca-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5faca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5faca-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5faca-112">Not supported.</span></span>|
|<span data-ttu-id="5faca-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5faca-113">Application</span></span>|<span data-ttu-id="5faca-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5faca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5faca-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5faca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="5faca-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5faca-116">Request headers</span></span>
|<span data-ttu-id="5faca-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5faca-117">Header</span></span>|<span data-ttu-id="5faca-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5faca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5faca-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5faca-119">Authorization</span></span>|<span data-ttu-id="5faca-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5faca-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5faca-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5faca-121">Accept</span></span>|<span data-ttu-id="5faca-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="5faca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5faca-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5faca-123">Request body</span></span>
<span data-ttu-id="5faca-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="5faca-124">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="5faca-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5faca-125">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="5faca-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5faca-126">Property</span></span>|<span data-ttu-id="5faca-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5faca-127">Type</span></span>|<span data-ttu-id="5faca-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5faca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5faca-129">ID</span><span class="sxs-lookup"><span data-stu-id="5faca-129">id</span></span>|<span data-ttu-id="5faca-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5faca-130">String</span></span>|<span data-ttu-id="5faca-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5faca-131">Key of the entity.</span></span>|
|<span data-ttu-id="5faca-132">Einstellung</span><span class="sxs-lookup"><span data-stu-id="5faca-132">setting</span></span>|<span data-ttu-id="5faca-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5faca-133">String</span></span>|<span data-ttu-id="5faca-134">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="5faca-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="5faca-135">settingName</span><span class="sxs-lookup"><span data-stu-id="5faca-135">settingName</span></span>|<span data-ttu-id="5faca-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5faca-136">String</span></span>|<span data-ttu-id="5faca-137">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="5faca-137">Name of the setting.</span></span>|
|<span data-ttu-id="5faca-138">platformType</span><span class="sxs-lookup"><span data-stu-id="5faca-138">platformType</span></span>|[<span data-ttu-id="5faca-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="5faca-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="5faca-140">Einstellungsplattform.</span><span class="sxs-lookup"><span data-stu-id="5faca-140">Setting platform.</span></span> <span data-ttu-id="5faca-141">Mögliche Werte sind: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile` und `all`.</span><span class="sxs-lookup"><span data-stu-id="5faca-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="5faca-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-142">unknownDeviceCount</span></span>|<span data-ttu-id="5faca-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-143">Int32</span></span>|<span data-ttu-id="5faca-144">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="5faca-144">Number of unknown devices</span></span>|
|<span data-ttu-id="5faca-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="5faca-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-146">Int32</span></span>|<span data-ttu-id="5faca-147">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="5faca-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="5faca-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-148">compliantDeviceCount</span></span>|<span data-ttu-id="5faca-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-149">Int32</span></span>|<span data-ttu-id="5faca-150">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="5faca-150">Number of compliant devices</span></span>|
|<span data-ttu-id="5faca-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-151">remediatedDeviceCount</span></span>|<span data-ttu-id="5faca-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-152">Int32</span></span>|<span data-ttu-id="5faca-153">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="5faca-153">Number of remediated devices</span></span>|
|<span data-ttu-id="5faca-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5faca-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-155">Int32</span></span>|<span data-ttu-id="5faca-156">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="5faca-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5faca-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-157">errorDeviceCount</span></span>|<span data-ttu-id="5faca-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-158">Int32</span></span>|<span data-ttu-id="5faca-159">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="5faca-159">Number of error devices</span></span>|
|<span data-ttu-id="5faca-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5faca-160">conflictDeviceCount</span></span>|<span data-ttu-id="5faca-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5faca-161">Int32</span></span>|<span data-ttu-id="5faca-162">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="5faca-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="5faca-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="5faca-163">Response</span></span>
<span data-ttu-id="5faca-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5faca-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5faca-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5faca-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="5faca-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5faca-166">Request</span></span>
<span data-ttu-id="5faca-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5faca-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 311

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="5faca-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="5faca-168">Response</span></span>
<span data-ttu-id="5faca-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5faca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```








