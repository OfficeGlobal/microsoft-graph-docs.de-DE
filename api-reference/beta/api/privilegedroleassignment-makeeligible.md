---
title: 'PrivilegedRoleAssignment: MakeEligible'
description: Stellen Sie die rollenzuweisung als geeignet. Wenn die rollenzuweisung bereits vor dem Aufruf berechtigt ist, hat keine Auswirkung. Wenn die rollenzuweisung dauerhaft gelöscht wird und der Requestor unterscheidet sich von den Zielbenutzer, die rollenzuweisung wird sind berechtigt, und die Rolle wird für die Zielbenutzer deaktiviert werden. Wenn der Requestor der Zielbenutzer ist und die Rolle Sicherheitsadministrator oder privilegierten Rollen-Administrator ist, wird die Rolle mit den standardmäßigen Gültigkeitszeitraum aktiviert werden.
localization_priority: Normal
ms.openlocfilehash: 54260da3f69819a1f7a351e072f8af851f0e3d3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527236"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="56097-106">PrivilegedRoleAssignment: MakeEligible</span><span class="sxs-lookup"><span data-stu-id="56097-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56097-107">Stellen Sie die rollenzuweisung als geeignet.</span><span class="sxs-lookup"><span data-stu-id="56097-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="56097-108">Wenn die rollenzuweisung bereits vor dem Aufruf berechtigt ist, hat keine Auswirkung.</span><span class="sxs-lookup"><span data-stu-id="56097-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="56097-109">Wenn die rollenzuweisung dauerhaft gelöscht wird und der Requestor unterscheidet sich von den Zielbenutzer, die rollenzuweisung wird sind berechtigt, und die Rolle wird für die Zielbenutzer deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="56097-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="56097-110">Wenn der Requestor der Zielbenutzer ist und die Rolle Sicherheitsadministrator oder privilegierten Rollen-Administrator ist, wird die Rolle mit den standardmäßigen Gültigkeitszeitraum aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="56097-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="56097-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="56097-111">Permissions</span></span>
<span data-ttu-id="56097-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56097-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="56097-114">Der Requestor muss _privilegierten Rolle_ Administratorrolle haben.</span><span class="sxs-lookup"><span data-stu-id="56097-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="56097-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56097-115">Permission type</span></span>      | <span data-ttu-id="56097-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56097-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56097-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56097-117">Delegated (work or school account)</span></span> | <span data-ttu-id="56097-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56097-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56097-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56097-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56097-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56097-120">Not supported.</span></span>    |
|<span data-ttu-id="56097-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56097-121">Application</span></span> | <span data-ttu-id="56097-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56097-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56097-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56097-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="56097-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56097-124">Request headers</span></span>
| <span data-ttu-id="56097-125">Name</span><span class="sxs-lookup"><span data-stu-id="56097-125">Name</span></span>       | <span data-ttu-id="56097-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56097-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56097-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="56097-127">Authorization</span></span>  | <span data-ttu-id="56097-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56097-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56097-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56097-130">Request body</span></span>
<span data-ttu-id="56097-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56097-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56097-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="56097-132">Response</span></span>

<span data-ttu-id="56097-133">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="56097-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="56097-134">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="56097-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="56097-135">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="56097-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="56097-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56097-136">Example</span></span>
<span data-ttu-id="56097-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="56097-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56097-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56097-138">Request</span></span>
<span data-ttu-id="56097-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56097-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="56097-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="56097-140">Response</span></span>
<span data-ttu-id="56097-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56097-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-makeeligible.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
