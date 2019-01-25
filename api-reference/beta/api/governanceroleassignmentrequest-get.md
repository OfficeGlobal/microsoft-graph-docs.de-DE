---
title: Abrufen von governanceRoleAssignmentRequest
description: 'Rufen Sie eine GovernanceRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 6914dbe8c45bcc05bc684b08fb5fdf87405a045a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524135"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="8dac3-103">Abrufen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8dac3-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dac3-104">Rufen Sie eine [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="8dac3-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8dac3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8dac3-105">Permissions</span></span>
<span data-ttu-id="8dac3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dac3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dac3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8dac3-108">Permission type</span></span>      | <span data-ttu-id="8dac3-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8dac3-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dac3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8dac3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8dac3-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8dac3-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8dac3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8dac3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dac3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8dac3-113">Not supported.</span></span>    |
|<span data-ttu-id="8dac3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8dac3-114">Application</span></span> | <span data-ttu-id="8dac3-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8dac3-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="8dac3-116">Neben den Berechtigungsbereich benötigt den requestor</span><span class="sxs-lookup"><span data-stu-id="8dac3-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="8dac3-117">mindestens eine rollenzuweisung für die Ressource verfügen; oder</span><span class="sxs-lookup"><span data-stu-id="8dac3-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="8dac3-118">der Betreff der [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)ist.</span><span class="sxs-lookup"><span data-stu-id="8dac3-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="8dac3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8dac3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8dac3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8dac3-120">Optional query parameters</span></span>
<span data-ttu-id="8dac3-121">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8dac3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dac3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8dac3-122">Request headers</span></span>
| <span data-ttu-id="8dac3-123">Name</span><span class="sxs-lookup"><span data-stu-id="8dac3-123">Name</span></span>      |<span data-ttu-id="8dac3-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dac3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8dac3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dac3-125">Authorization</span></span>  | <span data-ttu-id="8dac3-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8dac3-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dac3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8dac3-127">Request body</span></span>
<span data-ttu-id="8dac3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8dac3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dac3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8dac3-129">Response</span></span>
<span data-ttu-id="8dac3-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8dac3-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dac3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8dac3-131">Example</span></span>
<span data-ttu-id="8dac3-132">GET-Anforderung einer Rolle-Zuordnung</span><span class="sxs-lookup"><span data-stu-id="8dac3-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="8dac3-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8dac3-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="8dac3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8dac3-134">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
