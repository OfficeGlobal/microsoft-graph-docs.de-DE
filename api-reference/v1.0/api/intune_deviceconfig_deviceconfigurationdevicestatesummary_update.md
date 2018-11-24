# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="e188e-101">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="e188e-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="e188e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e188e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e188e-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e188e-103">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e188e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e188e-104">Prerequisites</span></span>
<span data-ttu-id="e188e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e188e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e188e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e188e-107">Permission type</span></span>|<span data-ttu-id="e188e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e188e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e188e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e188e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e188e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e188e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e188e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e188e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e188e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e188e-112">Not supported.</span></span>|
|<span data-ttu-id="e188e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e188e-113">Application</span></span>|<span data-ttu-id="e188e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e188e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e188e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e188e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e188e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e188e-116">Request headers</span></span>
|<span data-ttu-id="e188e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e188e-117">Header</span></span>|<span data-ttu-id="e188e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e188e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e188e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e188e-119">Authorization</span></span>|<span data-ttu-id="e188e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e188e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e188e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e188e-121">Accept</span></span>|<span data-ttu-id="e188e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e188e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e188e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e188e-123">Request body</span></span>
<span data-ttu-id="e188e-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="e188e-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="e188e-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e188e-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="e188e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e188e-126">Property</span></span>|<span data-ttu-id="e188e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e188e-127">Type</span></span>|<span data-ttu-id="e188e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e188e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e188e-129">id</span><span class="sxs-lookup"><span data-stu-id="e188e-129">id</span></span>|<span data-ttu-id="e188e-130">String</span><span class="sxs-lookup"><span data-stu-id="e188e-130">String</span></span>|<span data-ttu-id="e188e-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e188e-131">Key of the entity.</span></span>|
|<span data-ttu-id="e188e-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-132">unknownDeviceCount</span></span>|<span data-ttu-id="e188e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-133">Int32</span></span>|<span data-ttu-id="e188e-134">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="e188e-134">Number of unknown devices</span></span>|
|<span data-ttu-id="e188e-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="e188e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-136">Int32</span></span>|<span data-ttu-id="e188e-137">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="e188e-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="e188e-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-138">compliantDeviceCount</span></span>|<span data-ttu-id="e188e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-139">Int32</span></span>|<span data-ttu-id="e188e-140">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="e188e-140">Number of compliant devices</span></span>|
|<span data-ttu-id="e188e-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-141">remediatedDeviceCount</span></span>|<span data-ttu-id="e188e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-142">Int32</span></span>|<span data-ttu-id="e188e-143">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="e188e-143">Number of remediated devices</span></span>|
|<span data-ttu-id="e188e-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e188e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-145">Int32</span></span>|<span data-ttu-id="e188e-146">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="e188e-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e188e-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-147">errorDeviceCount</span></span>|<span data-ttu-id="e188e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-148">Int32</span></span>|<span data-ttu-id="e188e-149">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="e188e-149">Number of error devices</span></span>|
|<span data-ttu-id="e188e-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e188e-150">conflictDeviceCount</span></span>|<span data-ttu-id="e188e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e188e-151">Int32</span></span>|<span data-ttu-id="e188e-152">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="e188e-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e188e-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="e188e-153">Response</span></span>
<span data-ttu-id="e188e-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e188e-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e188e-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e188e-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="e188e-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e188e-156">Request</span></span>
<span data-ttu-id="e188e-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e188e-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="e188e-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="e188e-158">Response</span></span>
<span data-ttu-id="e188e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e188e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



