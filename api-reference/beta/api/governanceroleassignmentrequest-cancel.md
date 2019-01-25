---
title: GovernanceRoleAssignmentRequest Abbrechen
description: Abbrechen einer GovernanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 0437051a3d2550da8a8fe3e9984214ff7c885e3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521733"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="aec70-103">GovernanceRoleAssignmentRequest Abbrechen</span><span class="sxs-lookup"><span data-stu-id="aec70-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aec70-104">Abbrechen einer [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="aec70-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aec70-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aec70-105">Permissions</span></span>
<span data-ttu-id="aec70-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec70-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aec70-108">Permission type</span></span>      | <span data-ttu-id="aec70-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aec70-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aec70-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aec70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aec70-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="aec70-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="aec70-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aec70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec70-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aec70-113">Not supported.</span></span>    |
|<span data-ttu-id="aec70-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aec70-114">Application</span></span> | <span data-ttu-id="aec70-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="aec70-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="aec70-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aec70-116">Optional query parameters</span></span>
<span data-ttu-id="aec70-117">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aec70-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="aec70-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aec70-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="aec70-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aec70-119">Request headers</span></span>
| <span data-ttu-id="aec70-120">Name</span><span class="sxs-lookup"><span data-stu-id="aec70-120">Name</span></span>       | <span data-ttu-id="aec70-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aec70-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aec70-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aec70-122">Authorization</span></span>  | <span data-ttu-id="aec70-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="aec70-123">Bearer {code}</span></span>|
| <span data-ttu-id="aec70-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="aec70-124">Content-type</span></span>  | <span data-ttu-id="aec70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aec70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec70-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aec70-126">Request body</span></span>
<span data-ttu-id="aec70-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aec70-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aec70-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="aec70-128">Response</span></span>
<span data-ttu-id="aec70-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aec70-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="aec70-131">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="aec70-131">Error codes</span></span>
<span data-ttu-id="aec70-132">Diese API folgt dem Standard-HTTP-Codes.</span><span class="sxs-lookup"><span data-stu-id="aec70-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="aec70-133">Außerdem werden die benutzerdefinierten Fehlercodes unten angezeigt.</span><span class="sxs-lookup"><span data-stu-id="aec70-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="aec70-134">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="aec70-134">Error code</span></span>     | <span data-ttu-id="aec70-135">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="aec70-135">Error message</span></span>              | <span data-ttu-id="aec70-136">Details</span><span class="sxs-lookup"><span data-stu-id="aec70-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="aec70-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="aec70-137">400 BadRequest</span></span> | <span data-ttu-id="aec70-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="aec70-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="aec70-139">Die GovernanceRoleAssignmentRequest ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="aec70-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="aec70-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="aec70-140">400 BadRequest</span></span> | <span data-ttu-id="aec70-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="aec70-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="aec70-142">Fordert nur in den Status der `Granted`, `PendingApproval`, `PendingApprovalProvisioning` und `PendingAdminDecision` abgebrochen werden kann.</span><span class="sxs-lookup"><span data-stu-id="aec70-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="aec70-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aec70-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aec70-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aec70-144">Request</span></span>
<span data-ttu-id="aec70-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aec70-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="aec70-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="aec70-146">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
