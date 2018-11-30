---
title: Domänen auflisten
description: Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.
ms.openlocfilehash: 51c9e4035c44567589ba2f9c7b86453e48db6a9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017196"
---
# <a name="list-domains"></a><span data-ttu-id="e82f8-103">Domänen auflisten</span><span class="sxs-lookup"><span data-stu-id="e82f8-103">List domains</span></span>

<span data-ttu-id="e82f8-104">Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="e82f8-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e82f8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e82f8-105">Permissions</span></span>
<span data-ttu-id="e82f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e82f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e82f8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e82f8-108">Permission type</span></span>      | <span data-ttu-id="e82f8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e82f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e82f8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e82f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e82f8-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e82f8-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="e82f8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e82f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e82f8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e82f8-113">Not supported.</span></span>    |
|<span data-ttu-id="e82f8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e82f8-114">Application</span></span> | <span data-ttu-id="e82f8-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e82f8-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e82f8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e82f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e82f8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e82f8-117">Optional query parameters</span></span>
<span data-ttu-id="e82f8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e82f8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e82f8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e82f8-119">Request headers</span></span>
| <span data-ttu-id="e82f8-120">Name</span><span class="sxs-lookup"><span data-stu-id="e82f8-120">Name</span></span>      |<span data-ttu-id="e82f8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e82f8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e82f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e82f8-122">Authorization</span></span>  | <span data-ttu-id="e82f8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e82f8-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e82f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e82f8-125">Accept</span></span>         | <span data-ttu-id="e82f8-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="e82f8-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="e82f8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e82f8-127">Request body</span></span>
<span data-ttu-id="e82f8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e82f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e82f8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e82f8-129">Response</span></span>

<span data-ttu-id="e82f8-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domain](../resources/domain.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e82f8-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e82f8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e82f8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e82f8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e82f8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="e82f8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e82f8-133">Response</span></span>
<span data-ttu-id="e82f8-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e82f8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->