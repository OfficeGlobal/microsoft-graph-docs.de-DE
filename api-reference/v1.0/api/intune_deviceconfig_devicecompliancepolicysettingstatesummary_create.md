# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f44b3-101">deviceCompliancePolicySettingStateSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="f44b3-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="f44b3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f44b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f44b3-103">Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f44b3-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f44b3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f44b3-104">Prerequisites</span></span>
<span data-ttu-id="f44b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f44b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f44b3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f44b3-107">Permission type</span></span>|<span data-ttu-id="f44b3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f44b3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f44b3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f44b3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f44b3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f44b3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f44b3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f44b3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f44b3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f44b3-112">Not supported.</span></span>|
|<span data-ttu-id="f44b3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f44b3-113">Application</span></span>|<span data-ttu-id="f44b3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f44b3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f44b3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f44b3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f44b3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f44b3-116">Request headers</span></span>
|<span data-ttu-id="f44b3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f44b3-117">Header</span></span>|<span data-ttu-id="f44b3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f44b3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f44b3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f44b3-119">Authorization</span></span>|<span data-ttu-id="f44b3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f44b3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f44b3-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f44b3-121">Accept</span></span>|<span data-ttu-id="f44b3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f44b3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f44b3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f44b3-123">Request body</span></span>
<span data-ttu-id="f44b3-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicySettingStateSummary an.</span><span class="sxs-lookup"><span data-stu-id="f44b3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f44b3-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicySettingStateSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="f44b3-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="f44b3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f44b3-126">Property</span></span>|<span data-ttu-id="f44b3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f44b3-127">Type</span></span>|<span data-ttu-id="f44b3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f44b3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f44b3-129">Einstellung</span><span class="sxs-lookup"><span data-stu-id="f44b3-129">setting</span></span>|<span data-ttu-id="f44b3-130">String</span><span class="sxs-lookup"><span data-stu-id="f44b3-130">String</span></span>|<span data-ttu-id="f44b3-131">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f44b3-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="f44b3-132">settingName</span><span class="sxs-lookup"><span data-stu-id="f44b3-132">settingName</span></span>|<span data-ttu-id="f44b3-133">String</span><span class="sxs-lookup"><span data-stu-id="f44b3-133">String</span></span>|<span data-ttu-id="f44b3-134">Der Name der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="f44b3-134">Name of the setting.</span></span>|
|<span data-ttu-id="f44b3-135">platformType</span><span class="sxs-lookup"><span data-stu-id="f44b3-135">PlatformType</span></span>|<span data-ttu-id="f44b3-136">String</span><span class="sxs-lookup"><span data-stu-id="f44b3-136">String</span></span>|<span data-ttu-id="f44b3-137">Die Plattform der Einstellung. Mögliche Werte: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="f44b3-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="f44b3-138">id</span><span class="sxs-lookup"><span data-stu-id="f44b3-138">id</span></span>|<span data-ttu-id="f44b3-139">String</span><span class="sxs-lookup"><span data-stu-id="f44b3-139">String</span></span>|<span data-ttu-id="f44b3-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f44b3-140">Key of the setting.</span></span>|
|<span data-ttu-id="f44b3-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-141">unknownDeviceCount</span></span>|<span data-ttu-id="f44b3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-142">Int32</span></span>|<span data-ttu-id="f44b3-143">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="f44b3-143">Number of unknown devices</span></span>|
|<span data-ttu-id="f44b3-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="f44b3-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-145">Int32</span></span>|<span data-ttu-id="f44b3-146">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="f44b3-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="f44b3-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-147">compliantDeviceCount</span></span>|<span data-ttu-id="f44b3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-148">Int32</span></span>|<span data-ttu-id="f44b3-149">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="f44b3-149">Number of compliant devices</span></span>|
|<span data-ttu-id="f44b3-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-150">remediatedDeviceCount</span></span>|<span data-ttu-id="f44b3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-151">Int32</span></span>|<span data-ttu-id="f44b3-152">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="f44b3-152">Number of remediated devices</span></span>|
|<span data-ttu-id="f44b3-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f44b3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-154">Int32</span></span>|<span data-ttu-id="f44b3-155">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="f44b3-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f44b3-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-156">errorDeviceCount</span></span>|<span data-ttu-id="f44b3-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-157">Int32</span></span>|<span data-ttu-id="f44b3-158">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="f44b3-158">Number of error devices</span></span>|
|<span data-ttu-id="f44b3-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44b3-159">conflictDeviceCount</span></span>|<span data-ttu-id="f44b3-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f44b3-160">Int32</span></span>|<span data-ttu-id="f44b3-161">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="f44b3-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f44b3-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="f44b3-162">Response</span></span>
<span data-ttu-id="f44b3-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f44b3-163">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f44b3-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f44b3-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="f44b3-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f44b3-165">Request</span></span>
<span data-ttu-id="f44b3-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f44b3-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f44b3-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="f44b3-167">Response</span></span>
<span data-ttu-id="f44b3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f44b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



