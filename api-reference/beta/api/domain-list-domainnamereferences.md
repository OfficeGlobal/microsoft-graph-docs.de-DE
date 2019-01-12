---
title: domainNameReferences auflisten
description: Dient zum Abrufen einer Liste von directoryObject-Objekten mit einem Verweis auf die Domäne. Die zurückgegebene Liste enthält alle Directory-Objekte, die von der Domäne abhängig sind.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2a0e2cdbfb4a7a0899650e884a190ea45855d72c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985368"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="9bbf4-104">domainNameReferences auflisten</span><span class="sxs-lookup"><span data-stu-id="9bbf4-104">List domainNameReferences</span></span>

> <span data-ttu-id="9bbf4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bbf4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bbf4-p103">Dient zum Abrufen einer Liste von [directoryObject](../resources/directoryobject.md)-Objekten mit einem Verweis auf die Domäne. Die zurückgegebene Liste enthält alle Directory-Objekte, die von der Domäne abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-p103">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bbf4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9bbf4-109">Permissions</span></span>

<span data-ttu-id="9bbf4-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bbf4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9bbf4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bbf4-112">Permission type</span></span>      | <span data-ttu-id="9bbf4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bbf4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bbf4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bbf4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9bbf4-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bbf4-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="9bbf4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bbf4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bbf4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bbf4-117">Not supported.</span></span>    |
|<span data-ttu-id="9bbf4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bbf4-118">Application</span></span> | <span data-ttu-id="9bbf4-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bbf4-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bbf4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bbf4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="9bbf4-121">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="9bbf4-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9bbf4-122">Optional query parameters</span></span>

<span data-ttu-id="9bbf4-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bbf4-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bbf4-124">Request headers</span></span>

| <span data-ttu-id="9bbf4-125">Name</span><span class="sxs-lookup"><span data-stu-id="9bbf4-125">Name</span></span>      |<span data-ttu-id="9bbf4-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bbf4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9bbf4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bbf4-127">Authorization</span></span>  | <span data-ttu-id="9bbf4-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bbf4-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bbf4-130">Request body</span></span>

<span data-ttu-id="9bbf4-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bbf4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bbf4-132">Response</span></span>

<span data-ttu-id="9bbf4-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bbf4-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bbf4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bbf4-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bbf4-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="9bbf4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bbf4-136">Response</span></span>
<span data-ttu-id="9bbf4-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bbf4-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
