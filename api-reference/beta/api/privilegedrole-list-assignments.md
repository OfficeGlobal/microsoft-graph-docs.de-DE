---
title: Liste Zuordnungen
description: Abrufen einer Liste von PrivilegedRoleAssignment-Objekten, die die Rolle zugeordnet sind. Jeder PrivilegedRoleAssignment stellt eine rollenzuweisung an einen Benutzer.
localization_priority: Normal
ms.openlocfilehash: f7dd2b94c5d3ac49a6a8c9183373801f76e27964
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508272"
---
# <a name="list-assignments"></a><span data-ttu-id="07dfd-104">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="07dfd-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07dfd-105">Abrufen einer Liste von [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekten, die die Rolle zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="07dfd-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="07dfd-106">Jeder [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) stellt eine rollenzuweisung an einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="07dfd-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="07dfd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07dfd-107">Permissions</span></span>
<span data-ttu-id="07dfd-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07dfd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07dfd-110">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="07dfd-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="07dfd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07dfd-111">Permission type</span></span>      | <span data-ttu-id="07dfd-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07dfd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07dfd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07dfd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07dfd-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07dfd-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07dfd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07dfd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07dfd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07dfd-116">Not supported.</span></span>    |
|<span data-ttu-id="07dfd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07dfd-117">Application</span></span> | <span data-ttu-id="07dfd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07dfd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07dfd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07dfd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="07dfd-120">Beachten Sie, dass ``<id>`` ist die Id der Ziel-Rolle.</span><span class="sxs-lookup"><span data-stu-id="07dfd-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="07dfd-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="07dfd-121">Optional query parameters</span></span>
<span data-ttu-id="07dfd-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07dfd-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07dfd-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07dfd-123">Request headers</span></span>
| <span data-ttu-id="07dfd-124">Name</span><span class="sxs-lookup"><span data-stu-id="07dfd-124">Name</span></span>      |<span data-ttu-id="07dfd-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07dfd-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07dfd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="07dfd-126">Authorization</span></span>  | <span data-ttu-id="07dfd-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07dfd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07dfd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07dfd-129">Request body</span></span>
<span data-ttu-id="07dfd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="07dfd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07dfd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="07dfd-131">Response</span></span>

<span data-ttu-id="07dfd-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07dfd-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="07dfd-133">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="07dfd-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="07dfd-134">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="07dfd-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="07dfd-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07dfd-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07dfd-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07dfd-136">Request</span></span>
<span data-ttu-id="07dfd-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07dfd-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="07dfd-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="07dfd-138">Response</span></span>
<span data-ttu-id="07dfd-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07dfd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
