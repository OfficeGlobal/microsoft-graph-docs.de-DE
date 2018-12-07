---
title: Liste governanceRoleAssignments
description: Eine Auflistung der GovernanceRoleAssignments abzurufen.
ms.openlocfilehash: 0f4680c8998191fa07af993e8ee3712557b7010d
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191067"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="6924d-103">Liste governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="6924d-103">List governanceRoleAssignments</span></span>

> <span data-ttu-id="6924d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6924d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6924d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6924d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6924d-106">Eine Auflistung der [GovernanceRoleAssignments](../resources/governanceroleassignment.md)abzurufen.</span><span class="sxs-lookup"><span data-stu-id="6924d-106">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6924d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6924d-107">Permissions</span></span>
<span data-ttu-id="6924d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6924d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6924d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6924d-110">Permission type</span></span>      | <span data-ttu-id="6924d-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6924d-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6924d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6924d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6924d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6924d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6924d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6924d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6924d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6924d-115">Not supported.</span></span>    |
|<span data-ttu-id="6924d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6924d-116">Application</span></span> | <span data-ttu-id="6924d-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6924d-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="6924d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6924d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6924d-119">Eine Auflistung von [GovernanceRoleAssignments](../resources/governanceroleassignment.md) für eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="6924d-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="6924d-120">**Hinweis:** Neben den Berechtigungsbereich erfordert dieser Anforderung den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="6924d-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="6924d-121">Eine Auflistung von [GovernanceRoleAssignments](../resources/governanceroleassignment.md) Meine aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="6924d-121">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6924d-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6924d-122">Optional query parameters</span></span>
<span data-ttu-id="6924d-123">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6924d-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6924d-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6924d-124">Request headers</span></span>
| <span data-ttu-id="6924d-125">Name</span><span class="sxs-lookup"><span data-stu-id="6924d-125">Name</span></span>      |<span data-ttu-id="6924d-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6924d-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6924d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6924d-127">Authorization</span></span>  | <span data-ttu-id="6924d-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6924d-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6924d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6924d-129">Request body</span></span>
<span data-ttu-id="6924d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6924d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6924d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6924d-131">Response</span></span>
<span data-ttu-id="6924d-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [GovernanceRoleAssignment](../resources/governanceroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6924d-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6924d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6924d-133">Example</span></span>

<span data-ttu-id="6924d-134">In diesem Beispiel wird gezeigt, wie meine rollenzuweisungen für das Abonnement Wingtip Toys - "Bemerkungen" abgerufen.</span><span class="sxs-lookup"><span data-stu-id="6924d-134">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="6924d-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6924d-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="6924d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6924d-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        ...
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
