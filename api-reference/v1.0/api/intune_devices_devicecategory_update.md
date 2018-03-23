# <a name="update-devicecategory"></a><span data-ttu-id="2d9aa-101">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="2d9aa-101">Update deviceCategory</span></span>

> <span data-ttu-id="2d9aa-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d9aa-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune_devices_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2d9aa-103">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d9aa-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d9aa-104">Prerequisites</span></span>
<span data-ttu-id="2d9aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d9aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2d9aa-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d9aa-107">Permission type</span></span>|<span data-ttu-id="2d9aa-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d9aa-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d9aa-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d9aa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2d9aa-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9aa-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2d9aa-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d9aa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d9aa-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d9aa-112">Not supported.</span></span>|
|<span data-ttu-id="2d9aa-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d9aa-113">Application</span></span>|<span data-ttu-id="2d9aa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d9aa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d9aa-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d9aa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="2d9aa-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d9aa-116">Request headers</span></span>
|<span data-ttu-id="2d9aa-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2d9aa-117">Header</span></span>|<span data-ttu-id="2d9aa-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2d9aa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d9aa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d9aa-119">Authorization</span></span>|<span data-ttu-id="2d9aa-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2d9aa-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d9aa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2d9aa-121">Accept</span></span>|<span data-ttu-id="2d9aa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2d9aa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9aa-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d9aa-123">Request body</span></span>
<span data-ttu-id="2d9aa-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune_devices_devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_devices_devicecategory.md) object.</span></span>

<span data-ttu-id="2d9aa-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune_devices_devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="2d9aa-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d9aa-126">Property</span></span>|<span data-ttu-id="2d9aa-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2d9aa-127">Type</span></span>|<span data-ttu-id="2d9aa-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d9aa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d9aa-129">id</span><span class="sxs-lookup"><span data-stu-id="2d9aa-129">id</span></span>|<span data-ttu-id="2d9aa-130">String</span><span class="sxs-lookup"><span data-stu-id="2d9aa-130">String</span></span>|<span data-ttu-id="2d9aa-131">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-131">Unique identifier for the device category.</span></span> <span data-ttu-id="2d9aa-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-132">Read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="2d9aa-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d9aa-133">Response</span></span>
<span data-ttu-id="2d9aa-134">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune_devices_devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-134">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d9aa-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d9aa-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d9aa-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d9aa-136">Request</span></span>
<span data-ttu-id="2d9aa-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-137">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="2d9aa-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d9aa-138">Response</span></span>
<span data-ttu-id="2d9aa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d9aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```



