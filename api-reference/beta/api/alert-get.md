---
title: Warnung erhalten
description: Abrufen der Eigenschaften und Beziehungen eines Alert-Objekts
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 2aea4388ef29978606a7bc09813c7cd92f977ed5
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364598"
---
# <a name="get-alert"></a><span data-ttu-id="8803a-103">Warnung erhalten</span><span class="sxs-lookup"><span data-stu-id="8803a-103">Get alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8803a-104">Ruft die Eigenschaften und Beziehungen eines [Alert](../resources/alert.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="8803a-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8803a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8803a-105">Permissions</span></span>

<span data-ttu-id="8803a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8803a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8803a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8803a-108">Permission type</span></span>      | <span data-ttu-id="8803a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8803a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8803a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8803a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8803a-111">Bereich securityevents. Read. all, Bereich securityevents. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="8803a-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="8803a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8803a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8803a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8803a-113">Not supported.</span></span>  |
|<span data-ttu-id="8803a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8803a-114">Application</span></span> | <span data-ttu-id="8803a-115">Bereich securityevents. Read. all, Bereich securityevents. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="8803a-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8803a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8803a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8803a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8803a-117">Request headers</span></span>

| <span data-ttu-id="8803a-118">Name</span><span class="sxs-lookup"><span data-stu-id="8803a-118">Name</span></span>      |<span data-ttu-id="8803a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8803a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8803a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8803a-120">Authorization</span></span>  | <span data-ttu-id="8803a-p102">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8803a-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8803a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8803a-123">Request body</span></span>

<span data-ttu-id="8803a-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8803a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8803a-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8803a-125">Response</span></span>

<span data-ttu-id="8803a-126">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **Alert** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8803a-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="8803a-127">Wenn ein anderer Statuscode als 2xx oder 404 von einem Anbieter zurückgegeben wird oder ein Timeout für einen Anbieter vorliegt, ist die `206 Partial Content` Antwort ein Statuscode mit der Antwort des Anbieters in einem Warnungs Header.</span><span class="sxs-lookup"><span data-stu-id="8803a-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="8803a-128">Weitere Informationen finden Sie unter [Microsoft Graph Security API Error Response](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="8803a-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="8803a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8803a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8803a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8803a-130">Request</span></span>

<span data-ttu-id="8803a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8803a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="8803a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8803a-132">Response</span></span>

<span data-ttu-id="8803a-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8803a-133">The following is an example of the response.</span></span>
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
  "historyStates": [
    {
      "appId": "appId-value",
      "assignedTo": "assignedTo-value",
      "comments": [
        "comments-value"
      ],
      "feedback": "feedback-value",
      "status": "status-value",
      "updatedDateTime": "datetime-value",
      "user": "user-value"
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
<!--
{
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
