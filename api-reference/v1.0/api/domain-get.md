---
title: Domäne abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.
ms.openlocfilehash: ab446db054d2bb8bdb6cd18ccb41879988e6d30c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017194"
---
# <a name="get-domain"></a><span data-ttu-id="2081c-103">Domäne abrufen</span><span class="sxs-lookup"><span data-stu-id="2081c-103">Get domain</span></span>

<span data-ttu-id="2081c-104">Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="2081c-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2081c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2081c-105">Permissions</span></span>

<span data-ttu-id="2081c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2081c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2081c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2081c-108">Permission type</span></span>      | <span data-ttu-id="2081c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2081c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2081c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2081c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2081c-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2081c-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="2081c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2081c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2081c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2081c-113">Not supported.</span></span>    |
|<span data-ttu-id="2081c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2081c-114">Application</span></span> | <span data-ttu-id="2081c-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2081c-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2081c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2081c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="2081c-117">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="2081c-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2081c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2081c-118">Optional query parameters</span></span>

<span data-ttu-id="2081c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2081c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2081c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2081c-120">Request headers</span></span>

| <span data-ttu-id="2081c-121">Name</span><span class="sxs-lookup"><span data-stu-id="2081c-121">Name</span></span>      |<span data-ttu-id="2081c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2081c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2081c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2081c-123">Authorization</span></span>  | <span data-ttu-id="2081c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2081c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2081c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2081c-126">Content-Type</span></span>  | <span data-ttu-id="2081c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2081c-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2081c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2081c-128">Request body</span></span>
<span data-ttu-id="2081c-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2081c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2081c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2081c-130">Response</span></span>

<span data-ttu-id="2081c-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2081c-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2081c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2081c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2081c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2081c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="2081c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2081c-134">Response</span></span>
<span data-ttu-id="2081c-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2081c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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