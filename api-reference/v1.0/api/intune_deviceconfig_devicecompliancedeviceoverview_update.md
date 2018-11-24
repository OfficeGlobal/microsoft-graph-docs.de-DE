# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="03ba2-101">Aktualisieren von „deviceComplianceDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="03ba2-101">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="03ba2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="03ba2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03ba2-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="03ba2-103">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03ba2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="03ba2-104">Prerequisites</span></span>
<span data-ttu-id="03ba2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03ba2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="03ba2-107">Permission type</span></span>|<span data-ttu-id="03ba2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="03ba2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03ba2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="03ba2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="03ba2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03ba2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03ba2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="03ba2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03ba2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="03ba2-112">Not supported.</span></span>|
|<span data-ttu-id="03ba2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="03ba2-113">Application</span></span>|<span data-ttu-id="03ba2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="03ba2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03ba2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="03ba2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="03ba2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="03ba2-116">Request headers</span></span>
|<span data-ttu-id="03ba2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="03ba2-117">Header</span></span>|<span data-ttu-id="03ba2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="03ba2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03ba2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="03ba2-119">Authorization</span></span>|<span data-ttu-id="03ba2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="03ba2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03ba2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="03ba2-121">Accept</span></span>|<span data-ttu-id="03ba2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="03ba2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ba2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="03ba2-123">Request body</span></span>
<span data-ttu-id="03ba2-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="03ba2-124">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="03ba2-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="03ba2-125">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="03ba2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03ba2-126">Property</span></span>|<span data-ttu-id="03ba2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="03ba2-127">Type</span></span>|<span data-ttu-id="03ba2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03ba2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03ba2-129">id</span><span class="sxs-lookup"><span data-stu-id="03ba2-129">id</span></span>|<span data-ttu-id="03ba2-130">String</span><span class="sxs-lookup"><span data-stu-id="03ba2-130">String</span></span>|<span data-ttu-id="03ba2-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="03ba2-131">Key of the entity.</span></span>|
|<span data-ttu-id="03ba2-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="03ba2-132">pendingCount</span></span>|<span data-ttu-id="03ba2-133">Int32</span><span class="sxs-lookup"><span data-stu-id="03ba2-133">Int32</span></span>|<span data-ttu-id="03ba2-134">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="03ba2-134">Number of pending devices</span></span>|
|<span data-ttu-id="03ba2-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="03ba2-135">notApplicableCount</span></span>|<span data-ttu-id="03ba2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="03ba2-136">Int32</span></span>|<span data-ttu-id="03ba2-137">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="03ba2-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="03ba2-138">successCount</span><span class="sxs-lookup"><span data-stu-id="03ba2-138">successCount</span></span>|<span data-ttu-id="03ba2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="03ba2-139">Int32</span></span>|<span data-ttu-id="03ba2-140">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="03ba2-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="03ba2-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="03ba2-141">errorCount</span></span>|<span data-ttu-id="03ba2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="03ba2-142">Int32</span></span>|<span data-ttu-id="03ba2-143">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="03ba2-143">Number of error devices</span></span>|
|<span data-ttu-id="03ba2-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="03ba2-144">failedCount</span></span>|<span data-ttu-id="03ba2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="03ba2-145">Int32</span></span>|<span data-ttu-id="03ba2-146">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="03ba2-146">Number of failed devices</span></span>|
|<span data-ttu-id="03ba2-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="03ba2-147">lastUpdateDateTime</span></span>|<span data-ttu-id="03ba2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03ba2-148">DateTimeOffset</span></span>|<span data-ttu-id="03ba2-149">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="03ba2-149">Last update time</span></span>|
|<span data-ttu-id="03ba2-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="03ba2-150">configurationVersion</span></span>|<span data-ttu-id="03ba2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="03ba2-151">Int32</span></span>|<span data-ttu-id="03ba2-152">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="03ba2-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="03ba2-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="03ba2-153">Response</span></span>
<span data-ttu-id="03ba2-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="03ba2-154">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03ba2-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03ba2-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="03ba2-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="03ba2-156">Request</span></span>
<span data-ttu-id="03ba2-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="03ba2-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="03ba2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="03ba2-158">Response</span></span>
<span data-ttu-id="03ba2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03ba2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



