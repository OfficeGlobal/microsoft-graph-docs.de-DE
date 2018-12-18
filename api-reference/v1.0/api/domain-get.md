---
title: Domäne abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.
author: lleonard-msft
ms.openlocfilehash: 6135f43ab305558c1ade7d9ec1bc27c9e5c4a043
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330065"
---
# <a name="get-domain"></a><span data-ttu-id="a0ee5-103">Domäne abrufen</span><span class="sxs-lookup"><span data-stu-id="a0ee5-103">Get domain</span></span>

<span data-ttu-id="a0ee5-104">Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0ee5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0ee5-105">Permissions</span></span>

<span data-ttu-id="a0ee5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ee5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a0ee5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0ee5-108">Permission type</span></span>      | <span data-ttu-id="a0ee5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0ee5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0ee5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0ee5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0ee5-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0ee5-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="a0ee5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0ee5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ee5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0ee5-113">Not supported.</span></span>    |
|<span data-ttu-id="a0ee5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0ee5-114">Application</span></span> | <span data-ttu-id="a0ee5-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ee5-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0ee5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0ee5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="a0ee5-117">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a0ee5-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a0ee5-118">Optional query parameters</span></span>

<span data-ttu-id="a0ee5-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0ee5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0ee5-120">Request headers</span></span>

| <span data-ttu-id="a0ee5-121">Name</span><span class="sxs-lookup"><span data-stu-id="a0ee5-121">Name</span></span>      |<span data-ttu-id="a0ee5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0ee5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0ee5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0ee5-123">Authorization</span></span>  | <span data-ttu-id="a0ee5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0ee5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0ee5-126">Content-Type</span></span>  | <span data-ttu-id="a0ee5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0ee5-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0ee5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0ee5-128">Request body</span></span>
<span data-ttu-id="a0ee5-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0ee5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0ee5-130">Response</span></span>

<span data-ttu-id="a0ee5-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0ee5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0ee5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0ee5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0ee5-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="a0ee5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0ee5-134">Response</span></span>
<span data-ttu-id="a0ee5-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0ee5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->