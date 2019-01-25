---
title: Erstellen von privilegedRoleAssignment
description: Verwenden Sie diese API, um eine neue PrivilegedRoleAssignment erstellen.
localization_priority: Normal
ms.openlocfilehash: 5522956b129eae8a19fd00b0e70b41380dbdd25e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513403"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="574b4-103">Erstellen von privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="574b4-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="574b4-104">Verwenden Sie diese API, um eine neue [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="574b4-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="574b4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="574b4-105">Permissions</span></span>
<span data-ttu-id="574b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="574b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="574b4-108">Der Requestor muss _privilegierten Rolle_ Administratorrolle haben.</span><span class="sxs-lookup"><span data-stu-id="574b4-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="574b4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="574b4-109">Permission type</span></span>      | <span data-ttu-id="574b4-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="574b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="574b4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="574b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="574b4-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="574b4-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="574b4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="574b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="574b4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="574b4-114">Not supported.</span></span>    |
|<span data-ttu-id="574b4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="574b4-115">Application</span></span> | <span data-ttu-id="574b4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="574b4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="574b4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="574b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="574b4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="574b4-118">Request headers</span></span>
| <span data-ttu-id="574b4-119">Name</span><span class="sxs-lookup"><span data-stu-id="574b4-119">Name</span></span>       | <span data-ttu-id="574b4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="574b4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="574b4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="574b4-121">Authorization</span></span>  | <span data-ttu-id="574b4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="574b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="574b4-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="574b4-124">Request body</span></span>
<span data-ttu-id="574b4-125">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="574b4-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="574b4-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="574b4-126">Response</span></span>

<span data-ttu-id="574b4-127">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="574b4-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="574b4-128">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="574b4-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="574b4-129">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="574b4-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="574b4-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="574b4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="574b4-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="574b4-131">Request</span></span>
<span data-ttu-id="574b4-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="574b4-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="574b4-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="574b4-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="574b4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="574b4-134">Response</span></span>
<span data-ttu-id="574b4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="574b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
