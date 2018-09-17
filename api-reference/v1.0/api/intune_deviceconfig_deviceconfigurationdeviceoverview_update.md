# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="2bb59-101">Aktualisieren von „deviceConfigurationDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="2bb59-101">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="2bb59-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2bb59-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bb59-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2bb59-103">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2bb59-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2bb59-104">Prerequisites</span></span>
<span data-ttu-id="2bb59-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2bb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2bb59-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2bb59-107">Permission type</span></span>|<span data-ttu-id="2bb59-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2bb59-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bb59-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2bb59-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2bb59-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb59-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bb59-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2bb59-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bb59-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bb59-112">Not supported.</span></span>|
|<span data-ttu-id="2bb59-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2bb59-113">Application</span></span>|<span data-ttu-id="2bb59-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bb59-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bb59-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bb59-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="2bb59-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2bb59-116">Request headers</span></span>
|<span data-ttu-id="2bb59-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2bb59-117">Header</span></span>|<span data-ttu-id="2bb59-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2bb59-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bb59-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2bb59-119">Authorization</span></span>|<span data-ttu-id="2bb59-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2bb59-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bb59-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2bb59-121">Accept</span></span>|<span data-ttu-id="2bb59-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="2bb59-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bb59-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2bb59-123">Request body</span></span>
<span data-ttu-id="2bb59-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="2bb59-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="2bb59-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2bb59-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="2bb59-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2bb59-126">Property</span></span>|<span data-ttu-id="2bb59-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2bb59-127">Type</span></span>|<span data-ttu-id="2bb59-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bb59-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bb59-129">ID</span><span class="sxs-lookup"><span data-stu-id="2bb59-129">id</span></span>|<span data-ttu-id="2bb59-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2bb59-130">String</span></span>|<span data-ttu-id="2bb59-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2bb59-131">Key of the entity.</span></span>|
|<span data-ttu-id="2bb59-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="2bb59-132">pendingCount</span></span>|<span data-ttu-id="2bb59-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb59-133">Int32</span></span>|<span data-ttu-id="2bb59-134">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="2bb59-134">Number of pending devices</span></span>|
|<span data-ttu-id="2bb59-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2bb59-135">notApplicableCount</span></span>|<span data-ttu-id="2bb59-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb59-136">Int32</span></span>|<span data-ttu-id="2bb59-137">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="2bb59-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="2bb59-138">successCount</span><span class="sxs-lookup"><span data-stu-id="2bb59-138">successCount</span></span>|<span data-ttu-id="2bb59-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb59-139">Int32</span></span>|<span data-ttu-id="2bb59-140">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="2bb59-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="2bb59-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="2bb59-141">errorCount</span></span>|<span data-ttu-id="2bb59-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb59-142">Int32</span></span>|<span data-ttu-id="2bb59-143">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="2bb59-143">Number of error devices</span></span>|
|<span data-ttu-id="2bb59-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="2bb59-144">failedCount</span></span>|<span data-ttu-id="2bb59-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb59-145">Int32</span></span>|<span data-ttu-id="2bb59-146">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="2bb59-146">Number of failed devices</span></span>|
|<span data-ttu-id="2bb59-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb59-147">lastUpdateDateTime</span></span>|<span data-ttu-id="2bb59-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb59-148">DateTimeOffset</span></span>|<span data-ttu-id="2bb59-149">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="2bb59-149">Last update time</span></span>|
|<span data-ttu-id="2bb59-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="2bb59-150">configurationVersion</span></span>|<span data-ttu-id="2bb59-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb59-151">Int32</span></span>|<span data-ttu-id="2bb59-152">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="2bb59-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="2bb59-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bb59-153">Response</span></span>
<span data-ttu-id="2bb59-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2bb59-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bb59-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2bb59-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="2bb59-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bb59-156">Request</span></span>
<span data-ttu-id="2bb59-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2bb59-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="2bb59-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bb59-158">Response</span></span>
<span data-ttu-id="2bb59-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2bb59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








