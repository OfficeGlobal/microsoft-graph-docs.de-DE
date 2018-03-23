# <a name="create-iosvppebookassignment"></a><span data-ttu-id="047c8-101">Erstellen von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="047c8-101">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="047c8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="047c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="047c8-103">Diese Methode erstellt ein neues Objekt des Typs [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="047c8-103">Create a new [plannerBucket](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="047c8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="047c8-104">Prerequisites</span></span>
<span data-ttu-id="047c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="047c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="047c8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="047c8-107">Permission type</span></span>|<span data-ttu-id="047c8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="047c8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="047c8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="047c8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="047c8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="047c8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="047c8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="047c8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="047c8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="047c8-112">Not supported.</span></span>|
|<span data-ttu-id="047c8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="047c8-113">Application</span></span>|<span data-ttu-id="047c8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="047c8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="047c8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="047c8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="047c8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="047c8-116">Request headers</span></span>
|<span data-ttu-id="047c8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="047c8-117">Header</span></span>|<span data-ttu-id="047c8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="047c8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="047c8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="047c8-119">Authorization</span></span>|<span data-ttu-id="047c8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="047c8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="047c8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="047c8-121">Accept</span></span>|<span data-ttu-id="047c8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="047c8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="047c8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="047c8-123">Request body</span></span>
<span data-ttu-id="047c8-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosVppEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="047c8-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="047c8-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosVppEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="047c8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="047c8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="047c8-126">Property</span></span>|<span data-ttu-id="047c8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="047c8-127">Type</span></span>|<span data-ttu-id="047c8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="047c8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="047c8-129">id</span><span class="sxs-lookup"><span data-stu-id="047c8-129">id</span></span>|<span data-ttu-id="047c8-130">String</span><span class="sxs-lookup"><span data-stu-id="047c8-130">String</span></span>|<span data-ttu-id="047c8-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="047c8-131">Key of the setting.</span></span> <span data-ttu-id="047c8-132">Geerbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="047c8-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="047c8-133">target</span><span class="sxs-lookup"><span data-stu-id="047c8-133">target</span></span>|[<span data-ttu-id="047c8-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="047c8-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="047c8-135">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="047c8-135">The assignment target for eBook.</span></span> <span data-ttu-id="047c8-136">Geerbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="047c8-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="047c8-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="047c8-137">installIntent</span></span>|<span data-ttu-id="047c8-138">String</span><span class="sxs-lookup"><span data-stu-id="047c8-138">String</span></span>|<span data-ttu-id="047c8-139">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="047c8-139">The install intent for eBook.</span></span> <span data-ttu-id="047c8-140">Geerbt von [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="047c8-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="047c8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="047c8-141">Response</span></span>
<span data-ttu-id="047c8-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="047c8-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="047c8-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="047c8-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="047c8-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="047c8-144">Request</span></span>
<span data-ttu-id="047c8-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="047c8-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="047c8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="047c8-146">Response</span></span>
<span data-ttu-id="047c8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="047c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



