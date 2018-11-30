---
title: 'PrivilegedRoleAssignmentRequest: Meine'
description: Abrufen der anfordernden Person privilegierten Role Assignment Anforderungen.
ms.openlocfilehash: a2e6ca655359594480e09127721813f73726e2e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064592"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="18767-103">PrivilegedRoleAssignmentRequest: Meine</span><span class="sxs-lookup"><span data-stu-id="18767-103">privilegedRoleAssignmentRequest: my</span></span>

> <span data-ttu-id="18767-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18767-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18767-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18767-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18767-106">Abrufen der anfordernden Person privilegierten Role Assignment Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="18767-106">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="18767-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18767-107">Permissions</span></span>
<span data-ttu-id="18767-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18767-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18767-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18767-110">Permission type</span></span>                        | <span data-ttu-id="18767-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18767-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="18767-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18767-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18767-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18767-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18767-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18767-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18767-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18767-115">Not supported.</span></span> |
|<span data-ttu-id="18767-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18767-116">Application</span></span>                            | <span data-ttu-id="18767-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18767-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18767-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18767-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18767-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="18767-119">Optional query parameters</span></span>
<span data-ttu-id="18767-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18767-120">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18767-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18767-121">Request headers</span></span>
| <span data-ttu-id="18767-122">Name</span><span class="sxs-lookup"><span data-stu-id="18767-122">Name</span></span>      |<span data-ttu-id="18767-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18767-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18767-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="18767-124">Authorization</span></span>  | <span data-ttu-id="18767-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18767-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18767-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18767-127">Request body</span></span>
<span data-ttu-id="18767-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18767-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18767-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="18767-129">Response</span></span>
<span data-ttu-id="18767-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="18767-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18767-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18767-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18767-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18767-132">Request</span></span>
<span data-ttu-id="18767-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18767-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="18767-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="18767-134">Response</span></span>
<span data-ttu-id="18767-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18767-135">The following is an example of the response.</span></span> <span data-ttu-id="18767-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="18767-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="18767-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18767-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
