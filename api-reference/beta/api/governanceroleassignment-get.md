---
title: Abrufen von governanceRoleAssignment
description: Abrufen der Eigenschaften und Beziehungen zwischen einer GovernanceRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: f699e1b5332652b2b87f3972d2ae47b06894b2e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508839"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="13630-103">Abrufen von governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="13630-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13630-104">Abrufen der Eigenschaften und Beziehungen zwischen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13630-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13630-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13630-105">Permissions</span></span>
<span data-ttu-id="13630-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13630-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13630-108">Permission type</span></span>      | <span data-ttu-id="13630-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13630-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13630-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13630-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13630-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="13630-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="13630-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13630-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13630-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13630-113">Not supported.</span></span>    |
|<span data-ttu-id="13630-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13630-114">Application</span></span> | <span data-ttu-id="13630-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="13630-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="13630-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13630-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="13630-117">Abrufen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md) auf eine Ressource</span><span class="sxs-lookup"><span data-stu-id="13630-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="13630-118">*Hinweis: Neben den Berechtigungsbereich benötigt den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.*</span><span class="sxs-lookup"><span data-stu-id="13630-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="13630-119">Abrufen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md) davon.</span><span class="sxs-lookup"><span data-stu-id="13630-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13630-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="13630-120">Optional query parameters</span></span>
<span data-ttu-id="13630-121">Diese Methode unterstützt [OData-Abfrage-Parameter](/graph/query-parameters) **nicht** als `$filter` helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="13630-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13630-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13630-122">Request headers</span></span>
| <span data-ttu-id="13630-123">Name</span><span class="sxs-lookup"><span data-stu-id="13630-123">Name</span></span>      |<span data-ttu-id="13630-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13630-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13630-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="13630-125">Authorization</span></span>  | <span data-ttu-id="13630-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="13630-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="13630-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13630-127">Request body</span></span>
<span data-ttu-id="13630-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="13630-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13630-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="13630-129">Response</span></span>
<span data-ttu-id="13630-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="13630-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13630-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13630-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="13630-132">Abrufen einer [GovernanceRoleAssignment](../resources/governanceroleassignment.md) Abonnement "Wingtip Toys –" Bemerkungen ""</span><span class="sxs-lookup"><span data-stu-id="13630-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="13630-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13630-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="13630-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="13630-134">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
