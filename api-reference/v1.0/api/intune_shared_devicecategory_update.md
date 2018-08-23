# <a name="update-devicecategory"></a><span data-ttu-id="4e5fc-101">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="4e5fc-101">Update deviceCategory</span></span>

> <span data-ttu-id="4e5fc-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e5fc-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="4e5fc-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e5fc-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e5fc-104">Prerequisites</span></span>
<span data-ttu-id="4e5fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e5fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4e5fc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e5fc-107">Permission type</span></span>|<span data-ttu-id="4e5fc-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e5fc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e5fc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e5fc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4e5fc-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e5fc-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4e5fc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e5fc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e5fc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e5fc-112">Not supported.</span></span>|
|<span data-ttu-id="4e5fc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e5fc-113">Application</span></span>|<span data-ttu-id="4e5fc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e5fc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e5fc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e5fc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="4e5fc-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e5fc-116">Request headers</span></span>
|<span data-ttu-id="4e5fc-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4e5fc-117">Header</span></span>|<span data-ttu-id="4e5fc-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4e5fc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e5fc-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4e5fc-119">Authorization</span></span>|<span data-ttu-id="4e5fc-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e5fc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e5fc-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="4e5fc-121">Accept</span></span>|<span data-ttu-id="4e5fc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4e5fc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e5fc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e5fc-123">Request body</span></span>
<span data-ttu-id="4e5fc-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-124">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="4e5fc-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-125">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="4e5fc-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e5fc-126">Property</span></span>|<span data-ttu-id="4e5fc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4e5fc-127">Type</span></span>|<span data-ttu-id="4e5fc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e5fc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e5fc-129">id</span><span class="sxs-lookup"><span data-stu-id="4e5fc-129">id</span></span>|<span data-ttu-id="4e5fc-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e5fc-130">String</span></span>|<span data-ttu-id="4e5fc-131">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-131">Unique identifier for the device category.</span></span> <span data-ttu-id="4e5fc-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-132">Read-only.</span></span>|
|<span data-ttu-id="4e5fc-133">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="4e5fc-133">**On-boarding**</span></span>|
|<span data-ttu-id="4e5fc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4e5fc-134">displayName</span></span>|<span data-ttu-id="4e5fc-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e5fc-135">String</span></span>|<span data-ttu-id="4e5fc-136">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-136">Display name for the device category.</span></span>|
|<span data-ttu-id="4e5fc-137">description</span><span class="sxs-lookup"><span data-stu-id="4e5fc-137">description</span></span>|<span data-ttu-id="4e5fc-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e5fc-138">String</span></span>|<span data-ttu-id="4e5fc-139">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-139">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="4e5fc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e5fc-140">Response</span></span>
<span data-ttu-id="4e5fc-141">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-141">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e5fc-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e5fc-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e5fc-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e5fc-143">Request</span></span>
<span data-ttu-id="4e5fc-144">Es folgen Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-144">Here are a couple of examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="4e5fc-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e5fc-145">Response</span></span>
<span data-ttu-id="4e5fc-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-146">Here is an example of the response.</span></span> <span data-ttu-id="4e5fc-147">Hinweis: Das hier gezeigte Response-Objekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4e5fc-148">Response-Eigenschaften variieren entsprechend Kontext.</span><span class="sxs-lookup"><span data-stu-id="4e5fc-148">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



