---
title: PrivilegedRoleAssignmentRequest Abbrechen
description: Abbrechen einer PrivilegedRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 0cca3f33e6e027c18e24862dc4736006058f8e41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528473"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="d6a0b-103">PrivilegedRoleAssignmentRequest Abbrechen</span><span class="sxs-lookup"><span data-stu-id="d6a0b-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6a0b-104">Abbrechen einer [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="d6a0b-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6a0b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d6a0b-105">Permissions</span></span>
<span data-ttu-id="d6a0b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6a0b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6a0b-108">Permission type</span></span>                        | <span data-ttu-id="d6a0b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6a0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6a0b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6a0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6a0b-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6a0b-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6a0b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6a0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6a0b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6a0b-113">Not supported.</span></span> |
|<span data-ttu-id="d6a0b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6a0b-114">Application</span></span>                            | <span data-ttu-id="d6a0b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6a0b-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="d6a0b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6a0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="d6a0b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6a0b-117">Request headers</span></span>
| <span data-ttu-id="d6a0b-118">Name</span><span class="sxs-lookup"><span data-stu-id="d6a0b-118">Name</span></span>      |<span data-ttu-id="d6a0b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6a0b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6a0b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6a0b-120">Authorization</span></span>  | <span data-ttu-id="d6a0b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6a0b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6a0b-123">Request body</span></span>
<span data-ttu-id="d6a0b-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6a0b-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6a0b-125">Response</span></span>
<span data-ttu-id="d6a0b-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 Ok` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="d6a0b-127">Es gibt [PrivilegedRoleAssignmentRequest] (... / resources/privilegedRoleAssignmentRequest.md) in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-127">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="d6a0b-128">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="d6a0b-128">Error codes</span></span>
<span data-ttu-id="d6a0b-129">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="d6a0b-130">Darüber hinaus wird die benutzerdefinierte Fehlercodes in der folgenden Tabelle aufgeführten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="d6a0b-131">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="d6a0b-131">Error code</span></span>     | <span data-ttu-id="d6a0b-132">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="d6a0b-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="d6a0b-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d6a0b-133">400 BadRequest</span></span> | <span data-ttu-id="d6a0b-134">RequestId darf nicht Null sein.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="d6a0b-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d6a0b-135">400 BadRequest</span></span> | <span data-ttu-id="d6a0b-136">Fordern Sie mit dem Anforderungs-ID wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="d6a0b-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d6a0b-137">400 BadRequest</span></span> | <span data-ttu-id="d6a0b-138">Abbruch kann nur auf Status geplant und Ausstehende Genehmigung durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="d6a0b-139">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="d6a0b-139">403 UnAuthorized</span></span> | <span data-ttu-id="d6a0b-140">Anfordernde Person nicht berechtigt, stellen Sie Abbrechen Anruf oder die Anforderung wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="d6a0b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6a0b-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6a0b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6a0b-142">Request</span></span>
<span data-ttu-id="d6a0b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6a0b-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="d6a0b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6a0b-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequests"
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
    "userId": "Self"，
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
