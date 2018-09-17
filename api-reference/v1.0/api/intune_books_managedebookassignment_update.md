# <a name="update-managedebookassignment"></a><span data-ttu-id="1ef8b-101">Aktualisieren von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="1ef8b-101">Update managedEBookAssignment</span></span>

> <span data-ttu-id="1ef8b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ef8b-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ef8b-103">Update the properties of a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ef8b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ef8b-104">Prerequisites</span></span>
<span data-ttu-id="1ef8b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ef8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ef8b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ef8b-107">Permission type</span></span>|<span data-ttu-id="1ef8b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ef8b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ef8b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ef8b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1ef8b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef8b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ef8b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ef8b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ef8b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ef8b-112">Not supported.</span></span>|
|<span data-ttu-id="1ef8b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ef8b-113">Application</span></span>|<span data-ttu-id="1ef8b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ef8b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ef8b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ef8b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1ef8b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ef8b-116">Request headers</span></span>
|<span data-ttu-id="1ef8b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1ef8b-117">Header</span></span>|<span data-ttu-id="1ef8b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1ef8b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ef8b-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1ef8b-119">Authorization</span></span>|<span data-ttu-id="1ef8b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ef8b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ef8b-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1ef8b-121">Accept</span></span>|<span data-ttu-id="1ef8b-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1ef8b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef8b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ef8b-123">Request body</span></span>
<span data-ttu-id="1ef8b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-124">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>

<span data-ttu-id="1ef8b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-125">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span></span>

|<span data-ttu-id="1ef8b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ef8b-126">Property</span></span>|<span data-ttu-id="1ef8b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1ef8b-127">Type</span></span>|<span data-ttu-id="1ef8b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ef8b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef8b-129">ID</span><span class="sxs-lookup"><span data-stu-id="1ef8b-129">id</span></span>|<span data-ttu-id="1ef8b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ef8b-130">String</span></span>|<span data-ttu-id="1ef8b-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1ef8b-131">Key of the entity.</span></span>|
|<span data-ttu-id="1ef8b-132">Ziel</span><span class="sxs-lookup"><span data-stu-id="1ef8b-132">target</span></span>|[<span data-ttu-id="1ef8b-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1ef8b-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1ef8b-134">Zuweisungsziel für das E-Book</span><span class="sxs-lookup"><span data-stu-id="1ef8b-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="1ef8b-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="1ef8b-135">installIntent</span></span>|[<span data-ttu-id="1ef8b-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="1ef8b-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="1ef8b-137">Installationsabsicht für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-137">The install intent for eBook.</span></span> <span data-ttu-id="1ef8b-138">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-138">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ef8b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ef8b-139">Response</span></span>
<span data-ttu-id="1ef8b-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-140">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef8b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ef8b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ef8b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ef8b-142">Request</span></span>
<span data-ttu-id="1ef8b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="1ef8b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ef8b-144">Response</span></span>
<span data-ttu-id="1ef8b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ef8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








