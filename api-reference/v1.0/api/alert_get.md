# <a name="get-alert"></a><span data-ttu-id="9812a-101">Warnung abrufen</span><span class="sxs-lookup"><span data-stu-id="9812a-101">Get alert</span></span>

 <span data-ttu-id="9812a-102">Rufen Sie die Eigenschaften und die Beziehungen eines [alerts](../resources/alert.md)-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="9812a-102">Retrieve the properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9812a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9812a-103">Permissions</span></span>

<span data-ttu-id="9812a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9812a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9812a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9812a-106">Permission type</span></span>      | <span data-ttu-id="9812a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9812a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9812a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9812a-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9812a-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9812a-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="9812a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9812a-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9812a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9812a-111">Not supported.</span></span>  |
|<span data-ttu-id="9812a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9812a-112">Application</span></span> | <span data-ttu-id="9812a-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9812a-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9812a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9812a-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="9812a-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9812a-115">Request headers</span></span>

| <span data-ttu-id="9812a-116">Name</span><span class="sxs-lookup"><span data-stu-id="9812a-116">Name</span></span>      |<span data-ttu-id="9812a-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9812a-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9812a-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9812a-118">Authorization</span></span>  | <span data-ttu-id="9812a-p102">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9812a-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9812a-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9812a-121">Request body</span></span>

<span data-ttu-id="9812a-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9812a-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9812a-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="9812a-123">Response</span></span>

<span data-ttu-id="9812a-124">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein **alert**-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9812a-124">If successful, this method returns a `200 OK` response code and an updated **iosLobApp** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9812a-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9812a-125">Example</span></span>

### <a name="request"></a><span data-ttu-id="9812a-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9812a-126">Request</span></span>

<span data-ttu-id="9812a-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9812a-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="9812a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9812a-128">Response</span></span>

<span data-ttu-id="9812a-129">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9812a-129">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "destinationServiceIp": "String",
      "destinationServiceName": "String",
      "riskScore": "String"
    }
  ],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [
    {
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "name": "String",
      "path": "String",
      "riskScore": "String"
    }
  ],
  "hostStates": [
    {
      "fqdn": "String",
      "isAzureAadJoined": true,
      "isAzureAadRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "String",
      "os": "String",
      "privateIpAddress": "String",
      "publicIpAddress": "String",
      "riskScore": "String"
    }
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "category": "String",
      "family": "String",
      "name": "String",
      "severity": "String",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "applicationName": "String",
      "destinationAddress": "String",
      "destinationDomain": "String",
      "destinationPort": "String",
      "destinationUrl": "String",
      "direction": "@odata.type: microsoft.graph.connectionDirection",
      "domainRegisteredDateTime": "String (timestamp)",
      "localDnsName": "String",
      "natDestinationAddress": "String",
      "natDestinationPort": "String",
      "natSourceAddress": "String",
      "natSourcePort": "String",
      "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
      "riskScore": "String",
      "sourceAddress": "String",
      "sourcePort": "String",
      "status": "@odata.type: microsoft.graph.connectionStatus",
      "urlParameters": "String"
    }
  ],
  "processes": [
    {
      "accountName": "String",
      "commandLine": "String",
      "createdDateTime": "String (timestamp)",
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
      "isElevated": true,
      "name": "String",
      "parentProcessCreatedDateTime": "String (timestamp)",
      "parentProcessId": 1024,
      "parentProcessName": "String",
      "path": "String",
      "processId": 1024
    }
  ],
  "recommendedActions": ["String"],
  "registryKeyStates": [
    {
      "hive": "@odata.type: microsoft.graph.registryHive",
      "key": "String",
      "oldKey": "String",
      "oldValueData": "String",
      "oldValueName": "String",
      "operation": "@odata.type: microsoft.graph.registryOperation",
      "processId": 1024,
      "valueData": "String",
      "valueName": "String",
      "valueType": "@odata.type: microsoft.graph.registryValueType"
    }
  ],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [
    {
      "name": "String",
      "type": "String",
      "value": "String"
    }
  ],
  "userStates": [
    {
      "aadUserId": "String",
      "accountName": "String",
      "domainName": "String",
      "emailRole": "@odata.type: microsoft.graph.emailRole",
      "isVpn": true,
      "logonDateTime": "String (timestamp)",
      "logonId": "String",
      "logonIp": "String",
      "logonLocation": "String",
      "logonType": "@odata.type: microsoft.graph.logonType",
      "onPremisesSecurityIdentifier": "String",
      "riskScore": "String",
      "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
      "userPrincipalName": "String"
    }
  ],
  "vendorInformation": {
    "provider": "String",
    "providerVersion": "String",
    "subProvider": "String",
    "vendor": "String"
  },
  "vulnerabilityStates": [
    {
      "cve": "String",
      "severity": "String",
      "wasRunning": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
