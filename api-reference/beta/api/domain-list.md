---
title: Domänen auflisten
description: Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2872ccc8e15bafc7f086d72d663a5bf68dfce86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964970"
---
# <a name="list-domains"></a><span data-ttu-id="94e3e-103">Domänen auflisten</span><span class="sxs-lookup"><span data-stu-id="94e3e-103">List domains</span></span>

> <span data-ttu-id="94e3e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94e3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94e3e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94e3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94e3e-106">Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="94e3e-106">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="94e3e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="94e3e-107">Permissions</span></span>
<span data-ttu-id="94e3e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e3e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94e3e-110">Permission type</span></span>      | <span data-ttu-id="94e3e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94e3e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94e3e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94e3e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94e3e-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e3e-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="94e3e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94e3e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94e3e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94e3e-115">Not supported.</span></span>    |
|<span data-ttu-id="94e3e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94e3e-116">Application</span></span> | <span data-ttu-id="94e3e-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e3e-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94e3e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94e3e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94e3e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="94e3e-119">Optional query parameters</span></span>
<span data-ttu-id="94e3e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94e3e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94e3e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94e3e-121">Request headers</span></span>
| <span data-ttu-id="94e3e-122">Name</span><span class="sxs-lookup"><span data-stu-id="94e3e-122">Name</span></span>      |<span data-ttu-id="94e3e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94e3e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94e3e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e3e-124">Authorization</span></span>  | <span data-ttu-id="94e3e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="94e3e-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="94e3e-127">Accept</span></span>         | <span data-ttu-id="94e3e-128">application/json;</span><span class="sxs-lookup"><span data-stu-id="94e3e-128">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="94e3e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94e3e-129">Request body</span></span>
<span data-ttu-id="94e3e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="94e3e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e3e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="94e3e-131">Response</span></span>

<span data-ttu-id="94e3e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domain](../resources/domain.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94e3e-132">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94e3e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94e3e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94e3e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94e3e-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
##### <a name="response"></a><span data-ttu-id="94e3e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="94e3e-135">Response</span></span>
<span data-ttu-id="94e3e-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94e3e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "name": "contoso.com",
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
