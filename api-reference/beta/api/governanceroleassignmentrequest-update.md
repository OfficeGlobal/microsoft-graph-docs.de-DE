---
title: GovernanceRoleAssignmentRequests aktualisieren
description: So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf GovernanceRoleAssignmentRequests, die in den Status der sind `PendingAdminDecision`.
ms.openlocfilehash: 0f52b810b861e18a679ae8aea4ffdf7fd2d67abd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065624"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="0d424-103">GovernanceRoleAssignmentRequests aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d424-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="0d424-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0d424-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d424-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d424-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d424-106">So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="0d424-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d424-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d424-107">Permissions</span></span>
<span data-ttu-id="0d424-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d424-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d424-110">Permission type</span></span>      | <span data-ttu-id="0d424-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d424-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d424-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d424-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d424-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0d424-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0d424-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d424-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d424-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d424-115">Not supported.</span></span>    |
|<span data-ttu-id="0d424-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d424-116">Application</span></span> | <span data-ttu-id="0d424-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0d424-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="0d424-118">Diese API erfordert neben der Berechtigungsbereich den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource, der die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="0d424-118">Besides the permission scope, this API requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource, which the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

## <a name="http-request"></a><span data-ttu-id="0d424-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d424-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

### <a name="request-headers"></a><span data-ttu-id="0d424-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d424-120">Request headers</span></span>
| <span data-ttu-id="0d424-121">Name</span><span class="sxs-lookup"><span data-stu-id="0d424-121">Name</span></span>           | <span data-ttu-id="0d424-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d424-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d424-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d424-123">Authorization</span></span>  | <span data-ttu-id="0d424-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0d424-124">Bearer {code}</span></span>|
| <span data-ttu-id="0d424-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="0d424-125">Content-type</span></span>  | <span data-ttu-id="0d424-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d424-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="0d424-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d424-127">Request body</span></span>
|<span data-ttu-id="0d424-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="0d424-128">Parameters</span></span>      |<span data-ttu-id="0d424-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0d424-129">Type</span></span>                   |<span data-ttu-id="0d424-130">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d424-130">Required</span></span> |<span data-ttu-id="0d424-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d424-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="0d424-132">Grund</span><span class="sxs-lookup"><span data-stu-id="0d424-132">reason</span></span>        |<span data-ttu-id="0d424-133">String</span><span class="sxs-lookup"><span data-stu-id="0d424-133">String</span></span>                 |<span data-ttu-id="0d424-134">✓</span><span class="sxs-lookup"><span data-stu-id="0d424-134">✓</span></span>        |<span data-ttu-id="0d424-135">Der Grund für seine Entscheidung vom Administrator bereitgestellten.</span><span class="sxs-lookup"><span data-stu-id="0d424-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="0d424-136">Entscheidung</span><span class="sxs-lookup"><span data-stu-id="0d424-136">decision</span></span>        |<span data-ttu-id="0d424-137">String</span><span class="sxs-lookup"><span data-stu-id="0d424-137">String</span></span>                 |<span data-ttu-id="0d424-138">✓</span><span class="sxs-lookup"><span data-stu-id="0d424-138">✓</span></span>        |<span data-ttu-id="0d424-139">Die Entscheidung Administrator der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d424-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="0d424-140">Der Wert aktualisiert werden sollen, als `AdminApproved` oder `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="0d424-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="0d424-141">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="0d424-141">schedule</span></span>      |[<span data-ttu-id="0d424-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d424-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="0d424-143">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d424-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="0d424-144">Status der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d424-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="0d424-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="0d424-145">assignmentState</span></span>      |<span data-ttu-id="0d424-146">String</span><span class="sxs-lookup"><span data-stu-id="0d424-146">String</span></span>|         | <span data-ttu-id="0d424-147">Der Status der Aufgabe und die Werte sind möglich `Eligible` oder `Active`.</span><span class="sxs-lookup"><span data-stu-id="0d424-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="0d424-148">Für die Entscheidung der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d424-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="0d424-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d424-149">Response</span></span>
<span data-ttu-id="0d424-150">Diese Methode kann nur angewendet werden, auf Anfragen, die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="0d424-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="0d424-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d424-p106">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="0d424-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d424-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d424-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d424-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="0d424-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d424-155">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="0d424-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d424-156">Response</span></span>
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
