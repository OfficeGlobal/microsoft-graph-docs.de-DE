---
title: Liste Zuordnungen
description: Abrufen einer Liste von PrivilegedRoleAssignment-Objekten, die die Rolle zugeordnet sind. Jeder PrivilegedRoleAssignment stellt eine rollenzuweisung an einen Benutzer.
ms.openlocfilehash: 52cc720381baa6b7c82fe3b5c88d469081da3b81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062865"
---
# <a name="list-assignments"></a><span data-ttu-id="06b17-104">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="06b17-104">List assignments</span></span>

> <span data-ttu-id="06b17-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06b17-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06b17-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06b17-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06b17-107">Abrufen einer Liste von [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekten, die die Rolle zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="06b17-107">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="06b17-108">Jeder [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) stellt eine rollenzuweisung an einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="06b17-108">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="06b17-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06b17-109">Permissions</span></span>
<span data-ttu-id="06b17-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06b17-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="06b17-112">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="06b17-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="06b17-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06b17-113">Permission type</span></span>      | <span data-ttu-id="06b17-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06b17-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06b17-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06b17-115">Delegated (work or school account)</span></span> | <span data-ttu-id="06b17-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06b17-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06b17-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06b17-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06b17-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06b17-118">Not supported.</span></span>    |
|<span data-ttu-id="06b17-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06b17-119">Application</span></span> | <span data-ttu-id="06b17-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06b17-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06b17-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06b17-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="06b17-122">Beachten Sie, dass ``<id>`` ist die Id der Ziel-Rolle.</span><span class="sxs-lookup"><span data-stu-id="06b17-122">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="06b17-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="06b17-123">Optional query parameters</span></span>
<span data-ttu-id="06b17-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06b17-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06b17-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06b17-125">Request headers</span></span>
| <span data-ttu-id="06b17-126">Name</span><span class="sxs-lookup"><span data-stu-id="06b17-126">Name</span></span>      |<span data-ttu-id="06b17-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06b17-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06b17-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="06b17-128">Authorization</span></span>  | <span data-ttu-id="06b17-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06b17-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06b17-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06b17-131">Request body</span></span>
<span data-ttu-id="06b17-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="06b17-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06b17-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="06b17-133">Response</span></span>

<span data-ttu-id="06b17-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="06b17-134">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="06b17-135">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="06b17-135">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="06b17-136">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="06b17-136">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="06b17-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06b17-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06b17-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06b17-138">Request</span></span>
<span data-ttu-id="06b17-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06b17-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="06b17-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="06b17-140">Response</span></span>
<span data-ttu-id="06b17-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06b17-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
