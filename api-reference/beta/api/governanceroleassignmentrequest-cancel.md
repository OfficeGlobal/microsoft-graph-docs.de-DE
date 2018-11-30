---
title: GovernanceRoleAssignmentRequest Abbrechen
description: Abbrechen einer GovernanceRoleAssignmentRequest.
ms.openlocfilehash: 3e83d47b94f69b124b841f99490a012f2e39a42c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060898"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="f3db8-103">GovernanceRoleAssignmentRequest Abbrechen</span><span class="sxs-lookup"><span data-stu-id="f3db8-103">Cancel governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="f3db8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3db8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3db8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3db8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3db8-106">Abbrechen einer [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f3db8-106">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3db8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f3db8-107">Permissions</span></span>
<span data-ttu-id="f3db8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3db8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3db8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3db8-110">Permission type</span></span>      | <span data-ttu-id="f3db8-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f3db8-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3db8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3db8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3db8-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f3db8-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f3db8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3db8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3db8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3db8-115">Not supported.</span></span>    |
|<span data-ttu-id="f3db8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3db8-116">Application</span></span> | <span data-ttu-id="f3db8-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f3db8-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f3db8-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f3db8-118">Optional query parameters</span></span>
<span data-ttu-id="f3db8-119">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f3db8-119">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="f3db8-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3db8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="f3db8-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3db8-121">Request headers</span></span>
| <span data-ttu-id="f3db8-122">Name</span><span class="sxs-lookup"><span data-stu-id="f3db8-122">Name</span></span>       | <span data-ttu-id="f3db8-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3db8-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3db8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3db8-124">Authorization</span></span>  | <span data-ttu-id="f3db8-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f3db8-125">Bearer {code}</span></span>|
| <span data-ttu-id="f3db8-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f3db8-126">Content-type</span></span>  | <span data-ttu-id="f3db8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f3db8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3db8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3db8-128">Request body</span></span>
<span data-ttu-id="f3db8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3db8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3db8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3db8-130">Response</span></span>
<span data-ttu-id="f3db8-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3db8-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="f3db8-133">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="f3db8-133">Error codes</span></span>
<span data-ttu-id="f3db8-134">Diese API folgt dem Standard-HTTP-Codes.</span><span class="sxs-lookup"><span data-stu-id="f3db8-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="f3db8-135">Außerdem werden die benutzerdefinierten Fehlercodes unten angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f3db8-135">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="f3db8-136">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="f3db8-136">Error code</span></span>     | <span data-ttu-id="f3db8-137">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="f3db8-137">Error message</span></span>              | <span data-ttu-id="f3db8-138">Details</span><span class="sxs-lookup"><span data-stu-id="f3db8-138">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="f3db8-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f3db8-139">400 BadRequest</span></span> | <span data-ttu-id="f3db8-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="f3db8-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="f3db8-141">Die GovernanceRoleAssignmentRequest ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="f3db8-141">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="f3db8-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f3db8-142">400 BadRequest</span></span> | <span data-ttu-id="f3db8-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="f3db8-143">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="f3db8-144">Fordert nur in den Status der `Granted`, `PendingApproval`, `PendingApprovalProvisioning` und `PendingAdminDecision` abgebrochen werden kann.</span><span class="sxs-lookup"><span data-stu-id="f3db8-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="f3db8-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3db8-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3db8-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3db8-146">Request</span></span>
<span data-ttu-id="f3db8-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3db8-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="f3db8-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3db8-148">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->