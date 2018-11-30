---
title: Erstellen von privilegedRoleAssignment
description: Verwenden Sie diese API, um eine neue PrivilegedRoleAssignment erstellen.
ms.openlocfilehash: cee00a71ff9ff233902ba19fb1f3f699ab746f98
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062048"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="8131f-103">Erstellen von privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8131f-103">Create privilegedRoleAssignment</span></span>

> <span data-ttu-id="8131f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8131f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8131f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8131f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8131f-106">Verwenden Sie diese API, um eine neue [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8131f-106">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8131f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8131f-107">Permissions</span></span>
<span data-ttu-id="8131f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8131f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8131f-110">Der Requestor muss _privilegierten Rolle_ Administratorrolle haben.</span><span class="sxs-lookup"><span data-stu-id="8131f-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="8131f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8131f-111">Permission type</span></span>      | <span data-ttu-id="8131f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8131f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8131f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8131f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8131f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8131f-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8131f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8131f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8131f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8131f-116">Not supported.</span></span>    |
|<span data-ttu-id="8131f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8131f-117">Application</span></span> | <span data-ttu-id="8131f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8131f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8131f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8131f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="8131f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8131f-120">Request headers</span></span>
| <span data-ttu-id="8131f-121">Name</span><span class="sxs-lookup"><span data-stu-id="8131f-121">Name</span></span>       | <span data-ttu-id="8131f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8131f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8131f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8131f-123">Authorization</span></span>  | <span data-ttu-id="8131f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8131f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8131f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8131f-126">Request body</span></span>
<span data-ttu-id="8131f-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8131f-127">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8131f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8131f-128">Response</span></span>

<span data-ttu-id="8131f-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8131f-129">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="8131f-130">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="8131f-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8131f-131">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="8131f-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8131f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8131f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8131f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8131f-133">Request</span></span>
<span data-ttu-id="8131f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8131f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="8131f-135">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8131f-135">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8131f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8131f-136">Response</span></span>
<span data-ttu-id="8131f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8131f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->