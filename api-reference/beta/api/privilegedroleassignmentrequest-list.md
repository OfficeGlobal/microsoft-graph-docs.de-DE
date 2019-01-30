---
title: Liste privilegedRoleAssignmentRequests
description: 'Eine Auflistung der PrivilegedRoleAssignmentRequest abzurufen. '
localization_priority: Normal
ms.openlocfilehash: 06a6c66bcb566df0b6db5193bd753832bd9235a3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640728"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="3fe65-103">Liste privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="3fe65-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fe65-104">Eine Auflistung der [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)abzurufen.</span><span class="sxs-lookup"><span data-stu-id="3fe65-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="3fe65-105">**Hinweis:** Dieser anfordernden Person muss mindestens eine rollenzuweisung für die Ressource verfügen.</span><span class="sxs-lookup"><span data-stu-id="3fe65-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fe65-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3fe65-106">Permissions</span></span>
<span data-ttu-id="3fe65-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fe65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fe65-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3fe65-109">Permission type</span></span>                        | <span data-ttu-id="3fe65-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3fe65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fe65-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3fe65-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fe65-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3fe65-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3fe65-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3fe65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fe65-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fe65-114">Not supported.</span></span> |
|<span data-ttu-id="3fe65-115">Application</span><span class="sxs-lookup"><span data-stu-id="3fe65-115">Application</span></span>                            | <span data-ttu-id="3fe65-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fe65-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fe65-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fe65-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fe65-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3fe65-118">Optional query parameters</span></span>
<span data-ttu-id="3fe65-119">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="3fe65-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fe65-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3fe65-120">Request headers</span></span>
| <span data-ttu-id="3fe65-121">Name</span><span class="sxs-lookup"><span data-stu-id="3fe65-121">Name</span></span>      |<span data-ttu-id="3fe65-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3fe65-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fe65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fe65-123">Authorization</span></span>  | <span data-ttu-id="3fe65-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3fe65-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fe65-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3fe65-126">Request body</span></span>
<span data-ttu-id="3fe65-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3fe65-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fe65-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fe65-128">Response</span></span>
<span data-ttu-id="3fe65-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3fe65-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe65-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3fe65-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fe65-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fe65-131">Request</span></span>
<span data-ttu-id="3fe65-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3fe65-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="3fe65-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fe65-133">Response</span></span>
<span data-ttu-id="3fe65-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3fe65-134">The following is an example of the response.</span></span> <span data-ttu-id="3fe65-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3fe65-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3fe65-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3fe65-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "@odata.context":"https://https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
  "value":[
    {
      "schedule":{
        "type":"activation","startDateTime":"2018-02-07T22:55:00Z","endDateTime":null,"duration" : null
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
