# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="56f1d-101">deviceCompliancePolicySettingStateSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="56f1d-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="56f1d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56f1d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56f1d-103">Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56f1d-103">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56f1d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56f1d-104">Prerequisites</span></span>
<span data-ttu-id="56f1d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56f1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56f1d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56f1d-107">Permission type</span></span>|<span data-ttu-id="56f1d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56f1d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56f1d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56f1d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="56f1d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56f1d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56f1d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56f1d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56f1d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56f1d-112">Not supported.</span></span>|
|<span data-ttu-id="56f1d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56f1d-113">Application</span></span>|<span data-ttu-id="56f1d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56f1d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56f1d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56f1d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="56f1d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56f1d-116">Request headers</span></span>
|<span data-ttu-id="56f1d-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="56f1d-117">Header</span></span>|<span data-ttu-id="56f1d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="56f1d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56f1d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="56f1d-119">Authorization</span></span>|<span data-ttu-id="56f1d-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56f1d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56f1d-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="56f1d-121">Accept</span></span>|<span data-ttu-id="56f1d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="56f1d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56f1d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56f1d-123">Request body</span></span>
<span data-ttu-id="56f1d-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicySettingStateSummary an.</span><span class="sxs-lookup"><span data-stu-id="56f1d-124">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="56f1d-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicySettingStateSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="56f1d-125">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="56f1d-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56f1d-126">Property</span></span>|<span data-ttu-id="56f1d-127">Typ</span><span class="sxs-lookup"><span data-stu-id="56f1d-127">Type</span></span>|<span data-ttu-id="56f1d-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56f1d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56f1d-129">id</span><span class="sxs-lookup"><span data-stu-id="56f1d-129">id</span></span>|<span data-ttu-id="56f1d-130">String</span><span class="sxs-lookup"><span data-stu-id="56f1d-130">String</span></span>|<span data-ttu-id="56f1d-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="56f1d-131">Key of the entity.</span></span>|
|<span data-ttu-id="56f1d-132">setting</span><span class="sxs-lookup"><span data-stu-id="56f1d-132">setting</span></span>|<span data-ttu-id="56f1d-133">String</span><span class="sxs-lookup"><span data-stu-id="56f1d-133">String</span></span>|<span data-ttu-id="56f1d-134">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="56f1d-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="56f1d-135">settingName</span><span class="sxs-lookup"><span data-stu-id="56f1d-135">settingName</span></span>|<span data-ttu-id="56f1d-136">String</span><span class="sxs-lookup"><span data-stu-id="56f1d-136">String</span></span>|<span data-ttu-id="56f1d-137">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="56f1d-137">Name of the setting.</span></span>|
|<span data-ttu-id="56f1d-138">platformType</span><span class="sxs-lookup"><span data-stu-id="56f1d-138">platformType</span></span>|[<span data-ttu-id="56f1d-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="56f1d-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="56f1d-140">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="56f1d-140">Setting platform.</span></span> <span data-ttu-id="56f1d-141">Mögliche Werte sind: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile` und `all`.</span><span class="sxs-lookup"><span data-stu-id="56f1d-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="56f1d-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-142">unknownDeviceCount</span></span>|<span data-ttu-id="56f1d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-143">Int32</span></span>|<span data-ttu-id="56f1d-144">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="56f1d-144">Number of unknown devices</span></span>|
|<span data-ttu-id="56f1d-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="56f1d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-146">Int32</span></span>|<span data-ttu-id="56f1d-147">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="56f1d-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="56f1d-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-148">compliantDeviceCount</span></span>|<span data-ttu-id="56f1d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-149">Int32</span></span>|<span data-ttu-id="56f1d-150">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="56f1d-150">Number of compliant devices</span></span>|
|<span data-ttu-id="56f1d-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-151">remediatedDeviceCount</span></span>|<span data-ttu-id="56f1d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-152">Int32</span></span>|<span data-ttu-id="56f1d-153">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="56f1d-153">Number of remediated devices</span></span>|
|<span data-ttu-id="56f1d-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="56f1d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-155">Int32</span></span>|<span data-ttu-id="56f1d-156">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="56f1d-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="56f1d-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-157">errorDeviceCount</span></span>|<span data-ttu-id="56f1d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-158">Int32</span></span>|<span data-ttu-id="56f1d-159">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="56f1d-159">Number of error devices</span></span>|
|<span data-ttu-id="56f1d-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56f1d-160">conflictDeviceCount</span></span>|<span data-ttu-id="56f1d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="56f1d-161">Int32</span></span>|<span data-ttu-id="56f1d-162">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="56f1d-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="56f1d-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="56f1d-163">Response</span></span>
<span data-ttu-id="56f1d-164">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56f1d-164">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56f1d-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56f1d-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="56f1d-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56f1d-166">Request</span></span>
<span data-ttu-id="56f1d-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56f1d-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
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

### <a name="response"></a><span data-ttu-id="56f1d-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="56f1d-168">Response</span></span>
<span data-ttu-id="56f1d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56f1d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



