---
title: 'PrivilegedRoleAssignment: MakePermanent'
description: Stellen Sie die rollenzuweisung als dauerhaft entfernt.
localization_priority: Normal
ms.openlocfilehash: 9c6334662cf8496262b49b14ceb3f51f7a4f8dbc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511394"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="3e76f-103">PrivilegedRoleAssignment: MakePermanent</span><span class="sxs-lookup"><span data-stu-id="3e76f-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e76f-104">Stellen Sie die rollenzuweisung als dauerhaft entfernt.</span><span class="sxs-lookup"><span data-stu-id="3e76f-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e76f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e76f-105">Permissions</span></span>
<span data-ttu-id="3e76f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e76f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3e76f-108">Der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="3e76f-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3e76f-109">Andernfalls wird HTTP 403 Verboten Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e76f-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="3e76f-110">Der Requestor muss _privilegierten Rolle_ Administratorrolle haben.</span><span class="sxs-lookup"><span data-stu-id="3e76f-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="3e76f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e76f-111">Permission type</span></span>      | <span data-ttu-id="3e76f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e76f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e76f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e76f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3e76f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e76f-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e76f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e76f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e76f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e76f-116">Not supported.</span></span>    |
|<span data-ttu-id="3e76f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e76f-117">Application</span></span> | <span data-ttu-id="3e76f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e76f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e76f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e76f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="3e76f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e76f-120">Request headers</span></span>
| <span data-ttu-id="3e76f-121">Name</span><span class="sxs-lookup"><span data-stu-id="3e76f-121">Name</span></span>       | <span data-ttu-id="3e76f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e76f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e76f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e76f-123">Authorization</span></span>  | <span data-ttu-id="3e76f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e76f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e76f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e76f-126">Request body</span></span>
<span data-ttu-id="3e76f-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3e76f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e76f-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="3e76f-128">Parameter</span></span>    | <span data-ttu-id="3e76f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3e76f-129">Type</span></span>   |<span data-ttu-id="3e76f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e76f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e76f-131">Grund</span><span class="sxs-lookup"><span data-stu-id="3e76f-131">reason</span></span>|<span data-ttu-id="3e76f-132">string</span><span class="sxs-lookup"><span data-stu-id="3e76f-132">string</span></span>|<span data-ttu-id="3e76f-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="3e76f-133">Optional.</span></span> <span data-ttu-id="3e76f-134">Der Grund für diesen Anruf.</span><span class="sxs-lookup"><span data-stu-id="3e76f-134">The reason to make this call.</span></span>|
|<span data-ttu-id="3e76f-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="3e76f-135">ticketNumber</span></span>|<span data-ttu-id="3e76f-136">string</span><span class="sxs-lookup"><span data-stu-id="3e76f-136">string</span></span>|<span data-ttu-id="3e76f-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="3e76f-137">Optional.</span></span> <span data-ttu-id="3e76f-138">Die Anzahl der Ticket, die diese Aktion zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="3e76f-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="3e76f-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="3e76f-139">ticketSystem</span></span>|<span data-ttu-id="3e76f-140">string</span><span class="sxs-lookup"><span data-stu-id="3e76f-140">string</span></span>|<span data-ttu-id="3e76f-141">Optional.</span><span class="sxs-lookup"><span data-stu-id="3e76f-141">Optional.</span></span> <span data-ttu-id="3e76f-142">Das System Ticket.</span><span class="sxs-lookup"><span data-stu-id="3e76f-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="3e76f-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e76f-143">Response</span></span>

<span data-ttu-id="3e76f-144">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3e76f-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e76f-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e76f-145">Example</span></span>
<span data-ttu-id="3e76f-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3e76f-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e76f-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e76f-147">Request</span></span>
<span data-ttu-id="3e76f-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e76f-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makepermanent"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makePermanent
Content-type: application/json
Content-length: 110

{
  "reason": "reason-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```

##### <a name="response"></a><span data-ttu-id="3e76f-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e76f-149">Response</span></span>
<span data-ttu-id="3e76f-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e76f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
