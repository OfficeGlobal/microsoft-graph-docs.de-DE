---
title: 'PrivilegedRoleAssignment: MakeEligible'
description: Stellen Sie die rollenzuweisung als geeignet. Wenn die rollenzuweisung bereits vor dem Aufruf berechtigt ist, hat keine Auswirkung. Wenn die rollenzuweisung dauerhaft gelöscht wird und der Requestor unterscheidet sich von den Zielbenutzer, die rollenzuweisung wird sind berechtigt, und die Rolle wird für die Zielbenutzer deaktiviert werden. Wenn der Requestor der Zielbenutzer ist und die Rolle Sicherheitsadministrator oder privilegierten Rollen-Administrator ist, wird die Rolle mit den standardmäßigen Gültigkeitszeitraum aktiviert werden.
localization_priority: Normal
ms.openlocfilehash: 90f606ed1550f6341251e5185e620c29838a9ac9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822589"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="06c99-106">PrivilegedRoleAssignment: MakeEligible</span><span class="sxs-lookup"><span data-stu-id="06c99-106">privilegedRoleAssignment: makeEligible</span></span>

> <span data-ttu-id="06c99-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06c99-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06c99-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06c99-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06c99-109">Stellen Sie die rollenzuweisung als geeignet.</span><span class="sxs-lookup"><span data-stu-id="06c99-109">Make the role assignment as eligible.</span></span> <span data-ttu-id="06c99-110">Wenn die rollenzuweisung bereits vor dem Aufruf berechtigt ist, hat keine Auswirkung.</span><span class="sxs-lookup"><span data-stu-id="06c99-110">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="06c99-111">Wenn die rollenzuweisung dauerhaft gelöscht wird und der Requestor unterscheidet sich von den Zielbenutzer, die rollenzuweisung wird sind berechtigt, und die Rolle wird für die Zielbenutzer deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="06c99-111">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="06c99-112">Wenn der Requestor der Zielbenutzer ist und die Rolle Sicherheitsadministrator oder privilegierten Rollen-Administrator ist, wird die Rolle mit den standardmäßigen Gültigkeitszeitraum aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="06c99-112">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="06c99-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06c99-113">Permissions</span></span>
<span data-ttu-id="06c99-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c99-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="06c99-116">Der Requestor muss _privilegierten Rolle_ Administratorrolle haben.</span><span class="sxs-lookup"><span data-stu-id="06c99-116">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="06c99-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06c99-117">Permission type</span></span>      | <span data-ttu-id="06c99-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06c99-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06c99-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06c99-119">Delegated (work or school account)</span></span> | <span data-ttu-id="06c99-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06c99-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06c99-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06c99-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06c99-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06c99-122">Not supported.</span></span>    |
|<span data-ttu-id="06c99-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06c99-123">Application</span></span> | <span data-ttu-id="06c99-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06c99-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06c99-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06c99-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="06c99-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06c99-126">Request headers</span></span>
| <span data-ttu-id="06c99-127">Name</span><span class="sxs-lookup"><span data-stu-id="06c99-127">Name</span></span>       | <span data-ttu-id="06c99-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06c99-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06c99-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c99-129">Authorization</span></span>  | <span data-ttu-id="06c99-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06c99-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06c99-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06c99-132">Request body</span></span>
<span data-ttu-id="06c99-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="06c99-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06c99-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="06c99-134">Response</span></span>

<span data-ttu-id="06c99-135">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="06c99-135">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="06c99-136">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="06c99-136">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="06c99-137">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="06c99-137">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="06c99-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06c99-138">Example</span></span>
<span data-ttu-id="06c99-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="06c99-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06c99-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06c99-140">Request</span></span>
<span data-ttu-id="06c99-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06c99-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="06c99-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="06c99-142">Response</span></span>
<span data-ttu-id="06c99-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06c99-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
