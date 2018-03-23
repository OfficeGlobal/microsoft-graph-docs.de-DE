# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="02a74-101">Erstellen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="02a74-101">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="02a74-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="02a74-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02a74-103">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02a74-103">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02a74-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02a74-104">Prerequisites</span></span>
<span data-ttu-id="02a74-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="02a74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02a74-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02a74-107">Permission type</span></span>|<span data-ttu-id="02a74-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02a74-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a74-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02a74-109">Delegated (work or school account)</span></span>|<span data-ttu-id="02a74-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a74-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="02a74-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02a74-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a74-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02a74-112">Not supported.</span></span>|
|<span data-ttu-id="02a74-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02a74-113">Application</span></span>|<span data-ttu-id="02a74-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02a74-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a74-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02a74-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="02a74-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02a74-116">Request headers</span></span>
|<span data-ttu-id="02a74-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="02a74-117">Header</span></span>|<span data-ttu-id="02a74-118">Wert</span><span class="sxs-lookup"><span data-stu-id="02a74-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a74-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a74-119">Authorization</span></span>|<span data-ttu-id="02a74-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02a74-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02a74-121">Accept</span><span class="sxs-lookup"><span data-stu-id="02a74-121">Accept</span></span>|<span data-ttu-id="02a74-122">application/json</span><span class="sxs-lookup"><span data-stu-id="02a74-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a74-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02a74-123">Request body</span></span>
<span data-ttu-id="02a74-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="02a74-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="02a74-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="02a74-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="02a74-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02a74-126">Property</span></span>|<span data-ttu-id="02a74-127">Typ</span><span class="sxs-lookup"><span data-stu-id="02a74-127">Type</span></span>|<span data-ttu-id="02a74-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02a74-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a74-129">id</span><span class="sxs-lookup"><span data-stu-id="02a74-129">id</span></span>|<span data-ttu-id="02a74-130">String</span><span class="sxs-lookup"><span data-stu-id="02a74-130">String</span></span>|<span data-ttu-id="02a74-131">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="02a74-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="02a74-132">target</span><span class="sxs-lookup"><span data-stu-id="02a74-132">target</span></span>|[<span data-ttu-id="02a74-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="02a74-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_companyterms_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="02a74-134">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="02a74-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="02a74-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="02a74-135">Response</span></span>
<span data-ttu-id="02a74-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="02a74-136">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_companyterms_termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a74-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02a74-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="02a74-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02a74-138">Request</span></span>
<span data-ttu-id="02a74-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02a74-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02a74-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="02a74-140">Response</span></span>
<span data-ttu-id="02a74-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02a74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



