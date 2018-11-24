# <a name="create-deviceinstallstate"></a><span data-ttu-id="a261b-101">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="a261b-101">Create deviceInstallState</span></span>

> <span data-ttu-id="a261b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a261b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a261b-103">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="a261b-103">Create a new [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a261b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a261b-104">Prerequisites</span></span>
<span data-ttu-id="a261b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a261b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a261b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a261b-107">Permission type</span></span>|<span data-ttu-id="a261b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a261b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a261b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a261b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a261b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a261b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a261b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a261b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a261b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a261b-112">Not supported.</span></span>|
|<span data-ttu-id="a261b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a261b-113">Application</span></span>|<span data-ttu-id="a261b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a261b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a261b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a261b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="a261b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a261b-116">Request headers</span></span>
|<span data-ttu-id="a261b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a261b-117">Header</span></span>|<span data-ttu-id="a261b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a261b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a261b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a261b-119">Authorization</span></span>|<span data-ttu-id="a261b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a261b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a261b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a261b-121">Accept</span></span>|<span data-ttu-id="a261b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a261b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a261b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a261b-123">Request body</span></span>
<span data-ttu-id="a261b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="a261b-124">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="a261b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a261b-125">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="a261b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a261b-126">Property</span></span>|<span data-ttu-id="a261b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a261b-127">Type</span></span>|<span data-ttu-id="a261b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a261b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a261b-129">id</span><span class="sxs-lookup"><span data-stu-id="a261b-129">id</span></span>|<span data-ttu-id="a261b-130">String</span><span class="sxs-lookup"><span data-stu-id="a261b-130">String</span></span>|<span data-ttu-id="a261b-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a261b-131">Key of the entity.</span></span>|
|<span data-ttu-id="a261b-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="a261b-132">deviceName</span></span>|<span data-ttu-id="a261b-133">String</span><span class="sxs-lookup"><span data-stu-id="a261b-133">String</span></span>|<span data-ttu-id="a261b-134">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="a261b-134">Device name.</span></span>|
|<span data-ttu-id="a261b-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="a261b-135">deviceId</span></span>|<span data-ttu-id="a261b-136">String</span><span class="sxs-lookup"><span data-stu-id="a261b-136">String</span></span>|<span data-ttu-id="a261b-137">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="a261b-137">Device Id.</span></span>|
|<span data-ttu-id="a261b-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a261b-138">lastSyncDateTime</span></span>|<span data-ttu-id="a261b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a261b-139">DateTimeOffset</span></span>|<span data-ttu-id="a261b-140">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="a261b-140">Last sync date and time.</span></span>|
|<span data-ttu-id="a261b-141">installState</span><span class="sxs-lookup"><span data-stu-id="a261b-141">installState</span></span>|[<span data-ttu-id="a261b-142">installState</span><span class="sxs-lookup"><span data-stu-id="a261b-142">installState</span></span>](../resources/intune_books_installstate.md)|<span data-ttu-id="a261b-143">Der Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="a261b-143">The install state of the eBook.</span></span> <span data-ttu-id="a261b-144">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a261b-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="a261b-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="a261b-145">errorCode</span></span>|<span data-ttu-id="a261b-146">String</span><span class="sxs-lookup"><span data-stu-id="a261b-146">String</span></span>|<span data-ttu-id="a261b-147">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="a261b-147">The error code for install failures.</span></span>|
|<span data-ttu-id="a261b-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="a261b-148">osVersion</span></span>|<span data-ttu-id="a261b-149">String</span><span class="sxs-lookup"><span data-stu-id="a261b-149">String</span></span>|<span data-ttu-id="a261b-150">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="a261b-150">OS Version.</span></span>|
|<span data-ttu-id="a261b-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="a261b-151">osDescription</span></span>|<span data-ttu-id="a261b-152">String</span><span class="sxs-lookup"><span data-stu-id="a261b-152">String</span></span>|<span data-ttu-id="a261b-153">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="a261b-153">OS Description.</span></span>|
|<span data-ttu-id="a261b-154">userName</span><span class="sxs-lookup"><span data-stu-id="a261b-154">userName</span></span>|<span data-ttu-id="a261b-155">String</span><span class="sxs-lookup"><span data-stu-id="a261b-155">String</span></span>|<span data-ttu-id="a261b-156">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="a261b-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="a261b-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="a261b-157">Response</span></span>
<span data-ttu-id="a261b-158">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a261b-158">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a261b-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a261b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="a261b-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a261b-160">Request</span></span>
<span data-ttu-id="a261b-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a261b-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="a261b-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="a261b-162">Response</span></span>
<span data-ttu-id="a261b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a261b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



