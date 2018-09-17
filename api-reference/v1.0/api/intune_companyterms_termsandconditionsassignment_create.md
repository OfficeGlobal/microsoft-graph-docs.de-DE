# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="d3d5c-101">Erstellen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="d3d5c-101">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="d3d5c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3d5c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3d5c-103">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d3d5c-103">Create a new [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3d5c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3d5c-104">Prerequisites</span></span>
<span data-ttu-id="d3d5c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3d5c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3d5c-107">Permission type</span></span>|<span data-ttu-id="d3d5c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3d5c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3d5c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3d5c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d3d5c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d5c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d3d5c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3d5c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3d5c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3d5c-112">Not supported.</span></span>|
|<span data-ttu-id="d3d5c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3d5c-113">Application</span></span>|<span data-ttu-id="d3d5c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3d5c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3d5c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3d5c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d3d5c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3d5c-116">Request headers</span></span>
|<span data-ttu-id="d3d5c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3d5c-117">Header</span></span>|<span data-ttu-id="d3d5c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d3d5c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3d5c-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d3d5c-119">Authorization</span></span>|<span data-ttu-id="d3d5c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3d5c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3d5c-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="d3d5c-121">Accept</span></span>|<span data-ttu-id="d3d5c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d3d5c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3d5c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3d5c-123">Request body</span></span>
<span data-ttu-id="d3d5c-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="d3d5c-124">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="d3d5c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d3d5c-125">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="d3d5c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3d5c-126">Property</span></span>|<span data-ttu-id="d3d5c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d3d5c-127">Type</span></span>|<span data-ttu-id="d3d5c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3d5c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d5c-129">ID</span><span class="sxs-lookup"><span data-stu-id="d3d5c-129">id</span></span>|<span data-ttu-id="d3d5c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3d5c-130">String</span></span>|<span data-ttu-id="d3d5c-131">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="d3d5c-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d3d5c-132">Ziel</span><span class="sxs-lookup"><span data-stu-id="d3d5c-132">target</span></span>|[<span data-ttu-id="d3d5c-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d3d5c-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d3d5c-134">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="d3d5c-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d3d5c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3d5c-135">Response</span></span>
<span data-ttu-id="d3d5c-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d3d5c-136">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3d5c-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3d5c-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3d5c-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3d5c-138">Request</span></span>
<span data-ttu-id="d3d5c-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3d5c-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d3d5c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3d5c-140">Response</span></span>
<span data-ttu-id="d3d5c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3d5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








