# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="d6b44-101">deviceAndAppManagementRoleDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="d6b44-101">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="d6b44-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6b44-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6b44-103">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6b44-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6b44-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d6b44-104">Prerequisites</span></span>
<span data-ttu-id="d6b44-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6b44-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6b44-107">Permission type</span></span>|<span data-ttu-id="d6b44-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6b44-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b44-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6b44-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d6b44-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b44-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d6b44-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6b44-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b44-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6b44-112">Not supported.</span></span>|
|<span data-ttu-id="d6b44-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6b44-113">Application</span></span>|<span data-ttu-id="d6b44-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6b44-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6b44-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6b44-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6b44-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d6b44-116">Optional query parameters</span></span>
<span data-ttu-id="d6b44-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d6b44-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d6b44-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6b44-118">Request headers</span></span>
|<span data-ttu-id="d6b44-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d6b44-119">Header</span></span>|<span data-ttu-id="d6b44-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d6b44-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6b44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b44-121">Authorization</span></span>|<span data-ttu-id="d6b44-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6b44-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6b44-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d6b44-123">Accept</span></span>|<span data-ttu-id="d6b44-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b44-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b44-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6b44-125">Request body</span></span>
<span data-ttu-id="d6b44-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d6b44-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6b44-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6b44-127">Response</span></span>
<span data-ttu-id="d6b44-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6b44-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b44-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6b44-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6b44-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6b44-130">Request</span></span>
<span data-ttu-id="d6b44-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6b44-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="d6b44-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6b44-132">Response</span></span>
<span data-ttu-id="d6b44-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6b44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
    "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
    "displayName": "Display Name value",
    "description": "Description value",
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "resourceActions": [
          {
            "@odata.type": "microsoft.graph.resourceAction",
            "allowedResourceActions": [
              "Allowed Resource Actions value"
            ],
            "notAllowedResourceActions": [
              "Not Allowed Resource Actions value"
            ]
          }
        ]
      }
    ],
    "isBuiltIn": true
  }
}
```



