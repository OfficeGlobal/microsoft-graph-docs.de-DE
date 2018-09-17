# <a name="update-manageddeviceoverview"></a><span data-ttu-id="344de-101">Aktualisieren von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="344de-101">Update managedDeviceOverview</span></span>

> <span data-ttu-id="344de-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="344de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="344de-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="344de-103">Update the properties of a [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="344de-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="344de-104">Prerequisites</span></span>
<span data-ttu-id="344de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="344de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="344de-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="344de-107">Permission type</span></span>|<span data-ttu-id="344de-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="344de-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="344de-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="344de-109">Delegated (work or school account)</span></span>|<span data-ttu-id="344de-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344de-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="344de-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="344de-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="344de-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="344de-112">Not supported.</span></span>|
|<span data-ttu-id="344de-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="344de-113">Application</span></span>|<span data-ttu-id="344de-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="344de-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="344de-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="344de-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="344de-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="344de-116">Request headers</span></span>
|<span data-ttu-id="344de-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="344de-117">Header</span></span>|<span data-ttu-id="344de-118">Wert</span><span class="sxs-lookup"><span data-stu-id="344de-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="344de-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="344de-119">Authorization</span></span>|<span data-ttu-id="344de-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="344de-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="344de-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="344de-121">Accept</span></span>|<span data-ttu-id="344de-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="344de-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="344de-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="344de-123">Request body</span></span>
<span data-ttu-id="344de-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="344de-124">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="344de-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="344de-125">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span></span>

|<span data-ttu-id="344de-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="344de-126">Property</span></span>|<span data-ttu-id="344de-127">Typ</span><span class="sxs-lookup"><span data-stu-id="344de-127">Type</span></span>|<span data-ttu-id="344de-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="344de-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="344de-129">ID</span><span class="sxs-lookup"><span data-stu-id="344de-129">id</span></span>|<span data-ttu-id="344de-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="344de-130">String</span></span>|<span data-ttu-id="344de-131">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="344de-131">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="344de-132">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="344de-132">enrolledDeviceCount</span></span>|<span data-ttu-id="344de-133">Int32</span><span class="sxs-lookup"><span data-stu-id="344de-133">Int32</span></span>|<span data-ttu-id="344de-134">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="344de-134">Total enrolled device count.</span></span> <span data-ttu-id="344de-135">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="344de-135">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="344de-136">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="344de-136">mdmEnrolledCount</span></span>|<span data-ttu-id="344de-137">Int32</span><span class="sxs-lookup"><span data-stu-id="344de-137">Int32</span></span>|<span data-ttu-id="344de-138">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="344de-138">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="344de-139">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="344de-139">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="344de-140">Int32</span><span class="sxs-lookup"><span data-stu-id="344de-140">Int32</span></span>|<span data-ttu-id="344de-141">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="344de-141">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="344de-142">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="344de-142">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="344de-143">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="344de-143">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="344de-144">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="344de-144">Device operating system summary.</span></span>|
|<span data-ttu-id="344de-145">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="344de-145">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="344de-146">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="344de-146">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="344de-147">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="344de-147">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="344de-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="344de-148">Response</span></span>
<span data-ttu-id="344de-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="344de-149">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="344de-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="344de-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="344de-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="344de-151">Request</span></span>
<span data-ttu-id="344de-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="344de-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 625

{
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```

### <a name="response"></a><span data-ttu-id="344de-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="344de-153">Response</span></span>
<span data-ttu-id="344de-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="344de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```








