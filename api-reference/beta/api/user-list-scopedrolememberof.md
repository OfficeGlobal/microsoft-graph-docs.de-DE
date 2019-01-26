---
title: scopedAdministratorOf auflisten
description: Abrufen einer Liste der ScopedRoleMembership für den Benutzer.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: af5d74161aff083e6d1bc70ad8efa7866d4cc02c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577333"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="e6242-103">scopedAdministratorOf auflisten</span><span class="sxs-lookup"><span data-stu-id="e6242-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6242-104">Abrufen einer Liste der [ScopedRoleMembership](../resources/scopedrolemembership.md) für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e6242-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6242-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6242-105">Permissions</span></span>
<span data-ttu-id="e6242-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e6242-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6242-108">Permission type</span></span>      | <span data-ttu-id="e6242-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6242-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6242-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6242-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6242-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6242-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6242-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6242-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6242-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6242-113">Not supported.</span></span>    |
|<span data-ttu-id="e6242-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6242-114">Application</span></span> | <span data-ttu-id="e6242-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6242-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6242-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6242-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6242-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e6242-117">Optional query parameters</span></span>
<span data-ttu-id="e6242-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6242-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6242-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6242-119">Request headers</span></span>
| <span data-ttu-id="e6242-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e6242-120">Header</span></span>       | <span data-ttu-id="e6242-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e6242-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6242-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6242-122">Authorization</span></span>  | <span data-ttu-id="e6242-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6242-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6242-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6242-125">Request body</span></span>
<span data-ttu-id="e6242-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6242-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6242-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6242-127">Response</span></span>

<span data-ttu-id="e6242-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ScopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="e6242-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6242-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6242-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6242-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6242-130">Request</span></span>
<span data-ttu-id="e6242-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6242-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
##### <a name="response"></a><span data-ttu-id="e6242-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6242-132">Response</span></span>
<span data-ttu-id="e6242-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6242-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-scopedrolememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
