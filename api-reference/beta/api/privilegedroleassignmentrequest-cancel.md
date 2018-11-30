---
title: PrivilegedRoleAssignmentRequest Abbrechen
description: Abbrechen einer PrivilegedRoleAssignmentRequest.
ms.openlocfilehash: 99c1102235e93ca365dcdd0e619bcceac9f396f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062869"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="6a921-103">PrivilegedRoleAssignmentRequest Abbrechen</span><span class="sxs-lookup"><span data-stu-id="6a921-103">Cancel privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="6a921-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a921-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a921-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a921-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a921-106">Abbrechen einer [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="6a921-106">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a921-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a921-107">Permissions</span></span>
<span data-ttu-id="6a921-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a921-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a921-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a921-110">Permission type</span></span>                        | <span data-ttu-id="6a921-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a921-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a921-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a921-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a921-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a921-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a921-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a921-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a921-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a921-115">Not supported.</span></span> |
|<span data-ttu-id="6a921-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a921-116">Application</span></span>                            | <span data-ttu-id="6a921-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a921-117">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="6a921-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a921-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="6a921-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a921-119">Request headers</span></span>
| <span data-ttu-id="6a921-120">Name</span><span class="sxs-lookup"><span data-stu-id="6a921-120">Name</span></span>      |<span data-ttu-id="6a921-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a921-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a921-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a921-122">Authorization</span></span>  | <span data-ttu-id="6a921-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a921-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a921-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a921-125">Request body</span></span>
<span data-ttu-id="6a921-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6a921-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a921-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a921-127">Response</span></span>
<span data-ttu-id="6a921-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 Ok` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a921-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="6a921-129">Es gibt [PrivilegedRoleAssignmentRequest] (... / resources/privilegedRoleAssignmentRequest.md) in den Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6a921-129">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="6a921-130">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="6a921-130">Error codes</span></span>
<span data-ttu-id="6a921-131">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="6a921-131">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="6a921-132">Darüber hinaus wird die benutzerdefinierte Fehlercodes in der folgenden Tabelle aufgeführten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a921-132">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="6a921-133">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="6a921-133">Error code</span></span>     | <span data-ttu-id="6a921-134">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="6a921-134">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="6a921-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="6a921-135">400 BadRequest</span></span> | <span data-ttu-id="6a921-136">RequestId darf nicht Null sein.</span><span class="sxs-lookup"><span data-stu-id="6a921-136">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="6a921-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="6a921-137">400 BadRequest</span></span> | <span data-ttu-id="6a921-138">Fordern Sie mit dem Anforderungs-ID wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="6a921-138">Request with request ID not found.</span></span> |
| <span data-ttu-id="6a921-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="6a921-139">400 BadRequest</span></span> | <span data-ttu-id="6a921-140">Abbruch kann nur auf Status geplant und Ausstehende Genehmigung durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="6a921-140">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="6a921-141">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="6a921-141">403 UnAuthorized</span></span> | <span data-ttu-id="6a921-142">Anfordernde Person nicht berechtigt, stellen Sie Abbrechen Anruf oder die Anforderung wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="6a921-142">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="6a921-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a921-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a921-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a921-144">Request</span></span>
<span data-ttu-id="6a921-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a921-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="6a921-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a921-146">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
