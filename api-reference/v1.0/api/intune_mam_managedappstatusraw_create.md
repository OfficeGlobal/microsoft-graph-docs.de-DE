# <a name="create-managedappstatusraw"></a><span data-ttu-id="e20ee-101">Erstellen von „managedAppStatusRaw“</span><span class="sxs-lookup"><span data-stu-id="e20ee-101">Create managedAppStatusRaw</span></span>

> <span data-ttu-id="e20ee-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e20ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e20ee-103">Diese Methode erstellt ein neues Objekt des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="e20ee-103">Create a new [plannerBucket](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e20ee-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e20ee-104">Prerequisites</span></span>
<span data-ttu-id="e20ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e20ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e20ee-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e20ee-107">Permission type</span></span>|<span data-ttu-id="e20ee-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e20ee-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e20ee-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e20ee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e20ee-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e20ee-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e20ee-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e20ee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e20ee-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e20ee-112">Not supported.</span></span>|
|<span data-ttu-id="e20ee-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e20ee-113">Application</span></span>|<span data-ttu-id="e20ee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e20ee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e20ee-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e20ee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e20ee-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e20ee-116">Request headers</span></span>
|<span data-ttu-id="e20ee-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e20ee-117">Header</span></span>|<span data-ttu-id="e20ee-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e20ee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e20ee-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e20ee-119">Authorization</span></span>|<span data-ttu-id="e20ee-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e20ee-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e20ee-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e20ee-121">Accept</span></span>|<span data-ttu-id="e20ee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e20ee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e20ee-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e20ee-123">Request body</span></span>
<span data-ttu-id="e20ee-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedAppStatusRaw“ an.</span><span class="sxs-lookup"><span data-stu-id="e20ee-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="e20ee-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedAppStatusRaw“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e20ee-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="e20ee-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e20ee-126">Property</span></span>|<span data-ttu-id="e20ee-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e20ee-127">Type</span></span>|<span data-ttu-id="e20ee-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e20ee-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e20ee-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e20ee-129">displayName</span></span>|<span data-ttu-id="e20ee-130">String</span><span class="sxs-lookup"><span data-stu-id="e20ee-130">String</span></span>|<span data-ttu-id="e20ee-131">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="e20ee-131">Friendly name of the status report.</span></span> <span data-ttu-id="e20ee-132">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e20ee-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="e20ee-133">id</span><span class="sxs-lookup"><span data-stu-id="e20ee-133">id</span></span>|<span data-ttu-id="e20ee-134">String</span><span class="sxs-lookup"><span data-stu-id="e20ee-134">String</span></span>|<span data-ttu-id="e20ee-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="e20ee-135">Key of the setting.</span></span> <span data-ttu-id="e20ee-136">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e20ee-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="e20ee-137">version</span><span class="sxs-lookup"><span data-stu-id="e20ee-137">version</span></span>|<span data-ttu-id="e20ee-138">String</span><span class="sxs-lookup"><span data-stu-id="e20ee-138">String</span></span>|<span data-ttu-id="e20ee-139">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="e20ee-139">Version of the entity.</span></span> <span data-ttu-id="e20ee-140">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e20ee-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="e20ee-141">content</span><span class="sxs-lookup"><span data-stu-id="e20ee-141">content</span></span>|[<span data-ttu-id="e20ee-142">Json</span><span class="sxs-lookup"><span data-stu-id="e20ee-142">json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="e20ee-143">Inhalt des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="e20ee-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="e20ee-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e20ee-144">Response</span></span>
<span data-ttu-id="e20ee-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e20ee-145">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e20ee-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e20ee-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e20ee-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e20ee-147">Request</span></span>
<span data-ttu-id="e20ee-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e20ee-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="e20ee-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e20ee-149">Response</span></span>
<span data-ttu-id="e20ee-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e20ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



