---
title: Abrufen von privilegedRole
description: 'Rufen Sie die Eigenschaften und Beziehungen des PrivilegedRole-Objekts ab. '
ms.openlocfilehash: e68c794a313b739212ec4646f800e2bf85720e8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066106"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="c8466-103">Abrufen von privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c8466-103">Get privilegedRole</span></span>

> <span data-ttu-id="c8466-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8466-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8466-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8466-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8466-106">Rufen Sie die Eigenschaften und Beziehungen des [PrivilegedRole](../resources/privilegedrole.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="c8466-106">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c8466-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8466-107">Permissions</span></span>
<span data-ttu-id="c8466-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8466-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c8466-110">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="c8466-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="c8466-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8466-111">Permission type</span></span>      | <span data-ttu-id="c8466-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8466-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8466-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8466-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c8466-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8466-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8466-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8466-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8466-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8466-116">Not supported.</span></span>    |
|<span data-ttu-id="c8466-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8466-117">Application</span></span> | <span data-ttu-id="c8466-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8466-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8466-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8466-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8466-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c8466-120">Optional query parameters</span></span>
<span data-ttu-id="c8466-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8466-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8466-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8466-122">Request headers</span></span>
| <span data-ttu-id="c8466-123">Name</span><span class="sxs-lookup"><span data-stu-id="c8466-123">Name</span></span>      |<span data-ttu-id="c8466-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8466-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8466-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8466-125">Authorization</span></span>  | <span data-ttu-id="c8466-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8466-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8466-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8466-128">Request body</span></span>
<span data-ttu-id="c8466-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8466-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8466-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8466-130">Response</span></span>

<span data-ttu-id="c8466-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRole](../resources/privilegedrole.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c8466-131">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="c8466-132">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="c8466-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c8466-133">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="c8466-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c8466-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8466-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8466-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8466-135">Request</span></span>
<span data-ttu-id="c8466-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8466-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="c8466-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8466-137">Response</span></span>
<span data-ttu-id="c8466-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8466-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->