---
title: Warnung erhalten
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: a3c8acb8ab748636d7a79b7ce3995a61699f7946
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059355"
---
# <a name="get-alert"></a><span data-ttu-id="dcbb7-104">Warnung erhalten</span><span class="sxs-lookup"><span data-stu-id="dcbb7-104">Get alert</span></span>

 > <span data-ttu-id="dcbb7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcbb7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcbb7-107">Rufen Sie die Eigenschaften und die Beziehungen eines [Benachrichtigung](../resources/alert.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-107">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcbb7-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dcbb7-108">Permissions</span></span>

<span data-ttu-id="dcbb7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcbb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcbb7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dcbb7-111">Permission type</span></span>      | <span data-ttu-id="dcbb7-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dcbb7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcbb7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dcbb7-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="dcbb7-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcbb7-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="dcbb7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dcbb7-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dcbb7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcbb7-116">Not supported.</span></span>  |
|<span data-ttu-id="dcbb7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dcbb7-117">Application</span></span> | <span data-ttu-id="dcbb7-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcbb7-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcbb7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcbb7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dcbb7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dcbb7-120">Request headers</span></span>

| <span data-ttu-id="dcbb7-121">Name</span><span class="sxs-lookup"><span data-stu-id="dcbb7-121">Name</span></span>      |<span data-ttu-id="dcbb7-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcbb7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcbb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcbb7-123">Authorization</span></span>  | <span data-ttu-id="dcbb7-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcbb7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dcbb7-126">Request body</span></span>

<span data-ttu-id="dcbb7-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcbb7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcbb7-128">Response</span></span>

<span data-ttu-id="dcbb7-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine **Warnung** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-129">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="dcbb7-130">Wenn ein Statuscode als 2xx oder 404 von einem Anbieter zurückgegeben wird, oder wenn von ein Anbieter Zeitlimit überschritten, die Antwort werden eine `206 Partial Content` Statuscode mit der Antwort Anbieter in der Kopfzeile einer Warnung.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-130">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="dcbb7-131">Weitere Informationen finden Sie unter [Microsoft Graph Security-API-Fehlerantworten](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="dcbb7-131">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="dcbb7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dcbb7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcbb7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcbb7-133">Request</span></span>

<span data-ttu-id="dcbb7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="dcbb7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcbb7-135">Response</span></span>

<span data-ttu-id="dcbb7-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dcbb7-136">The following is an example of the response.</span></span>
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
