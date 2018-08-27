# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="2f8fc-101">Aktualisieren von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="2f8fc-101">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="2f8fc-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2f8fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f8fc-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f8fc-103">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f8fc-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f8fc-104">Prerequisites</span></span>
<span data-ttu-id="2f8fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f8fc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f8fc-107">Permission type</span></span>|<span data-ttu-id="2f8fc-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f8fc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f8fc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f8fc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2f8fc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f8fc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f8fc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f8fc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f8fc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f8fc-112">Not supported.</span></span>|
|<span data-ttu-id="2f8fc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f8fc-113">Application</span></span>|<span data-ttu-id="2f8fc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f8fc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f8fc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f8fc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2f8fc-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f8fc-116">Request headers</span></span>
|<span data-ttu-id="2f8fc-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f8fc-117">Header</span></span>|<span data-ttu-id="2f8fc-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2f8fc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f8fc-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2f8fc-119">Authorization</span></span>|<span data-ttu-id="2f8fc-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f8fc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f8fc-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2f8fc-121">Accept</span></span>|<span data-ttu-id="2f8fc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2f8fc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f8fc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f8fc-123">Request body</span></span>
<span data-ttu-id="2f8fc-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="2f8fc-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="2f8fc-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f8fc-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="2f8fc-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f8fc-126">Property</span></span>|<span data-ttu-id="2f8fc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2f8fc-127">Type</span></span>|<span data-ttu-id="2f8fc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f8fc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f8fc-129">ID</span><span class="sxs-lookup"><span data-stu-id="2f8fc-129">id</span></span>|<span data-ttu-id="2f8fc-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f8fc-130">String</span></span>|<span data-ttu-id="2f8fc-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2f8fc-131">Key of the entity.</span></span>|
|<span data-ttu-id="2f8fc-132">Ziel</span><span class="sxs-lookup"><span data-stu-id="2f8fc-132">target</span></span>|[<span data-ttu-id="2f8fc-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2f8fc-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2f8fc-134">Ziel der Zuweisung der Konformitätsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="2f8fc-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="2f8fc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f8fc-135">Response</span></span>
<span data-ttu-id="2f8fc-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f8fc-136">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f8fc-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f8fc-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f8fc-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f8fc-138">Request</span></span>
<span data-ttu-id="2f8fc-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f8fc-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2f8fc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f8fc-140">Response</span></span>
<span data-ttu-id="2f8fc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f8fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



