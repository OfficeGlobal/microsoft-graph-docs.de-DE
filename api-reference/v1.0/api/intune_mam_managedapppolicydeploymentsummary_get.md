# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="72b23-101">Abrufen von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="72b23-101">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="72b23-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="72b23-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72b23-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="72b23-103">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72b23-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="72b23-104">Prerequisites</span></span>
<span data-ttu-id="72b23-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="72b23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72b23-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72b23-107">Permission type</span></span>|<span data-ttu-id="72b23-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72b23-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72b23-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72b23-109">Delegated (work or school account)</span></span>|<span data-ttu-id="72b23-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72b23-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72b23-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72b23-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72b23-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72b23-112">Not supported.</span></span>|
|<span data-ttu-id="72b23-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72b23-113">Application</span></span>|<span data-ttu-id="72b23-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72b23-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72b23-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72b23-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72b23-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="72b23-116">Optional query parameters</span></span>
<span data-ttu-id="72b23-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="72b23-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="72b23-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72b23-118">Request headers</span></span>
|<span data-ttu-id="72b23-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="72b23-119">Header</span></span>|<span data-ttu-id="72b23-120">Wert</span><span class="sxs-lookup"><span data-stu-id="72b23-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72b23-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="72b23-121">Authorization</span></span>|<span data-ttu-id="72b23-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="72b23-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72b23-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="72b23-123">Accept</span></span>|<span data-ttu-id="72b23-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="72b23-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72b23-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72b23-125">Request body</span></span>
<span data-ttu-id="72b23-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="72b23-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72b23-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="72b23-127">Response</span></span>
<span data-ttu-id="72b23-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="72b23-128">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72b23-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72b23-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="72b23-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72b23-130">Request</span></span>
<span data-ttu-id="72b23-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72b23-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="72b23-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="72b23-132">Response</span></span>
<span data-ttu-id="72b23-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72b23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
    "version": "Version value"
  }
}
```








