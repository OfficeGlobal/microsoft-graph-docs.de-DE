# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="8af39-101">Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="8af39-101">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="8af39-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8af39-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8af39-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8af39-103">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8af39-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8af39-104">Prerequisites</span></span>
<span data-ttu-id="8af39-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8af39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8af39-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8af39-107">Permission type</span></span>|<span data-ttu-id="8af39-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8af39-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8af39-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8af39-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8af39-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8af39-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8af39-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8af39-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8af39-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8af39-112">Not supported.</span></span>|
|<span data-ttu-id="8af39-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8af39-113">Application</span></span>|<span data-ttu-id="8af39-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8af39-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8af39-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8af39-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8af39-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8af39-116">Request headers</span></span>
|<span data-ttu-id="8af39-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8af39-117">Header</span></span>|<span data-ttu-id="8af39-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8af39-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8af39-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8af39-119">Authorization</span></span>|<span data-ttu-id="8af39-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8af39-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8af39-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8af39-121">Accept</span></span>|<span data-ttu-id="8af39-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8af39-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af39-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8af39-123">Request body</span></span>
<span data-ttu-id="8af39-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="8af39-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="8af39-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8af39-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="8af39-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8af39-126">Property</span></span>|<span data-ttu-id="8af39-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8af39-127">Type</span></span>|<span data-ttu-id="8af39-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8af39-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8af39-129">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="8af39-129">inGracePeriodCount</span></span>|<span data-ttu-id="8af39-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-130">Int32</span></span>|<span data-ttu-id="8af39-131">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="8af39-131">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="8af39-132">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="8af39-132">configManagerCount</span></span>|<span data-ttu-id="8af39-133">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-133">Int32</span></span>|<span data-ttu-id="8af39-134">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8af39-134">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="8af39-135">ID</span><span class="sxs-lookup"><span data-stu-id="8af39-135">id</span></span>|<span data-ttu-id="8af39-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8af39-136">String</span></span>|<span data-ttu-id="8af39-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8af39-137">Key of the entity.</span></span>|
|<span data-ttu-id="8af39-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-138">unknownDeviceCount</span></span>|<span data-ttu-id="8af39-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-139">Int32</span></span>|<span data-ttu-id="8af39-140">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="8af39-140">Number of unknown devices</span></span>|
|<span data-ttu-id="8af39-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="8af39-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-142">Int32</span></span>|<span data-ttu-id="8af39-143">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="8af39-143">Number of not applicable devices</span></span>|
|<span data-ttu-id="8af39-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-144">compliantDeviceCount</span></span>|<span data-ttu-id="8af39-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-145">Int32</span></span>|<span data-ttu-id="8af39-146">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="8af39-146">Number of compliant devices</span></span>|
|<span data-ttu-id="8af39-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-147">remediatedDeviceCount</span></span>|<span data-ttu-id="8af39-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-148">Int32</span></span>|<span data-ttu-id="8af39-149">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="8af39-149">Number of remediated devices</span></span>|
|<span data-ttu-id="8af39-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8af39-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-151">Int32</span></span>|<span data-ttu-id="8af39-152">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="8af39-152">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8af39-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-153">errorDeviceCount</span></span>|<span data-ttu-id="8af39-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-154">Int32</span></span>|<span data-ttu-id="8af39-155">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="8af39-155">Number of error devices</span></span>|
|<span data-ttu-id="8af39-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8af39-156">conflictDeviceCount</span></span>|<span data-ttu-id="8af39-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8af39-157">Int32</span></span>|<span data-ttu-id="8af39-158">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="8af39-158">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8af39-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="8af39-159">Response</span></span>
<span data-ttu-id="8af39-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8af39-160">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af39-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8af39-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="8af39-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8af39-162">Request</span></span>
<span data-ttu-id="8af39-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8af39-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="8af39-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="8af39-164">Response</span></span>
<span data-ttu-id="8af39-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8af39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```








