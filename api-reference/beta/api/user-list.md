---
title: Benutzer auflisten
description: Dient zum Abrufen einer Liste von Benutzerobjekten.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 874ae4d3f54cfa67e6ac542cacab4b6eb39be716
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939511"
---
# <a name="list-users"></a><span data-ttu-id="3cf19-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="3cf19-103">List users</span></span>

> <span data-ttu-id="3cf19-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3cf19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cf19-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3cf19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3cf19-106">Mit dieser API können Sie eine Liste von Benutzerobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="3cf19-106">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf19-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3cf19-107">Permissions</span></span>

<span data-ttu-id="3cf19-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cf19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cf19-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3cf19-110">Permission type</span></span>      | <span data-ttu-id="3cf19-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3cf19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cf19-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3cf19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cf19-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cf19-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3cf19-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3cf19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf19-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cf19-115">Not supported.</span></span>    |
|<span data-ttu-id="3cf19-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3cf19-116">Application</span></span> | <span data-ttu-id="3cf19-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf19-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cf19-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cf19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cf19-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3cf19-119">Optional query parameters</span></span>

<span data-ttu-id="3cf19-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3cf19-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cf19-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3cf19-121">Request headers</span></span>
| <span data-ttu-id="3cf19-122">Header</span><span class="sxs-lookup"><span data-stu-id="3cf19-122">Header</span></span>        | <span data-ttu-id="3cf19-123">Wert</span><span class="sxs-lookup"><span data-stu-id="3cf19-123">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="3cf19-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cf19-124">Authorization</span></span> | <span data-ttu-id="3cf19-125">Bearer {token} (erforderlich)</span><span class="sxs-lookup"><span data-stu-id="3cf19-125">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="3cf19-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cf19-126">Content-Type</span></span>  | <span data-ttu-id="3cf19-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3cf19-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="3cf19-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3cf19-128">Request body</span></span>

<span data-ttu-id="3cf19-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3cf19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cf19-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cf19-130">Response</span></span>

<span data-ttu-id="3cf19-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3cf19-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf19-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3cf19-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3cf19-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cf19-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="3cf19-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cf19-134">Response</span></span>

<span data-ttu-id="3cf19-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3cf19-135">Here is an example of the response.</span></span> <span data-ttu-id="3cf19-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3cf19-136">Note: The response object shown here may be truncated for brevity.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
