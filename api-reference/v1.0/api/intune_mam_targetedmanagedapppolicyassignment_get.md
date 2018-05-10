# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="58357-101">Abrufen von „targetedManagedAppPolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="58357-101">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="58357-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58357-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58357-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="58357-103">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58357-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58357-104">Prerequisites</span></span>
<span data-ttu-id="58357-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58357-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58357-107">Permission type</span></span>|<span data-ttu-id="58357-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58357-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58357-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58357-109">Delegated (work or school account)</span></span>|<span data-ttu-id="58357-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58357-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="58357-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58357-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58357-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58357-112">Not supported.</span></span>|
|<span data-ttu-id="58357-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58357-113">Application</span></span>|<span data-ttu-id="58357-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58357-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58357-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58357-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58357-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="58357-116">Optional query parameters</span></span>
<span data-ttu-id="58357-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="58357-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="58357-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58357-118">Request headers</span></span>
|<span data-ttu-id="58357-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58357-119">Header</span></span>|<span data-ttu-id="58357-120">Wert</span><span class="sxs-lookup"><span data-stu-id="58357-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58357-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58357-121">Authorization</span></span>|<span data-ttu-id="58357-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58357-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58357-123">Accept</span><span class="sxs-lookup"><span data-stu-id="58357-123">Accept</span></span>|<span data-ttu-id="58357-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58357-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58357-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58357-125">Request body</span></span>
<span data-ttu-id="58357-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="58357-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58357-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="58357-127">Response</span></span>
<span data-ttu-id="58357-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58357-128">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58357-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58357-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="58357-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58357-130">Request</span></span>
<span data-ttu-id="58357-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58357-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="58357-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="58357-132">Response</span></span>
<span data-ttu-id="58357-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58357-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



