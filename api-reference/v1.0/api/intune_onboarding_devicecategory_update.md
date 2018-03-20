# <a name="update-devicecategory"></a><span data-ttu-id="31fbd-101">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="31fbd-101">Update deviceCategory</span></span>

> <span data-ttu-id="31fbd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31fbd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31fbd-103">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="31fbd-103">Update the properties of a [calendar](../resources/intune_onboarding_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31fbd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31fbd-104">Prerequisites</span></span>
<span data-ttu-id="31fbd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31fbd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31fbd-107">Permission type</span></span>|<span data-ttu-id="31fbd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31fbd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31fbd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31fbd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="31fbd-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31fbd-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="31fbd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31fbd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31fbd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31fbd-112">Not supported.</span></span>|
|<span data-ttu-id="31fbd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31fbd-113">Application</span></span>|<span data-ttu-id="31fbd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31fbd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31fbd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31fbd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="31fbd-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31fbd-116">Request headers</span></span>
|<span data-ttu-id="31fbd-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="31fbd-117">Header</span></span>|<span data-ttu-id="31fbd-118">Wert</span><span class="sxs-lookup"><span data-stu-id="31fbd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31fbd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="31fbd-119">Authorization</span></span>|<span data-ttu-id="31fbd-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31fbd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31fbd-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31fbd-121">Accept</span></span>|<span data-ttu-id="31fbd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="31fbd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31fbd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31fbd-123">Request body</span></span>
<span data-ttu-id="31fbd-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceCategory](../resources/intune_onboarding_devicecategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="31fbd-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_onboarding_devicecategory.md) object.</span></span>

<span data-ttu-id="31fbd-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCategory](../resources/intune_onboarding_devicecategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="31fbd-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="31fbd-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31fbd-126">Property</span></span>|<span data-ttu-id="31fbd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="31fbd-127">Type</span></span>|<span data-ttu-id="31fbd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31fbd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31fbd-129">id</span><span class="sxs-lookup"><span data-stu-id="31fbd-129">id</span></span>|<span data-ttu-id="31fbd-130">String</span><span class="sxs-lookup"><span data-stu-id="31fbd-130">String</span></span>|<span data-ttu-id="31fbd-131">Der eindeutige Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="31fbd-131">Unique identifier for the device category.</span></span> <span data-ttu-id="31fbd-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="31fbd-132">Read-only.</span></span>|
|<span data-ttu-id="31fbd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="31fbd-133">displayName</span></span>|<span data-ttu-id="31fbd-134">String</span><span class="sxs-lookup"><span data-stu-id="31fbd-134">String</span></span>|<span data-ttu-id="31fbd-135">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="31fbd-135">Display name for the device category.</span></span>|
|<span data-ttu-id="31fbd-136">description</span><span class="sxs-lookup"><span data-stu-id="31fbd-136">description</span></span>|<span data-ttu-id="31fbd-137">String</span><span class="sxs-lookup"><span data-stu-id="31fbd-137">String</span></span>|<span data-ttu-id="31fbd-138">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="31fbd-138">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="31fbd-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="31fbd-139">Response</span></span>
<span data-ttu-id="31fbd-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31fbd-140">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31fbd-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31fbd-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="31fbd-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31fbd-142">Request</span></span>
<span data-ttu-id="31fbd-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31fbd-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="31fbd-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="31fbd-144">Response</span></span>
<span data-ttu-id="31fbd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31fbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



