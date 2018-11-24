# <a name="create-detectedapp"></a><span data-ttu-id="468b5-101">Erstellen von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="468b5-101">Create detectedApp</span></span>

> <span data-ttu-id="468b5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="468b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="468b5-103">Diese Methode erstellt ein neues Objekt des Typs [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="468b5-103">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="468b5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="468b5-104">Prerequisites</span></span>
<span data-ttu-id="468b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="468b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="468b5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="468b5-107">Permission type</span></span>|<span data-ttu-id="468b5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="468b5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="468b5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="468b5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="468b5-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468b5-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="468b5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="468b5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="468b5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="468b5-112">Not supported.</span></span>|
|<span data-ttu-id="468b5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="468b5-113">Application</span></span>|<span data-ttu-id="468b5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="468b5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="468b5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="468b5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="468b5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="468b5-116">Request headers</span></span>
|<span data-ttu-id="468b5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="468b5-117">Header</span></span>|<span data-ttu-id="468b5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="468b5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="468b5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="468b5-119">Authorization</span></span>|<span data-ttu-id="468b5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="468b5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="468b5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="468b5-121">Accept</span></span>|<span data-ttu-id="468b5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="468b5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="468b5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="468b5-123">Request body</span></span>
<span data-ttu-id="468b5-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „detectedApp“ an.</span><span class="sxs-lookup"><span data-stu-id="468b5-124">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="468b5-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „detectedApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="468b5-125">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="468b5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="468b5-126">Property</span></span>|<span data-ttu-id="468b5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="468b5-127">Type</span></span>|<span data-ttu-id="468b5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="468b5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="468b5-129">id</span><span class="sxs-lookup"><span data-stu-id="468b5-129">id</span></span>|<span data-ttu-id="468b5-130">String</span><span class="sxs-lookup"><span data-stu-id="468b5-130">String</span></span>|<span data-ttu-id="468b5-131">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="468b5-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="468b5-132">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="468b5-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="468b5-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="468b5-133">Read-only.</span></span>|
|<span data-ttu-id="468b5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="468b5-134">displayName</span></span>|<span data-ttu-id="468b5-135">String</span><span class="sxs-lookup"><span data-stu-id="468b5-135">String</span></span>|<span data-ttu-id="468b5-136">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="468b5-136">Name of the discovered application.</span></span> <span data-ttu-id="468b5-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="468b5-137">Read-only</span></span>|
|<span data-ttu-id="468b5-138">version</span><span class="sxs-lookup"><span data-stu-id="468b5-138">version</span></span>|<span data-ttu-id="468b5-139">String</span><span class="sxs-lookup"><span data-stu-id="468b5-139">String</span></span>|<span data-ttu-id="468b5-140">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="468b5-140">Version of the discovered application.</span></span> <span data-ttu-id="468b5-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="468b5-141">Read-only</span></span>|
|<span data-ttu-id="468b5-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="468b5-142">sizeInByte</span></span>|<span data-ttu-id="468b5-143">Int64</span><span class="sxs-lookup"><span data-stu-id="468b5-143">Int64</span></span>|<span data-ttu-id="468b5-144">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="468b5-144">Discovered application size in bytes.</span></span> <span data-ttu-id="468b5-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="468b5-145">Read-only</span></span>|
|<span data-ttu-id="468b5-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="468b5-146">deviceCount</span></span>|<span data-ttu-id="468b5-147">Int32</span><span class="sxs-lookup"><span data-stu-id="468b5-147">Int32</span></span>|<span data-ttu-id="468b5-148">Anzahl von Geräten, auf denen die Anwendung installiert ist</span><span class="sxs-lookup"><span data-stu-id="468b5-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="468b5-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="468b5-149">Response</span></span>
<span data-ttu-id="468b5-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [detectedApp](../resources/intune_devices_detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="468b5-150">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="468b5-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="468b5-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="468b5-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="468b5-152">Request</span></span>
<span data-ttu-id="468b5-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="468b5-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="468b5-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="468b5-154">Response</span></span>
<span data-ttu-id="468b5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="468b5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



