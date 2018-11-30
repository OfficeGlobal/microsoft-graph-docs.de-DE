---
title: domainNameReferences auflisten
description: Dient zum Abrufen einer Liste von directoryObject-Objekten mit einem Verweis auf die Domäne. Die zurückgegebene Liste enthält alle Directory-Objekte, die von der Domäne abhängig sind.
ms.openlocfilehash: a79655a65f0560da12250c6b637aca8540fab643
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018420"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="3878f-104">domainNameReferences auflisten</span><span class="sxs-lookup"><span data-stu-id="3878f-104">List domainNameReferences</span></span>

<span data-ttu-id="3878f-p102">Dient zum Abrufen einer Liste von [directoryObject](../resources/directoryobject.md)-Objekten mit einem Verweis auf die Domäne. Die zurückgegebene Liste enthält alle Directory-Objekte, die von der Domäne abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="3878f-p102">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="3878f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3878f-107">Permissions</span></span>

<span data-ttu-id="3878f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3878f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3878f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3878f-110">Permission type</span></span>      | <span data-ttu-id="3878f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3878f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3878f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3878f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3878f-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3878f-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="3878f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3878f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3878f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3878f-115">Not supported.</span></span>    |
|<span data-ttu-id="3878f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3878f-116">Application</span></span> | <span data-ttu-id="3878f-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3878f-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3878f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3878f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="3878f-119">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="3878f-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3878f-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3878f-120">Optional query parameters</span></span>

<span data-ttu-id="3878f-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3878f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3878f-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3878f-122">Request headers</span></span>

| <span data-ttu-id="3878f-123">Name</span><span class="sxs-lookup"><span data-stu-id="3878f-123">Name</span></span>      |<span data-ttu-id="3878f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3878f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3878f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3878f-125">Authorization</span></span>  | <span data-ttu-id="3878f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3878f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3878f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3878f-128">Request body</span></span>

<span data-ttu-id="3878f-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3878f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3878f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3878f-130">Response</span></span>

<span data-ttu-id="3878f-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3878f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3878f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3878f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3878f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3878f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="3878f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3878f-134">Response</span></span>
<span data-ttu-id="3878f-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3878f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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