---
title: GovernanceRoleAssignmentRequests aktualisieren
description: So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf GovernanceRoleAssignmentRequests, die in den Status der sind `PendingAdminDecision`.
ms.openlocfilehash: bd924acd8ddd3a79ad1fb97ac5f9bdc9baba17dd
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191151"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="21ed2-103">GovernanceRoleAssignmentRequests aktualisieren</span><span class="sxs-lookup"><span data-stu-id="21ed2-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="21ed2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21ed2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21ed2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21ed2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21ed2-106">So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="21ed2-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="21ed2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="21ed2-107">Permissions</span></span>
<span data-ttu-id="21ed2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21ed2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="21ed2-110">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource, die die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="21ed2-110">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="21ed2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21ed2-111">Permission type</span></span>      | <span data-ttu-id="21ed2-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="21ed2-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21ed2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21ed2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="21ed2-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="21ed2-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="21ed2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21ed2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21ed2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21ed2-116">Not supported.</span></span>    |
|<span data-ttu-id="21ed2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21ed2-117">Application</span></span> | <span data-ttu-id="21ed2-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="21ed2-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="21ed2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21ed2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="21ed2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21ed2-120">Request headers</span></span>
| <span data-ttu-id="21ed2-121">Name</span><span class="sxs-lookup"><span data-stu-id="21ed2-121">Name</span></span>           | <span data-ttu-id="21ed2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21ed2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="21ed2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21ed2-123">Authorization</span></span>  | <span data-ttu-id="21ed2-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="21ed2-124">Bearer {code}</span></span>|
| <span data-ttu-id="21ed2-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="21ed2-125">Content-type</span></span>  | <span data-ttu-id="21ed2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21ed2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21ed2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21ed2-127">Request body</span></span>

|<span data-ttu-id="21ed2-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="21ed2-128">Parameters</span></span>      |<span data-ttu-id="21ed2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="21ed2-129">Type</span></span>                   |<span data-ttu-id="21ed2-130">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="21ed2-130">Required</span></span> |<span data-ttu-id="21ed2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21ed2-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="21ed2-132">Grund</span><span class="sxs-lookup"><span data-stu-id="21ed2-132">reason</span></span>        |<span data-ttu-id="21ed2-133">String</span><span class="sxs-lookup"><span data-stu-id="21ed2-133">String</span></span>                 |<span data-ttu-id="21ed2-134">✓</span><span class="sxs-lookup"><span data-stu-id="21ed2-134">✓</span></span>        |<span data-ttu-id="21ed2-135">Der Grund für seine Entscheidung vom Administrator bereitgestellten.</span><span class="sxs-lookup"><span data-stu-id="21ed2-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="21ed2-136">Entscheidung</span><span class="sxs-lookup"><span data-stu-id="21ed2-136">decision</span></span>        |<span data-ttu-id="21ed2-137">String</span><span class="sxs-lookup"><span data-stu-id="21ed2-137">String</span></span>                 |<span data-ttu-id="21ed2-138">✓</span><span class="sxs-lookup"><span data-stu-id="21ed2-138">✓</span></span>        |<span data-ttu-id="21ed2-139">Die Entscheidung Administrator der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21ed2-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="21ed2-140">Der Wert aktualisiert werden sollen, als `AdminApproved` oder `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="21ed2-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="21ed2-141">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="21ed2-141">schedule</span></span>      |[<span data-ttu-id="21ed2-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="21ed2-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="21ed2-143">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21ed2-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="21ed2-144">Status der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21ed2-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="21ed2-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="21ed2-145">assignmentState</span></span>      |<span data-ttu-id="21ed2-146">String</span><span class="sxs-lookup"><span data-stu-id="21ed2-146">String</span></span>|         | <span data-ttu-id="21ed2-147">Der Status der Aufgabe und die Werte sind möglich `Eligible` oder `Active`.</span><span class="sxs-lookup"><span data-stu-id="21ed2-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="21ed2-148">Für die Entscheidung der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21ed2-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="21ed2-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="21ed2-149">Response</span></span>
<span data-ttu-id="21ed2-150">Diese Methode kann nur angewendet werden, auf Anfragen, die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="21ed2-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="21ed2-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21ed2-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21ed2-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21ed2-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21ed2-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21ed2-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="21ed2-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21ed2-155">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="21ed2-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="21ed2-156">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
