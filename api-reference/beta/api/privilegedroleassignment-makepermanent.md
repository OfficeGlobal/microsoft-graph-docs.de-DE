---
title: 'PrivilegedRoleAssignment: MakePermanent'
description: Stellen Sie die rollenzuweisung als dauerhaft entfernt.
localization_priority: Normal
ms.openlocfilehash: c2c834454f7c6c7bd931b6985f5b35b92e48096d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849693"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="62010-103">PrivilegedRoleAssignment: MakePermanent</span><span class="sxs-lookup"><span data-stu-id="62010-103">privilegedRoleAssignment: makePermanent</span></span>

> <span data-ttu-id="62010-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="62010-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62010-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62010-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62010-106">Stellen Sie die rollenzuweisung als dauerhaft entfernt.</span><span class="sxs-lookup"><span data-stu-id="62010-106">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="62010-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="62010-107">Permissions</span></span>
<span data-ttu-id="62010-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62010-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="62010-110">Der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="62010-110">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="62010-111">Andernfalls wird HTTP 403 Verboten Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62010-111">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="62010-112">Der Requestor muss _privilegierten Rolle_ Administratorrolle haben.</span><span class="sxs-lookup"><span data-stu-id="62010-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="62010-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62010-113">Permission type</span></span>      | <span data-ttu-id="62010-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62010-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62010-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62010-115">Delegated (work or school account)</span></span> | <span data-ttu-id="62010-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62010-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62010-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62010-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62010-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62010-118">Not supported.</span></span>    |
|<span data-ttu-id="62010-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62010-119">Application</span></span> | <span data-ttu-id="62010-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62010-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62010-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62010-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="62010-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62010-122">Request headers</span></span>
| <span data-ttu-id="62010-123">Name</span><span class="sxs-lookup"><span data-stu-id="62010-123">Name</span></span>       | <span data-ttu-id="62010-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62010-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="62010-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="62010-125">Authorization</span></span>  | <span data-ttu-id="62010-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="62010-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62010-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62010-128">Request body</span></span>
<span data-ttu-id="62010-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="62010-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62010-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="62010-130">Parameter</span></span>    | <span data-ttu-id="62010-131">Typ</span><span class="sxs-lookup"><span data-stu-id="62010-131">Type</span></span>   |<span data-ttu-id="62010-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62010-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62010-133">Grund</span><span class="sxs-lookup"><span data-stu-id="62010-133">reason</span></span>|<span data-ttu-id="62010-134">string</span><span class="sxs-lookup"><span data-stu-id="62010-134">string</span></span>|<span data-ttu-id="62010-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="62010-135">Optional.</span></span> <span data-ttu-id="62010-136">Der Grund für diesen Anruf.</span><span class="sxs-lookup"><span data-stu-id="62010-136">The reason to make this call.</span></span>|
|<span data-ttu-id="62010-137">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="62010-137">ticketNumber</span></span>|<span data-ttu-id="62010-138">string</span><span class="sxs-lookup"><span data-stu-id="62010-138">string</span></span>|<span data-ttu-id="62010-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="62010-139">Optional.</span></span> <span data-ttu-id="62010-140">Die Anzahl der Ticket, die diese Aktion zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="62010-140">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="62010-141">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="62010-141">ticketSystem</span></span>|<span data-ttu-id="62010-142">string</span><span class="sxs-lookup"><span data-stu-id="62010-142">string</span></span>|<span data-ttu-id="62010-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="62010-143">Optional.</span></span> <span data-ttu-id="62010-144">Das System Ticket.</span><span class="sxs-lookup"><span data-stu-id="62010-144">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="62010-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="62010-145">Response</span></span>

<span data-ttu-id="62010-146">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="62010-146">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62010-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62010-147">Example</span></span>
<span data-ttu-id="62010-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="62010-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="62010-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62010-149">Request</span></span>
<span data-ttu-id="62010-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62010-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="62010-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="62010-151">Response</span></span>
<span data-ttu-id="62010-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62010-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
