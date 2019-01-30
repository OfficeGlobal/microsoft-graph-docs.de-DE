---
title: GovernanceRoleAssignmentRequests aktualisieren
description: So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf GovernanceRoleAssignmentRequests, die in den Status der sind `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 870cd685aade9bb722660b550ae210c6e10d1fe8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643262"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="e37b7-103">GovernanceRoleAssignmentRequests aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e37b7-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e37b7-104">So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="e37b7-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e37b7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e37b7-105">Permissions</span></span>
<span data-ttu-id="e37b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e37b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="e37b7-108">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource, die die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="e37b7-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="e37b7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e37b7-109">Permission type</span></span>      | <span data-ttu-id="e37b7-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e37b7-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e37b7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e37b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e37b7-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e37b7-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e37b7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e37b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e37b7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e37b7-114">Not supported.</span></span>    |
|<span data-ttu-id="e37b7-115">Application</span><span class="sxs-lookup"><span data-stu-id="e37b7-115">Application</span></span> | <span data-ttu-id="e37b7-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e37b7-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e37b7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e37b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="e37b7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e37b7-118">Request headers</span></span>
| <span data-ttu-id="e37b7-119">Name</span><span class="sxs-lookup"><span data-stu-id="e37b7-119">Name</span></span>           | <span data-ttu-id="e37b7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e37b7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e37b7-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e37b7-121">Authorization</span></span>  | <span data-ttu-id="e37b7-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e37b7-122">Bearer {code}</span></span>|
| <span data-ttu-id="e37b7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="e37b7-123">Content-type</span></span>  | <span data-ttu-id="e37b7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e37b7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e37b7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e37b7-125">Request body</span></span>

|<span data-ttu-id="e37b7-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="e37b7-126">Parameters</span></span>      |<span data-ttu-id="e37b7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e37b7-127">Type</span></span>                   |<span data-ttu-id="e37b7-128">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="e37b7-128">Required</span></span> |<span data-ttu-id="e37b7-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e37b7-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="e37b7-130">Grund</span><span class="sxs-lookup"><span data-stu-id="e37b7-130">reason</span></span>        |<span data-ttu-id="e37b7-131">String</span><span class="sxs-lookup"><span data-stu-id="e37b7-131">String</span></span>                 |<span data-ttu-id="e37b7-132">✓</span><span class="sxs-lookup"><span data-stu-id="e37b7-132">✓</span></span>        |<span data-ttu-id="e37b7-133">Der Grund für seine Entscheidung vom Administrator bereitgestellten.</span><span class="sxs-lookup"><span data-stu-id="e37b7-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="e37b7-134">Entscheidung</span><span class="sxs-lookup"><span data-stu-id="e37b7-134">decision</span></span>        |<span data-ttu-id="e37b7-135">String</span><span class="sxs-lookup"><span data-stu-id="e37b7-135">String</span></span>                 |<span data-ttu-id="e37b7-136">✓</span><span class="sxs-lookup"><span data-stu-id="e37b7-136">✓</span></span>        |<span data-ttu-id="e37b7-137">Die Entscheidung Administrator der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e37b7-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="e37b7-138">Der Wert aktualisiert werden sollen, als `AdminApproved` oder `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="e37b7-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="e37b7-139">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="e37b7-139">schedule</span></span>      |[<span data-ttu-id="e37b7-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e37b7-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="e37b7-141">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e37b7-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="e37b7-142">Status der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e37b7-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="e37b7-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e37b7-143">assignmentState</span></span>      |<span data-ttu-id="e37b7-144">String</span><span class="sxs-lookup"><span data-stu-id="e37b7-144">String</span></span>|         | <span data-ttu-id="e37b7-145">Der Status der Aufgabe und die Werte sind möglich `Eligible` oder `Active`.</span><span class="sxs-lookup"><span data-stu-id="e37b7-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="e37b7-146">Für die Entscheidung der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e37b7-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="e37b7-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="e37b7-147">Response</span></span>
<span data-ttu-id="e37b7-148">Diese Methode kann nur angewendet werden, auf Anfragen, die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="e37b7-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="e37b7-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e37b7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e37b7-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e37b7-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e37b7-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e37b7-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="e37b7-153">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e37b7-153">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="e37b7-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="e37b7-154">Response</span></span>
<!-- {
  "blockType": "response",
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
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
