# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="0237f-101">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="0237f-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="0237f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0237f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0237f-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0237f-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0237f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0237f-104">Prerequisites</span></span>
<span data-ttu-id="0237f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0237f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0237f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0237f-107">Permission type</span></span>|<span data-ttu-id="0237f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0237f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0237f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0237f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0237f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0237f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0237f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0237f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0237f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0237f-112">Not supported.</span></span>|
|<span data-ttu-id="0237f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0237f-113">Application</span></span>|<span data-ttu-id="0237f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0237f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0237f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0237f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="0237f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0237f-116">Request headers</span></span>
|<span data-ttu-id="0237f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0237f-117">Header</span></span>|<span data-ttu-id="0237f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0237f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0237f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0237f-119">Authorization</span></span>|<span data-ttu-id="0237f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0237f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0237f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0237f-121">Accept</span></span>|<span data-ttu-id="0237f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0237f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0237f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0237f-123">Request body</span></span>
<span data-ttu-id="0237f-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="0237f-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="0237f-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0237f-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="0237f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0237f-126">Property</span></span>|<span data-ttu-id="0237f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0237f-127">Type</span></span>|<span data-ttu-id="0237f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0237f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0237f-129">id</span><span class="sxs-lookup"><span data-stu-id="0237f-129">id</span></span>|<span data-ttu-id="0237f-130">String</span><span class="sxs-lookup"><span data-stu-id="0237f-130">String</span></span>|<span data-ttu-id="0237f-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0237f-131">Key of the setting.</span></span>|
|<span data-ttu-id="0237f-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-132">unknownDeviceCount</span></span>|<span data-ttu-id="0237f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-133">Int32</span></span>|<span data-ttu-id="0237f-134">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="0237f-134">Number of unknown devices</span></span>|
|<span data-ttu-id="0237f-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="0237f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-136">Int32</span></span>|<span data-ttu-id="0237f-137">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="0237f-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="0237f-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-138">compliantDeviceCount</span></span>|<span data-ttu-id="0237f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-139">Int32</span></span>|<span data-ttu-id="0237f-140">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="0237f-140">Number of compliant devices</span></span>|
|<span data-ttu-id="0237f-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-141">remediatedDeviceCount</span></span>|<span data-ttu-id="0237f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-142">Int32</span></span>|<span data-ttu-id="0237f-143">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="0237f-143">Number of remediated devices</span></span>|
|<span data-ttu-id="0237f-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0237f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-145">Int32</span></span>|<span data-ttu-id="0237f-146">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="0237f-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0237f-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-147">errorDeviceCount</span></span>|<span data-ttu-id="0237f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-148">Int32</span></span>|<span data-ttu-id="0237f-149">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="0237f-149">Number of error devices</span></span>|
|<span data-ttu-id="0237f-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0237f-150">conflictDeviceCount</span></span>|<span data-ttu-id="0237f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0237f-151">Int32</span></span>|<span data-ttu-id="0237f-152">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="0237f-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="0237f-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="0237f-153">Response</span></span>
<span data-ttu-id="0237f-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0237f-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0237f-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0237f-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0237f-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0237f-156">Request</span></span>
<span data-ttu-id="0237f-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0237f-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="0237f-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0237f-158">Response</span></span>
<span data-ttu-id="0237f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0237f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



