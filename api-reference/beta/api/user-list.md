---
title: Benutzer auflisten
description: Dient zum Abrufen einer Liste von Benutzerobjekten.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00cf39a3e50c6c9911471f60a1cc7def1ee4563b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528900"
---
# <a name="list-users"></a><span data-ttu-id="ce06e-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="ce06e-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce06e-104">Mit dieser API können Sie eine Liste von Benutzerobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="ce06e-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce06e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ce06e-105">Permissions</span></span>

<span data-ttu-id="ce06e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce06e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce06e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce06e-108">Permission type</span></span>      | <span data-ttu-id="ce06e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce06e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce06e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce06e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce06e-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce06e-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ce06e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce06e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce06e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce06e-113">Not supported.</span></span>    |
|<span data-ttu-id="ce06e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce06e-114">Application</span></span> | <span data-ttu-id="ce06e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce06e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce06e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce06e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce06e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ce06e-117">Optional query parameters</span></span>

<span data-ttu-id="ce06e-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ce06e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce06e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce06e-119">Request headers</span></span>
| <span data-ttu-id="ce06e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce06e-120">Header</span></span>        | <span data-ttu-id="ce06e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ce06e-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="ce06e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce06e-122">Authorization</span></span> | <span data-ttu-id="ce06e-123">Bearer {token} (erforderlich)</span><span class="sxs-lookup"><span data-stu-id="ce06e-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ce06e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce06e-124">Content-Type</span></span>  | <span data-ttu-id="ce06e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce06e-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="ce06e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce06e-126">Request body</span></span>

<span data-ttu-id="ce06e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce06e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce06e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce06e-128">Response</span></span>

<span data-ttu-id="ce06e-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce06e-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce06e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce06e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ce06e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce06e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="ce06e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce06e-132">Response</span></span>

<span data-ttu-id="ce06e-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ce06e-133">Here is an example of the response.</span></span> <span data-ttu-id="ce06e-134">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ce06e-134">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
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
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
