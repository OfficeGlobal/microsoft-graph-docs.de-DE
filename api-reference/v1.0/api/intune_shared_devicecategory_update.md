# <a name="update-devicecategory"></a><span data-ttu-id="30078-101">Aktualisieren von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="30078-101">Update deviceCategory</span></span>

> <span data-ttu-id="30078-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="30078-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30078-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="30078-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30078-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="30078-104">Prerequisites</span></span>
<span data-ttu-id="30078-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="30078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="30078-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30078-107">Permission type</span></span>|<span data-ttu-id="30078-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30078-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30078-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30078-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="30078-110">&nbsp;&nbsp; **Onboarding** und</span><span class="sxs-lookup"><span data-stu-id="30078-110">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="30078-111">&nbsp;&nbsp; **Gerätemanagement**</span><span class="sxs-lookup"><span data-stu-id="30078-111">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="30078-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30078-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="30078-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30078-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30078-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30078-114">Not supported.</span></span>|
|<span data-ttu-id="30078-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30078-115">Application</span></span>|<span data-ttu-id="30078-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30078-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30078-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30078-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="30078-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30078-118">Request headers</span></span>
|<span data-ttu-id="30078-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="30078-119">Header</span></span>|<span data-ttu-id="30078-120">Wert</span><span class="sxs-lookup"><span data-stu-id="30078-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30078-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30078-121">Authorization</span></span>|<span data-ttu-id="30078-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="30078-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30078-123">Accept</span><span class="sxs-lookup"><span data-stu-id="30078-123">Accept</span></span>|<span data-ttu-id="30078-124">application/json</span><span class="sxs-lookup"><span data-stu-id="30078-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30078-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30078-125">Request body</span></span>
<span data-ttu-id="30078-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="30078-126">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="30078-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="30078-127">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="30078-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30078-128">Property</span></span>|<span data-ttu-id="30078-129">Typ</span><span class="sxs-lookup"><span data-stu-id="30078-129">Type</span></span>|<span data-ttu-id="30078-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30078-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30078-131">id</span><span class="sxs-lookup"><span data-stu-id="30078-131">id</span></span>|<span data-ttu-id="30078-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30078-132">String</span></span>|<span data-ttu-id="30078-133">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="30078-133">Unique identifier for the device category.</span></span> <span data-ttu-id="30078-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="30078-134">Read-only.</span></span>|
|<span data-ttu-id="30078-135">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="30078-135">**Onboarding**</span></span>|
|<span data-ttu-id="30078-136">displayName</span><span class="sxs-lookup"><span data-stu-id="30078-136">displayName</span></span>|<span data-ttu-id="30078-137">String</span><span class="sxs-lookup"><span data-stu-id="30078-137">String</span></span>|<span data-ttu-id="30078-138">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="30078-138">Display name for the device category.</span></span>|
|<span data-ttu-id="30078-139">description</span><span class="sxs-lookup"><span data-stu-id="30078-139">description</span></span>|<span data-ttu-id="30078-140">String</span><span class="sxs-lookup"><span data-stu-id="30078-140">String</span></span>|<span data-ttu-id="30078-141">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="30078-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="30078-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="30078-142">Response</span></span>
<span data-ttu-id="30078-143">Bei erfolgreicher Ausführung, gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="30078-143">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30078-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30078-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="30078-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30078-145">Request</span></span>
<span data-ttu-id="30078-146">Es folgen Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30078-146">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30078-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="30078-147">Response</span></span>
<span data-ttu-id="30078-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30078-148">Here is an example of the response.</span></span> <span data-ttu-id="30078-149">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="30078-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="30078-150">Response-Eigenschaften variiert entsprechend Kontext.</span><span class="sxs-lookup"><span data-stu-id="30078-150">Response properties will vary according to context.</span></span>
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



