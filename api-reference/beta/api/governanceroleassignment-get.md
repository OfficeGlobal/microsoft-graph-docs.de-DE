---
title: Abrufen von governanceRoleAssignment
description: Abrufen der Eigenschaften und Beziehungen zwischen einer GovernanceRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 838c096ccb8b719d9a07741aa80f3e132071a0c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887570"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="d7552-103">Abrufen von governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d7552-103">Get governanceRoleAssignment</span></span>

> <span data-ttu-id="d7552-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d7552-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7552-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7552-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7552-106">Abrufen der Eigenschaften und Beziehungen zwischen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d7552-106">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7552-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7552-107">Permissions</span></span>
<span data-ttu-id="d7552-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7552-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7552-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7552-110">Permission type</span></span>      | <span data-ttu-id="d7552-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7552-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7552-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7552-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7552-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d7552-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d7552-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7552-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7552-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7552-115">Not supported.</span></span>    |
|<span data-ttu-id="d7552-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7552-116">Application</span></span> | <span data-ttu-id="d7552-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d7552-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7552-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7552-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="d7552-119">Abrufen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md) auf eine Ressource</span><span class="sxs-lookup"><span data-stu-id="d7552-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="d7552-120">*Hinweis: Neben den Berechtigungsbereich benötigt den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.*</span><span class="sxs-lookup"><span data-stu-id="d7552-120">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="d7552-121">Abrufen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md) davon.</span><span class="sxs-lookup"><span data-stu-id="d7552-121">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7552-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d7552-122">Optional query parameters</span></span>
<span data-ttu-id="d7552-123">Diese Methode unterstützt [OData-Abfrage-Parameter](/graph/query-parameters) **nicht** als `$filter` helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="d7552-123">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7552-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7552-124">Request headers</span></span>
| <span data-ttu-id="d7552-125">Name</span><span class="sxs-lookup"><span data-stu-id="d7552-125">Name</span></span>      |<span data-ttu-id="d7552-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7552-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7552-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7552-127">Authorization</span></span>  | <span data-ttu-id="d7552-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d7552-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7552-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7552-129">Request body</span></span>
<span data-ttu-id="d7552-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7552-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d7552-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7552-131">Response</span></span>
<span data-ttu-id="d7552-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d7552-132">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7552-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7552-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="d7552-134">Abrufen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md) Abonnement "Wingtip Toys –" Bemerkungen ""</span><span class="sxs-lookup"><span data-stu-id="d7552-134">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="d7552-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7552-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="d7552-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7552-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
