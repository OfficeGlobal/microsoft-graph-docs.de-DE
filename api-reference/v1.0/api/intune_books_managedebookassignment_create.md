# <a name="create-managedebookassignment"></a><span data-ttu-id="a93d2-101">Erstellen von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="a93d2-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="a93d2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a93d2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a93d2-103">Diese Methode erstellt ein neues Objekt des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a93d2-103">Create a new [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a93d2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a93d2-104">Prerequisites</span></span>
<span data-ttu-id="a93d2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a93d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a93d2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a93d2-107">Permission type</span></span>|<span data-ttu-id="a93d2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a93d2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a93d2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a93d2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a93d2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a93d2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a93d2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a93d2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a93d2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a93d2-112">Not supported.</span></span>|
|<span data-ttu-id="a93d2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a93d2-113">Application</span></span>|<span data-ttu-id="a93d2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a93d2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a93d2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a93d2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a93d2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a93d2-116">Request headers</span></span>
|<span data-ttu-id="a93d2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a93d2-117">Header</span></span>|<span data-ttu-id="a93d2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a93d2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a93d2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a93d2-119">Authorization</span></span>|<span data-ttu-id="a93d2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a93d2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a93d2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a93d2-121">Accept</span></span>|<span data-ttu-id="a93d2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a93d2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a93d2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a93d2-123">Request body</span></span>
<span data-ttu-id="a93d2-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="a93d2-124">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="a93d2-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a93d2-125">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="a93d2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a93d2-126">Property</span></span>|<span data-ttu-id="a93d2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a93d2-127">Type</span></span>|<span data-ttu-id="a93d2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a93d2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a93d2-129">id</span><span class="sxs-lookup"><span data-stu-id="a93d2-129">id</span></span>|<span data-ttu-id="a93d2-130">String</span><span class="sxs-lookup"><span data-stu-id="a93d2-130">String</span></span>|<span data-ttu-id="a93d2-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a93d2-131">Key of the entity.</span></span>|
|<span data-ttu-id="a93d2-132">target</span><span class="sxs-lookup"><span data-stu-id="a93d2-132">target</span></span>|[<span data-ttu-id="a93d2-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a93d2-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a93d2-134">Zuweisungsziel für das E-Book</span><span class="sxs-lookup"><span data-stu-id="a93d2-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="a93d2-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="a93d2-135">installIntent</span></span>|[<span data-ttu-id="a93d2-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="a93d2-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="a93d2-137">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="a93d2-137">The install intent for eBook.</span></span> <span data-ttu-id="a93d2-138">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="a93d2-138">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="a93d2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a93d2-139">Response</span></span>
<span data-ttu-id="a93d2-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a93d2-140">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a93d2-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a93d2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a93d2-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a93d2-142">Request</span></span>
<span data-ttu-id="a93d2-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a93d2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="a93d2-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a93d2-144">Response</span></span>
<span data-ttu-id="a93d2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a93d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



