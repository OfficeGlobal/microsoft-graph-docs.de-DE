---
title: Abrufen von governanceRoleAssignmentRequest
description: 'Rufen Sie eine GovernanceRoleAssignmentRequest. '
ms.openlocfilehash: 4dca14c081edc9cd3609bd4eab1c79a10953e433
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062719"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="67aea-103">Abrufen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="67aea-103">Get governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="67aea-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67aea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67aea-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67aea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67aea-106">Rufen Sie eine [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="67aea-106">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="67aea-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67aea-107">Permissions</span></span>
<span data-ttu-id="67aea-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67aea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67aea-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67aea-110">Permission type</span></span>      | <span data-ttu-id="67aea-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67aea-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67aea-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67aea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="67aea-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="67aea-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="67aea-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67aea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67aea-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67aea-115">Not supported.</span></span>    |
|<span data-ttu-id="67aea-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67aea-116">Application</span></span> | <span data-ttu-id="67aea-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="67aea-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="67aea-118">Neben den Berechtigungsbereich benötigt den requestor</span><span class="sxs-lookup"><span data-stu-id="67aea-118">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="67aea-119">mindestens eine rollenzuweisung für die Ressource verfügen; oder</span><span class="sxs-lookup"><span data-stu-id="67aea-119">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="67aea-120">der Betreff der [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)ist.</span><span class="sxs-lookup"><span data-stu-id="67aea-120">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="67aea-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67aea-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67aea-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="67aea-122">Optional query parameters</span></span>
<span data-ttu-id="67aea-123">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="67aea-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67aea-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67aea-124">Request headers</span></span>
| <span data-ttu-id="67aea-125">Name</span><span class="sxs-lookup"><span data-stu-id="67aea-125">Name</span></span>      |<span data-ttu-id="67aea-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67aea-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67aea-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="67aea-127">Authorization</span></span>  | <span data-ttu-id="67aea-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="67aea-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="67aea-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67aea-129">Request body</span></span>
<span data-ttu-id="67aea-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="67aea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67aea-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="67aea-131">Response</span></span>
<span data-ttu-id="67aea-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="67aea-132">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67aea-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67aea-133">Example</span></span>
<span data-ttu-id="67aea-134">GET-Anforderung einer Rolle-Zuordnung</span><span class="sxs-lookup"><span data-stu-id="67aea-134">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="67aea-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67aea-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="67aea-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="67aea-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->