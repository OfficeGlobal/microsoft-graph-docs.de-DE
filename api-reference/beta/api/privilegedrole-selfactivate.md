---
title: 'PrivilegedRole: SelfActivate'
description: Aktivieren Sie die Rolle, die an die anfordernde Person zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515069"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="b1385-103">PrivilegedRole: SelfActivate</span><span class="sxs-lookup"><span data-stu-id="b1385-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1385-104">Aktivieren Sie die Rolle, die an die anfordernde Person zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="b1385-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="b1385-105">**Hinweis:** Eine effektive Dezember 2018, diese API wird nicht mehr unterstützt und sollte nicht verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b1385-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="b1385-106">Verwenden Sie stattdessen die [PrivilegedRoleAssignmentRequest erstellen](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="b1385-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="b1385-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1385-107">Permissions</span></span>
<span data-ttu-id="b1385-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b1385-110">Der Requestor kann nur aufgerufen ```selfActivate``` für die Rolle, die ihm zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="b1385-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="b1385-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1385-111">Permission type</span></span>      | <span data-ttu-id="b1385-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1385-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1385-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1385-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1385-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1385-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1385-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1385-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1385-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1385-116">Not supported.</span></span>    |
|<span data-ttu-id="b1385-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1385-117">Application</span></span> | <span data-ttu-id="b1385-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1385-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1385-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1385-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="b1385-120">Beachten Sie, dass ``<id>`` ist die Ziel-Rolle-ID.</span><span class="sxs-lookup"><span data-stu-id="b1385-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1385-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1385-121">Request headers</span></span>
| <span data-ttu-id="b1385-122">Name</span><span class="sxs-lookup"><span data-stu-id="b1385-122">Name</span></span>       | <span data-ttu-id="b1385-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1385-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b1385-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1385-124">Authorization</span></span>  | <span data-ttu-id="b1385-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1385-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1385-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1385-127">Request body</span></span>
<span data-ttu-id="b1385-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b1385-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1385-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="b1385-129">Parameter</span></span>    | <span data-ttu-id="b1385-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b1385-130">Type</span></span>   |<span data-ttu-id="b1385-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1385-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1385-132">Grund</span><span class="sxs-lookup"><span data-stu-id="b1385-132">reason</span></span>|<span data-ttu-id="b1385-133">string</span><span class="sxs-lookup"><span data-stu-id="b1385-133">string</span></span>|<span data-ttu-id="b1385-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="b1385-134">Optional.</span></span> <span data-ttu-id="b1385-135">Beschreibung der Grund für diese Rolle Aktivierung.</span><span class="sxs-lookup"><span data-stu-id="b1385-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="b1385-136">duration</span><span class="sxs-lookup"><span data-stu-id="b1385-136">duration</span></span>|<span data-ttu-id="b1385-137">string</span><span class="sxs-lookup"><span data-stu-id="b1385-137">string</span></span>|<span data-ttu-id="b1385-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="b1385-138">Optional.</span></span> <span data-ttu-id="b1385-139">Gültige Werte werden konnte ```min``` (minimale Aktivierung Dauer), ```default``` (Standard-Aktivierung Dauer für die Rolle), oder einen double-Wert an, wie viele Stunden die Aktivierung ist.</span><span class="sxs-lookup"><span data-stu-id="b1385-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="b1385-140">Die angegebene Dauer darf nicht länger als die Rolle Aktivierung Dauer aus der Einstellung der Rolle sein.</span><span class="sxs-lookup"><span data-stu-id="b1385-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="b1385-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="b1385-141">ticketNumber</span></span>|<span data-ttu-id="b1385-142">string</span><span class="sxs-lookup"><span data-stu-id="b1385-142">string</span></span>|<span data-ttu-id="b1385-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="b1385-143">Optional.</span></span> <span data-ttu-id="b1385-144">Die Ticket-Nummer, die zum Nachverfolgen von dieser Rolle-Aktivierung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b1385-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="b1385-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="b1385-145">ticketSystem</span></span>|<span data-ttu-id="b1385-146">string</span><span class="sxs-lookup"><span data-stu-id="b1385-146">string</span></span>|<span data-ttu-id="b1385-147">Optional.</span><span class="sxs-lookup"><span data-stu-id="b1385-147">Optional.</span></span> <span data-ttu-id="b1385-148">Das System Ticket.</span><span class="sxs-lookup"><span data-stu-id="b1385-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="b1385-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1385-149">Response</span></span>

<span data-ttu-id="b1385-150">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b1385-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="b1385-151">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="b1385-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b1385-152">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="b1385-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b1385-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1385-153">Example</span></span>
<span data-ttu-id="b1385-154">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="b1385-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b1385-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1385-155">Request</span></span>
<span data-ttu-id="b1385-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1385-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```

##### <a name="response"></a><span data-ttu-id="b1385-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1385-157">Response</span></span>
<span data-ttu-id="b1385-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1385-158">Here is an example of the response.</span></span> 

><span data-ttu-id="b1385-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b1385-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
