---
title: GovernanceRoleAssignmentRequests aktualisieren
description: So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf GovernanceRoleAssignmentRequests, die in den Status der sind `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 3d68e06688922177e2a1a183a9fe4bfc6be6a91d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874935"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="65bda-103">GovernanceRoleAssignmentRequests aktualisieren</span><span class="sxs-lookup"><span data-stu-id="65bda-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="65bda-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65bda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65bda-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65bda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65bda-106">So aktualisieren Sie ihre Entscheidungen Administratoren können (`AdminApproved` oder `AdminDenied`) auf [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="65bda-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="65bda-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65bda-107">Permissions</span></span>
<span data-ttu-id="65bda-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65bda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="65bda-110">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource, die die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="65bda-110">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="65bda-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65bda-111">Permission type</span></span>      | <span data-ttu-id="65bda-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65bda-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65bda-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65bda-113">Delegated (work or school account)</span></span> | <span data-ttu-id="65bda-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="65bda-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="65bda-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65bda-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65bda-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65bda-116">Not supported.</span></span>    |
|<span data-ttu-id="65bda-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65bda-117">Application</span></span> | <span data-ttu-id="65bda-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="65bda-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="65bda-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65bda-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="65bda-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65bda-120">Request headers</span></span>
| <span data-ttu-id="65bda-121">Name</span><span class="sxs-lookup"><span data-stu-id="65bda-121">Name</span></span>           | <span data-ttu-id="65bda-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65bda-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65bda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65bda-123">Authorization</span></span>  | <span data-ttu-id="65bda-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="65bda-124">Bearer {code}</span></span>|
| <span data-ttu-id="65bda-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="65bda-125">Content-type</span></span>  | <span data-ttu-id="65bda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65bda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65bda-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65bda-127">Request body</span></span>

|<span data-ttu-id="65bda-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="65bda-128">Parameters</span></span>      |<span data-ttu-id="65bda-129">Typ</span><span class="sxs-lookup"><span data-stu-id="65bda-129">Type</span></span>                   |<span data-ttu-id="65bda-130">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="65bda-130">Required</span></span> |<span data-ttu-id="65bda-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65bda-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="65bda-132">Grund</span><span class="sxs-lookup"><span data-stu-id="65bda-132">reason</span></span>        |<span data-ttu-id="65bda-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65bda-133">String</span></span>                 |<span data-ttu-id="65bda-134">✓</span><span class="sxs-lookup"><span data-stu-id="65bda-134">✓</span></span>        |<span data-ttu-id="65bda-135">Der Grund für seine Entscheidung vom Administrator bereitgestellten.</span><span class="sxs-lookup"><span data-stu-id="65bda-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="65bda-136">Entscheidung</span><span class="sxs-lookup"><span data-stu-id="65bda-136">decision</span></span>        |<span data-ttu-id="65bda-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65bda-137">String</span></span>                 |<span data-ttu-id="65bda-138">✓</span><span class="sxs-lookup"><span data-stu-id="65bda-138">✓</span></span>        |<span data-ttu-id="65bda-139">Die Entscheidung Administrator der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65bda-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="65bda-140">Der Wert aktualisiert werden sollen, als `AdminApproved` oder `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="65bda-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="65bda-141">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="65bda-141">schedule</span></span>      |[<span data-ttu-id="65bda-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="65bda-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="65bda-143">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65bda-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="65bda-144">Status der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65bda-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="65bda-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="65bda-145">assignmentState</span></span>      |<span data-ttu-id="65bda-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65bda-146">String</span></span>|         | <span data-ttu-id="65bda-147">Der Status der Aufgabe und die Werte sind möglich `Eligible` oder `Active`.</span><span class="sxs-lookup"><span data-stu-id="65bda-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="65bda-148">Für die Entscheidung der `AdminApproved`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65bda-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="65bda-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="65bda-149">Response</span></span>
<span data-ttu-id="65bda-150">Diese Methode kann nur angewendet werden, auf Anfragen, die in den Status der sind `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="65bda-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="65bda-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65bda-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65bda-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65bda-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65bda-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65bda-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="65bda-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65bda-155">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="65bda-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="65bda-156">Response</span></span>
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
