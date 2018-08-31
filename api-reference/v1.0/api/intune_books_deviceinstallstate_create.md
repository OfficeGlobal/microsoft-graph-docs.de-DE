# <a name="create-deviceinstallstate"></a><span data-ttu-id="9a408-101">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="9a408-101">Create deviceInstallState</span></span>

> <span data-ttu-id="9a408-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9a408-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a408-103">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="9a408-103">Create a new [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a408-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9a408-104">Prerequisites</span></span>
<span data-ttu-id="9a408-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a408-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a408-107">Permission type</span></span>|<span data-ttu-id="9a408-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a408-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a408-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a408-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9a408-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a408-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9a408-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a408-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a408-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a408-112">Not supported.</span></span>|
|<span data-ttu-id="9a408-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a408-113">Application</span></span>|<span data-ttu-id="9a408-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a408-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a408-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a408-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="9a408-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a408-116">Request headers</span></span>
|<span data-ttu-id="9a408-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9a408-117">Header</span></span>|<span data-ttu-id="9a408-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9a408-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a408-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9a408-119">Authorization</span></span>|<span data-ttu-id="9a408-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a408-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a408-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="9a408-121">Accept</span></span>|<span data-ttu-id="9a408-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="9a408-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a408-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a408-123">Request body</span></span>
<span data-ttu-id="9a408-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="9a408-124">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="9a408-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9a408-125">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="9a408-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a408-126">Property</span></span>|<span data-ttu-id="9a408-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9a408-127">Type</span></span>|<span data-ttu-id="9a408-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a408-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a408-129">id</span><span class="sxs-lookup"><span data-stu-id="9a408-129">id</span></span>|<span data-ttu-id="9a408-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-130">String</span></span>|<span data-ttu-id="9a408-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9a408-131">Key of the entity.</span></span>|
|<span data-ttu-id="9a408-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="9a408-132">deviceName</span></span>|<span data-ttu-id="9a408-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-133">String</span></span>|<span data-ttu-id="9a408-134">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="9a408-134">Device name.</span></span>|
|<span data-ttu-id="9a408-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="9a408-135">deviceId</span></span>|<span data-ttu-id="9a408-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-136">String</span></span>|<span data-ttu-id="9a408-137">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="9a408-137">Device Id.</span></span>|
|<span data-ttu-id="9a408-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9a408-138">lastSyncDateTime</span></span>|<span data-ttu-id="9a408-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a408-139">DateTimeOffset</span></span>|<span data-ttu-id="9a408-140">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="9a408-140">Last sync date and time.</span></span>|
|<span data-ttu-id="9a408-141">installState</span><span class="sxs-lookup"><span data-stu-id="9a408-141">installState</span></span>|[<span data-ttu-id="9a408-142">installState</span><span class="sxs-lookup"><span data-stu-id="9a408-142">installState</span></span>](../resources/intune_books_installstate.md)|<span data-ttu-id="9a408-143">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="9a408-143">The install state of the eBook.</span></span> <span data-ttu-id="9a408-144">Mögliche Werte: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9a408-144">The possible values are `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="9a408-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="9a408-145">errorCode</span></span>|<span data-ttu-id="9a408-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-146">String</span></span>|<span data-ttu-id="9a408-147">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="9a408-147">The error code for install failures.</span></span>|
|<span data-ttu-id="9a408-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="9a408-148">osVersion</span></span>|<span data-ttu-id="9a408-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-149">String</span></span>|<span data-ttu-id="9a408-150">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="9a408-150">OS Version.</span></span>|
|<span data-ttu-id="9a408-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="9a408-151">osDescription</span></span>|<span data-ttu-id="9a408-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-152">String</span></span>|<span data-ttu-id="9a408-153">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="9a408-153">OS Description.</span></span>|
|<span data-ttu-id="9a408-154">userName</span><span class="sxs-lookup"><span data-stu-id="9a408-154">userName</span></span>|<span data-ttu-id="9a408-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9a408-155">String</span></span>|<span data-ttu-id="9a408-156">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="9a408-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="9a408-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a408-157">Response</span></span>
<span data-ttu-id="9a408-158">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9a408-158">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a408-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a408-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a408-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a408-160">Request</span></span>
<span data-ttu-id="9a408-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a408-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a408-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a408-162">Response</span></span>
<span data-ttu-id="9a408-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a408-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



