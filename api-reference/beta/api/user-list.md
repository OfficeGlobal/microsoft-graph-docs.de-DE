---
title: Benutzer auflisten
description: Dient zum Abrufen einer Liste von Benutzerobjekten.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 48b63f5a9ccc3616bd8ecee986cbf26dfedfb8d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890531"
---
# <a name="list-users"></a><span data-ttu-id="6cfa9-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="6cfa9-103">List users</span></span>

> <span data-ttu-id="6cfa9-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cfa9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cfa9-106">Mit dieser API können Sie eine Liste von Benutzerobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-106">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cfa9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6cfa9-107">Permissions</span></span>

<span data-ttu-id="6cfa9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cfa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cfa9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6cfa9-110">Permission type</span></span>      | <span data-ttu-id="6cfa9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6cfa9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cfa9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6cfa9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6cfa9-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cfa9-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6cfa9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6cfa9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cfa9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cfa9-115">Not supported.</span></span>    |
|<span data-ttu-id="6cfa9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6cfa9-116">Application</span></span> | <span data-ttu-id="6cfa9-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cfa9-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cfa9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cfa9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cfa9-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6cfa9-119">Optional query parameters</span></span>

<span data-ttu-id="6cfa9-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cfa9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6cfa9-121">Request headers</span></span>
| <span data-ttu-id="6cfa9-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6cfa9-122">Header</span></span>        | <span data-ttu-id="6cfa9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6cfa9-123">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="6cfa9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cfa9-124">Authorization</span></span> | <span data-ttu-id="6cfa9-125">Bearer {token} (erforderlich)</span><span class="sxs-lookup"><span data-stu-id="6cfa9-125">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="6cfa9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cfa9-126">Content-Type</span></span>  | <span data-ttu-id="6cfa9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6cfa9-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="6cfa9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6cfa9-128">Request body</span></span>

<span data-ttu-id="6cfa9-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cfa9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cfa9-130">Response</span></span>

<span data-ttu-id="6cfa9-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cfa9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6cfa9-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6cfa9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cfa9-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="6cfa9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cfa9-134">Response</span></span>

<span data-ttu-id="6cfa9-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-135">Here is an example of the response.</span></span> <span data-ttu-id="6cfa9-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="6cfa9-136">Note: The response object shown here may be truncated for brevity.</span></span> 

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
