---
title: PrivilegedRoleAssignmentRequest Abbrechen
description: Abbrechen einer PrivilegedRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 2d717f0ca6fccc274b4ee80cda6b65f02f01abec
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577508"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="ae743-103">PrivilegedRoleAssignmentRequest Abbrechen</span><span class="sxs-lookup"><span data-stu-id="ae743-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae743-104">Abbrechen einer [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="ae743-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae743-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae743-105">Permissions</span></span>
<span data-ttu-id="ae743-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae743-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae743-108">Permission type</span></span>                        | <span data-ttu-id="ae743-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae743-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae743-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae743-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae743-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae743-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae743-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae743-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae743-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae743-113">Not supported.</span></span> |
|<span data-ttu-id="ae743-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae743-114">Application</span></span>                            | <span data-ttu-id="ae743-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae743-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="ae743-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae743-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="ae743-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae743-117">Request headers</span></span>
| <span data-ttu-id="ae743-118">Name</span><span class="sxs-lookup"><span data-stu-id="ae743-118">Name</span></span>      |<span data-ttu-id="ae743-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae743-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae743-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae743-120">Authorization</span></span>  | <span data-ttu-id="ae743-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae743-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae743-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae743-123">Request body</span></span>
<span data-ttu-id="ae743-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ae743-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae743-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae743-125">Response</span></span>
<span data-ttu-id="ae743-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 Ok` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae743-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="ae743-127">[PrivilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) zurückgegeben im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ae743-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="ae743-128">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="ae743-128">Error codes</span></span>
<span data-ttu-id="ae743-129">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="ae743-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="ae743-130">Darüber hinaus wird die benutzerdefinierte Fehlercodes in der folgenden Tabelle aufgeführten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae743-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="ae743-131">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="ae743-131">Error code</span></span>     | <span data-ttu-id="ae743-132">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="ae743-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="ae743-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae743-133">400 BadRequest</span></span> | <span data-ttu-id="ae743-134">RequestId darf nicht Null sein.</span><span class="sxs-lookup"><span data-stu-id="ae743-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="ae743-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae743-135">400 BadRequest</span></span> | <span data-ttu-id="ae743-136">Fordern Sie mit dem Anforderungs-ID wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="ae743-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="ae743-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae743-137">400 BadRequest</span></span> | <span data-ttu-id="ae743-138">Abbruch kann nur auf Status geplant und Ausstehende Genehmigung durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ae743-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="ae743-139">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="ae743-139">403 UnAuthorized</span></span> | <span data-ttu-id="ae743-140">Anfordernde Person nicht berechtigt, stellen Sie Abbrechen Anruf oder die Anforderung wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="ae743-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="ae743-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae743-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae743-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae743-142">Request</span></span>
<span data-ttu-id="ae743-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae743-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="ae743-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae743-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
