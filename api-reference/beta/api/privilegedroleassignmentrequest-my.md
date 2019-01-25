---
title: 'PrivilegedRoleAssignmentRequest: Meine'
description: Abrufen der anfordernden Person privilegierten Role Assignment Anforderungen.
localization_priority: Normal
ms.openlocfilehash: 79545b5ea0ad88c55d7a09eb5c77982e812721eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508867"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="5a120-103">PrivilegedRoleAssignmentRequest: Meine</span><span class="sxs-lookup"><span data-stu-id="5a120-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a120-104">Abrufen der anfordernden Person privilegierten Role Assignment Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="5a120-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a120-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a120-105">Permissions</span></span>
<span data-ttu-id="5a120-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a120-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a120-108">Permission type</span></span>                        | <span data-ttu-id="5a120-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a120-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a120-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a120-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a120-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a120-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a120-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a120-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a120-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a120-113">Not supported.</span></span> |
|<span data-ttu-id="5a120-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a120-114">Application</span></span>                            | <span data-ttu-id="5a120-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a120-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a120-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a120-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a120-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5a120-117">Optional query parameters</span></span>
<span data-ttu-id="5a120-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a120-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a120-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a120-119">Request headers</span></span>
| <span data-ttu-id="5a120-120">Name</span><span class="sxs-lookup"><span data-stu-id="5a120-120">Name</span></span>      |<span data-ttu-id="5a120-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a120-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a120-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a120-122">Authorization</span></span>  | <span data-ttu-id="5a120-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a120-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a120-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a120-125">Request body</span></span>
<span data-ttu-id="5a120-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5a120-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a120-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a120-127">Response</span></span>
<span data-ttu-id="5a120-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5a120-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a120-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a120-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a120-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a120-130">Request</span></span>
<span data-ttu-id="5a120-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a120-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="5a120-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a120-132">Response</span></span>
<span data-ttu-id="5a120-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a120-133">The following is an example of the response.</span></span> <span data-ttu-id="5a120-134">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="5a120-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5a120-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a120-135">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
    "@odata.count": 4,
    "value": [{
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-08T02:35:17.903Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
         "userId": "Self"，
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
        "status": "RequestedApproval",
        "duration": "2",
        "reason": "Activate the role for business purpose",
        "ticketNumber": "234",
        "ticketSystem": "system",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }, {
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-07T22:55:00Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "03ea0c3d-90a0-42d4-b220-11c049c506fb",
        "userId": "Self"，
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-07T22:17:37.2215343Z",
        "status": "ApprovalAborted",
        "duration": "1",
        "reason": "Activate for testing",
        "ticketNumber": "222",
        "ticketSystem": "222",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('03ea0c3d-90a0-42d4-b220-11c049c506fb')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-my.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
