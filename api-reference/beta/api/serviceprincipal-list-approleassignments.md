---
title: 'ServicePrincipal: AppRoleAssignments auflisten'
description: Abrufen einer Liste von Approleassignment-Objekten.
localization_priority: Normal
ms.openlocfilehash: af98d4b92e936a961d0edefe6a4f00c71a5a75ed
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641985"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="1380c-103">ServicePrincipal: AppRoleAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="1380c-103">servicePrincipal: List appRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1380c-104">Abrufen einer Liste von Approleassignment-Objekten.</span><span class="sxs-lookup"><span data-stu-id="1380c-104">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1380c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1380c-105">Permissions</span></span>
<span data-ttu-id="1380c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1380c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1380c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1380c-108">Permission type</span></span>      | <span data-ttu-id="1380c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1380c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1380c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1380c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1380c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1380c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1380c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1380c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1380c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1380c-113">Not supported.</span></span>    |
|<span data-ttu-id="1380c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1380c-114">Application</span></span> | <span data-ttu-id="1380c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1380c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1380c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1380c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1380c-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1380c-117">Optional query parameters</span></span>
<span data-ttu-id="1380c-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1380c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1380c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1380c-119">Request headers</span></span>
| <span data-ttu-id="1380c-120">Name</span><span class="sxs-lookup"><span data-stu-id="1380c-120">Name</span></span>       | <span data-ttu-id="1380c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="1380c-121">Type</span></span> | <span data-ttu-id="1380c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1380c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1380c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1380c-123">Authorization</span></span>  | <span data-ttu-id="1380c-124">string</span><span class="sxs-lookup"><span data-stu-id="1380c-124">string</span></span>  | <span data-ttu-id="1380c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1380c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1380c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1380c-127">Request body</span></span>
<span data-ttu-id="1380c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1380c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1380c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1380c-129">Response</span></span>

<span data-ttu-id="1380c-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [AppRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1380c-130">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1380c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1380c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1380c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1380c-132">Request</span></span>
<span data-ttu-id="1380c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1380c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="1380c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1380c-134">Response</span></span>
<span data-ttu-id="1380c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1380c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
