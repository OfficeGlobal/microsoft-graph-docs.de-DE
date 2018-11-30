---
title: 'PrivilegedRole: SelfActivate'
description: Aktivieren Sie die Rolle, die an die anfordernde Person zugewiesen ist.
ms.openlocfilehash: bff445bf1fa5d7c0dfbce080b4361b0479b7dcb7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064164"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="51b27-103">PrivilegedRole: SelfActivate</span><span class="sxs-lookup"><span data-stu-id="51b27-103">privilegedRole: selfActivate</span></span>

><span data-ttu-id="51b27-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51b27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51b27-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51b27-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51b27-106">Aktivieren Sie die Rolle, die an die anfordernde Person zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="51b27-106">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="51b27-107">**Hinweis:** Eine effektive Dezember 2018, diese API wird nicht mehr unterstützt und sollte nicht verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="51b27-107">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="51b27-108">Verwenden Sie stattdessen die [PrivilegedRoleAssignmentRequest erstellen](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="51b27-108">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="51b27-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51b27-109">Permissions</span></span>
<span data-ttu-id="51b27-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51b27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="51b27-112">Der Requestor kann nur aufgerufen ```selfActivate``` für die Rolle, die ihm zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="51b27-112">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="51b27-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51b27-113">Permission type</span></span>      | <span data-ttu-id="51b27-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51b27-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51b27-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51b27-115">Delegated (work or school account)</span></span> | <span data-ttu-id="51b27-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51b27-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51b27-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51b27-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51b27-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51b27-118">Not supported.</span></span>    |
|<span data-ttu-id="51b27-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51b27-119">Application</span></span> | <span data-ttu-id="51b27-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51b27-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51b27-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51b27-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="51b27-122">Beachten Sie, dass ``<id>`` ist die Ziel-Rolle-ID.</span><span class="sxs-lookup"><span data-stu-id="51b27-122">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51b27-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51b27-123">Request headers</span></span>
| <span data-ttu-id="51b27-124">Name</span><span class="sxs-lookup"><span data-stu-id="51b27-124">Name</span></span>       | <span data-ttu-id="51b27-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51b27-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51b27-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="51b27-126">Authorization</span></span>  | <span data-ttu-id="51b27-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="51b27-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51b27-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51b27-129">Request body</span></span>
<span data-ttu-id="51b27-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="51b27-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51b27-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="51b27-131">Parameter</span></span>    | <span data-ttu-id="51b27-132">Typ</span><span class="sxs-lookup"><span data-stu-id="51b27-132">Type</span></span>   |<span data-ttu-id="51b27-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51b27-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51b27-134">Grund</span><span class="sxs-lookup"><span data-stu-id="51b27-134">reason</span></span>|<span data-ttu-id="51b27-135">string</span><span class="sxs-lookup"><span data-stu-id="51b27-135">string</span></span>|<span data-ttu-id="51b27-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="51b27-136">Optional.</span></span> <span data-ttu-id="51b27-137">Beschreibung der Grund für diese Rolle Aktivierung.</span><span class="sxs-lookup"><span data-stu-id="51b27-137">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="51b27-138">duration</span><span class="sxs-lookup"><span data-stu-id="51b27-138">duration</span></span>|<span data-ttu-id="51b27-139">string</span><span class="sxs-lookup"><span data-stu-id="51b27-139">string</span></span>|<span data-ttu-id="51b27-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="51b27-140">Optional.</span></span> <span data-ttu-id="51b27-141">Gültige Werte werden konnte ```min``` (minimale Aktivierung Dauer), ```default``` (Standard-Aktivierung Dauer für die Rolle), oder einen double-Wert an, wie viele Stunden die Aktivierung ist.</span><span class="sxs-lookup"><span data-stu-id="51b27-141">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="51b27-142">Die angegebene Dauer darf nicht länger als die Rolle Aktivierung Dauer aus der Einstellung der Rolle sein.</span><span class="sxs-lookup"><span data-stu-id="51b27-142">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="51b27-143">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="51b27-143">ticketNumber</span></span>|<span data-ttu-id="51b27-144">string</span><span class="sxs-lookup"><span data-stu-id="51b27-144">string</span></span>|<span data-ttu-id="51b27-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="51b27-145">Optional.</span></span> <span data-ttu-id="51b27-146">Die Ticket-Nummer, die zum Nachverfolgen von dieser Rolle-Aktivierung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="51b27-146">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="51b27-147">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="51b27-147">ticketSystem</span></span>|<span data-ttu-id="51b27-148">string</span><span class="sxs-lookup"><span data-stu-id="51b27-148">string</span></span>|<span data-ttu-id="51b27-149">Optional.</span><span class="sxs-lookup"><span data-stu-id="51b27-149">Optional.</span></span> <span data-ttu-id="51b27-150">Das System Ticket.</span><span class="sxs-lookup"><span data-stu-id="51b27-150">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="51b27-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="51b27-151">Response</span></span>

<span data-ttu-id="51b27-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="51b27-152">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="51b27-153">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="51b27-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="51b27-154">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="51b27-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="51b27-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51b27-155">Example</span></span>
<span data-ttu-id="51b27-156">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="51b27-156">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51b27-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51b27-157">Request</span></span>
<span data-ttu-id="51b27-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51b27-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="51b27-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="51b27-159">Response</span></span>
<span data-ttu-id="51b27-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51b27-160">Here is an example of the response.</span></span> 

><span data-ttu-id="51b27-p110">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="51b27-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
