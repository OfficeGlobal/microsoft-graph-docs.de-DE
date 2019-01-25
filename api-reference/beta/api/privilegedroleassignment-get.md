---
title: Abrufen von privilegedRoleAssignment
description: Rufen Sie die Eigenschaften und Beziehungen des PrivilegedRoleAssignment-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: 220001f523971adadd80a406b54f16d22f2ef48e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520319"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="8cb8d-103">Abrufen von privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb8d-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cb8d-104">Rufen Sie die Eigenschaften und Beziehungen des PrivilegedRoleAssignment-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cb8d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8cb8d-105">Permissions</span></span>
<span data-ttu-id="8cb8d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cb8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8cb8d-108">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="8cb8d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8cb8d-109">Permission type</span></span>      | <span data-ttu-id="8cb8d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8cb8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cb8d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8cb8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8cb8d-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cb8d-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cb8d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8cb8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cb8d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8cb8d-114">Not supported.</span></span>    |
|<span data-ttu-id="8cb8d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8cb8d-115">Application</span></span> | <span data-ttu-id="8cb8d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8cb8d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cb8d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8cb8d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cb8d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8cb8d-118">Optional query parameters</span></span>
<span data-ttu-id="8cb8d-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cb8d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8cb8d-120">Request headers</span></span>
| <span data-ttu-id="8cb8d-121">Name</span><span class="sxs-lookup"><span data-stu-id="8cb8d-121">Name</span></span>      |<span data-ttu-id="8cb8d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8cb8d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8cb8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb8d-123">Authorization</span></span>  | <span data-ttu-id="8cb8d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cb8d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8cb8d-126">Request body</span></span>
<span data-ttu-id="8cb8d-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cb8d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8cb8d-128">Response</span></span>

<span data-ttu-id="8cb8d-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="8cb8d-130">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8cb8d-131">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8cb8d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8cb8d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cb8d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8cb8d-133">Request</span></span>
<span data-ttu-id="8cb8d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="8cb8d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8cb8d-135">Response</span></span>
<span data-ttu-id="8cb8d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8cb8d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
