# <a name="update-managedappstatusraw"></a><span data-ttu-id="a979b-101">Aktualisieren von „managedAppStatusRaw“</span><span class="sxs-lookup"><span data-stu-id="a979b-101">Update managedAppStatusRaw</span></span>

> <span data-ttu-id="a979b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a979b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a979b-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a979b-103">Update the properties of a [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a979b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a979b-104">Prerequisites</span></span>
<span data-ttu-id="a979b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a979b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a979b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a979b-107">Permission type</span></span>|<span data-ttu-id="a979b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a979b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a979b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a979b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a979b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a979b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a979b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a979b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a979b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a979b-112">Not supported.</span></span>|
|<span data-ttu-id="a979b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a979b-113">Application</span></span>|<span data-ttu-id="a979b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a979b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a979b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a979b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a979b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a979b-116">Request headers</span></span>
|<span data-ttu-id="a979b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a979b-117">Header</span></span>|<span data-ttu-id="a979b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a979b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a979b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a979b-119">Authorization</span></span>|<span data-ttu-id="a979b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a979b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a979b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a979b-121">Accept</span></span>|<span data-ttu-id="a979b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a979b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a979b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a979b-123">Request body</span></span>
<span data-ttu-id="a979b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) an.</span><span class="sxs-lookup"><span data-stu-id="a979b-124">In the request body, supply a JSON representation for the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>

<span data-ttu-id="a979b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a979b-125">The following table shows the properties that are required when you create the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span></span>

|<span data-ttu-id="a979b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a979b-126">Property</span></span>|<span data-ttu-id="a979b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a979b-127">Type</span></span>|<span data-ttu-id="a979b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a979b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a979b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a979b-129">displayName</span></span>|<span data-ttu-id="a979b-130">String</span><span class="sxs-lookup"><span data-stu-id="a979b-130">String</span></span>|<span data-ttu-id="a979b-131">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="a979b-131">Friendly name of the status report.</span></span> <span data-ttu-id="a979b-132">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a979b-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="a979b-133">id</span><span class="sxs-lookup"><span data-stu-id="a979b-133">id</span></span>|<span data-ttu-id="a979b-134">String</span><span class="sxs-lookup"><span data-stu-id="a979b-134">String</span></span>|<span data-ttu-id="a979b-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="a979b-135">Key of the entity.</span></span> <span data-ttu-id="a979b-136">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a979b-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="a979b-137">version</span><span class="sxs-lookup"><span data-stu-id="a979b-137">version</span></span>|<span data-ttu-id="a979b-138">String</span><span class="sxs-lookup"><span data-stu-id="a979b-138">String</span></span>|<span data-ttu-id="a979b-139">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="a979b-139">Version of the entity.</span></span> <span data-ttu-id="a979b-140">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a979b-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="a979b-141">content</span><span class="sxs-lookup"><span data-stu-id="a979b-141">content</span></span>|[<span data-ttu-id="a979b-142">Json</span><span class="sxs-lookup"><span data-stu-id="a979b-142">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="a979b-143">Inhalt des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="a979b-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="a979b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a979b-144">Response</span></span>
<span data-ttu-id="a979b-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a979b-145">If successful, this method returns a `200 OK` response code and an updated [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a979b-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a979b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="a979b-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a979b-147">Request</span></span>
<span data-ttu-id="a979b-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a979b-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
Content-type: application/json
Content-length: 139

{
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="a979b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="a979b-149">Response</span></span>
<span data-ttu-id="a979b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a979b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "id": "80847581-7581-8084-8175-848081758480",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



