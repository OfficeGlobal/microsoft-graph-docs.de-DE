---
title: Domäne abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 49458b87f86bc5a7dbf4d7d3c196736050b2d6aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813573"
---
# <a name="get-domain"></a><span data-ttu-id="aeac0-103">Domäne abrufen</span><span class="sxs-lookup"><span data-stu-id="aeac0-103">Get domain</span></span>

> <span data-ttu-id="aeac0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aeac0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeac0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aeac0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aeac0-106">Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="aeac0-106">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeac0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aeac0-107">Permissions</span></span>

<span data-ttu-id="aeac0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeac0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aeac0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aeac0-110">Permission type</span></span>      | <span data-ttu-id="aeac0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aeac0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aeac0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aeac0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aeac0-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeac0-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="aeac0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aeac0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aeac0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aeac0-115">Not supported.</span></span>    |
|<span data-ttu-id="aeac0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aeac0-116">Application</span></span> | <span data-ttu-id="aeac0-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeac0-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aeac0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aeac0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="aeac0-119">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="aeac0-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="aeac0-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aeac0-120">Optional query parameters</span></span>

<span data-ttu-id="aeac0-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aeac0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeac0-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aeac0-122">Request headers</span></span>

| <span data-ttu-id="aeac0-123">Name</span><span class="sxs-lookup"><span data-stu-id="aeac0-123">Name</span></span>      |<span data-ttu-id="aeac0-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aeac0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aeac0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeac0-125">Authorization</span></span>  | <span data-ttu-id="aeac0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aeac0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aeac0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aeac0-128">Content-Type</span></span>  | <span data-ttu-id="aeac0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="aeac0-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="aeac0-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aeac0-130">Request body</span></span>
<span data-ttu-id="aeac0-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aeac0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeac0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="aeac0-132">Response</span></span>

<span data-ttu-id="aeac0-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aeac0-133">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aeac0-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aeac0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aeac0-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aeac0-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="aeac0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="aeac0-136">Response</span></span>
<span data-ttu-id="aeac0-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aeac0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
