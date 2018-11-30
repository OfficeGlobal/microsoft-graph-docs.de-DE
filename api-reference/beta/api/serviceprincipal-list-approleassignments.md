---
title: 'ServicePrincipal: AppRoleAssignments auflisten'
description: Abrufen einer Liste von Approleassignment-Objekten.
ms.openlocfilehash: 55a2a90981236afadabafdd8dc24e21aa874dbbe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062831"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="fd281-103">ServicePrincipal: AppRoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="fd281-103">servicePrincipal: List appRoleAssignments</span></span>

> <span data-ttu-id="fd281-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd281-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd281-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd281-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd281-106">Abrufen einer Liste von Approleassignment-Objekten.</span><span class="sxs-lookup"><span data-stu-id="fd281-106">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd281-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd281-107">Permissions</span></span>
<span data-ttu-id="fd281-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd281-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd281-110">Permission type</span></span>      | <span data-ttu-id="fd281-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd281-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd281-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd281-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd281-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd281-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd281-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd281-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd281-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd281-115">Not supported.</span></span>    |
|<span data-ttu-id="fd281-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd281-116">Application</span></span> | <span data-ttu-id="fd281-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd281-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd281-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd281-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd281-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd281-119">Optional query parameters</span></span>
<span data-ttu-id="fd281-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd281-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd281-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd281-121">Request headers</span></span>
| <span data-ttu-id="fd281-122">Name</span><span class="sxs-lookup"><span data-stu-id="fd281-122">Name</span></span>       | <span data-ttu-id="fd281-123">Typ</span><span class="sxs-lookup"><span data-stu-id="fd281-123">Type</span></span> | <span data-ttu-id="fd281-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd281-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd281-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd281-125">Authorization</span></span>  | <span data-ttu-id="fd281-126">string</span><span class="sxs-lookup"><span data-stu-id="fd281-126">string</span></span>  | <span data-ttu-id="fd281-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd281-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd281-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd281-129">Request body</span></span>
<span data-ttu-id="fd281-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd281-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd281-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd281-131">Response</span></span>

<span data-ttu-id="fd281-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [AppRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fd281-132">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd281-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd281-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd281-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd281-134">Request</span></span>
<span data-ttu-id="fd281-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd281-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="fd281-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd281-136">Response</span></span>
<span data-ttu-id="fd281-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd281-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->