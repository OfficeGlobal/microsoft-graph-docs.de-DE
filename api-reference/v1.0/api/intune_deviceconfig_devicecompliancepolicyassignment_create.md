# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="09eee-101">Erstellen von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="09eee-101">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="09eee-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="09eee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09eee-103">Diese Methode erstellt ein neues Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09eee-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09eee-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09eee-104">Prerequisites</span></span>
<span data-ttu-id="09eee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="09eee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="09eee-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09eee-107">Permission type</span></span>|<span data-ttu-id="09eee-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09eee-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09eee-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09eee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="09eee-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09eee-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09eee-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09eee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09eee-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09eee-112">Not supported.</span></span>|
|<span data-ttu-id="09eee-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09eee-113">Application</span></span>|<span data-ttu-id="09eee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09eee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09eee-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09eee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="09eee-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09eee-116">Request headers</span></span>
|<span data-ttu-id="09eee-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="09eee-117">Header</span></span>|<span data-ttu-id="09eee-118">Wert</span><span class="sxs-lookup"><span data-stu-id="09eee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09eee-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="09eee-119">Authorization</span></span>|<span data-ttu-id="09eee-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09eee-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09eee-121">Accept</span><span class="sxs-lookup"><span data-stu-id="09eee-121">Accept</span></span>|<span data-ttu-id="09eee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="09eee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09eee-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09eee-123">Request body</span></span>
<span data-ttu-id="09eee-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceCompliancePolicyAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="09eee-124">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="09eee-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceCompliancePolicyAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="09eee-125">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="09eee-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09eee-126">Property</span></span>|<span data-ttu-id="09eee-127">Typ</span><span class="sxs-lookup"><span data-stu-id="09eee-127">Type</span></span>|<span data-ttu-id="09eee-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09eee-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09eee-129">id</span><span class="sxs-lookup"><span data-stu-id="09eee-129">id</span></span>|<span data-ttu-id="09eee-130">String</span><span class="sxs-lookup"><span data-stu-id="09eee-130">String</span></span>|<span data-ttu-id="09eee-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="09eee-131">Key of the entity.</span></span>|
|<span data-ttu-id="09eee-132">target</span><span class="sxs-lookup"><span data-stu-id="09eee-132">target</span></span>|[<span data-ttu-id="09eee-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="09eee-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="09eee-134">Ziel der Zuweisung der Konformitätsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="09eee-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="09eee-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="09eee-135">Response</span></span>
<span data-ttu-id="09eee-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="09eee-136">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09eee-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09eee-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="09eee-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09eee-138">Request</span></span>
<span data-ttu-id="09eee-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09eee-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="09eee-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="09eee-140">Response</span></span>
<span data-ttu-id="09eee-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09eee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



