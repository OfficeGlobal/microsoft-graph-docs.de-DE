# <a name="update-deviceinstallstate"></a><span data-ttu-id="8870e-101">Aktualisieren von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="8870e-101">Update deviceInstallState</span></span>

> <span data-ttu-id="8870e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8870e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8870e-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="8870e-103">Update the properties of a [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8870e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8870e-104">Prerequisites</span></span>
<span data-ttu-id="8870e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8870e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8870e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8870e-107">Permission type</span></span>|<span data-ttu-id="8870e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8870e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8870e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8870e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8870e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8870e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8870e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8870e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8870e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8870e-112">Not supported.</span></span>|
|<span data-ttu-id="8870e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8870e-113">Application</span></span>|<span data-ttu-id="8870e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8870e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8870e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8870e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8870e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8870e-116">Request headers</span></span>
|<span data-ttu-id="8870e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8870e-117">Header</span></span>|<span data-ttu-id="8870e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8870e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8870e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8870e-119">Authorization</span></span>|<span data-ttu-id="8870e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8870e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8870e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8870e-121">Accept</span></span>|<span data-ttu-id="8870e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8870e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8870e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8870e-123">Request body</span></span>
<span data-ttu-id="8870e-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="8870e-124">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>

<span data-ttu-id="8870e-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8870e-125">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span></span>

|<span data-ttu-id="8870e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8870e-126">Property</span></span>|<span data-ttu-id="8870e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8870e-127">Type</span></span>|<span data-ttu-id="8870e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8870e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8870e-129">id</span><span class="sxs-lookup"><span data-stu-id="8870e-129">id</span></span>|<span data-ttu-id="8870e-130">String</span><span class="sxs-lookup"><span data-stu-id="8870e-130">String</span></span>|<span data-ttu-id="8870e-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8870e-131">Key of the entity.</span></span>|
|<span data-ttu-id="8870e-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="8870e-132">deviceName</span></span>|<span data-ttu-id="8870e-133">String</span><span class="sxs-lookup"><span data-stu-id="8870e-133">String</span></span>|<span data-ttu-id="8870e-134">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="8870e-134">Device name.</span></span>|
|<span data-ttu-id="8870e-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="8870e-135">deviceId</span></span>|<span data-ttu-id="8870e-136">String</span><span class="sxs-lookup"><span data-stu-id="8870e-136">String</span></span>|<span data-ttu-id="8870e-137">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="8870e-137">Device Id.</span></span>|
|<span data-ttu-id="8870e-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8870e-138">lastSyncDateTime</span></span>|<span data-ttu-id="8870e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8870e-139">DateTimeOffset</span></span>|<span data-ttu-id="8870e-140">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="8870e-140">Last sync date and time.</span></span>|
|<span data-ttu-id="8870e-141">installState</span><span class="sxs-lookup"><span data-stu-id="8870e-141">installState</span></span>|[<span data-ttu-id="8870e-142">installState</span><span class="sxs-lookup"><span data-stu-id="8870e-142">installState</span></span>](../resources/intune_books_installstate.md)|<span data-ttu-id="8870e-143">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="8870e-143">The install state of the eBook.</span></span> <span data-ttu-id="8870e-144">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8870e-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="8870e-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="8870e-145">errorCode</span></span>|<span data-ttu-id="8870e-146">String</span><span class="sxs-lookup"><span data-stu-id="8870e-146">String</span></span>|<span data-ttu-id="8870e-147">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="8870e-147">The error code for install failures.</span></span>|
|<span data-ttu-id="8870e-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="8870e-148">osVersion</span></span>|<span data-ttu-id="8870e-149">String</span><span class="sxs-lookup"><span data-stu-id="8870e-149">String</span></span>|<span data-ttu-id="8870e-150">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="8870e-150">OS Version.</span></span>|
|<span data-ttu-id="8870e-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="8870e-151">osDescription</span></span>|<span data-ttu-id="8870e-152">String</span><span class="sxs-lookup"><span data-stu-id="8870e-152">String</span></span>|<span data-ttu-id="8870e-153">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="8870e-153">OS Description.</span></span>|
|<span data-ttu-id="8870e-154">userName</span><span class="sxs-lookup"><span data-stu-id="8870e-154">userName</span></span>|<span data-ttu-id="8870e-155">String</span><span class="sxs-lookup"><span data-stu-id="8870e-155">String</span></span>|<span data-ttu-id="8870e-156">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="8870e-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="8870e-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="8870e-157">Response</span></span>
<span data-ttu-id="8870e-158">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `200 OK` und ein aktualisiertes Objekt des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8870e-158">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8870e-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8870e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="8870e-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8870e-160">Request</span></span>
<span data-ttu-id="8870e-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8870e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="8870e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="8870e-162">Response</span></span>
<span data-ttu-id="8870e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8870e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```



