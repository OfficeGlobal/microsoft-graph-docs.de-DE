---
title: Vereinbarungen zur Liste
description: Abrufen einer Liste von Vereinbarung-Objekten.
localization_priority: Normal
ms.openlocfilehash: 3ae255a386986b5627aed99f29dca5bfb9934e30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859920"
---
# <a name="list-agreements"></a><span data-ttu-id="ffbe5-103">Vereinbarungen zur Liste</span><span class="sxs-lookup"><span data-stu-id="ffbe5-103">List agreements</span></span>

> <span data-ttu-id="ffbe5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffbe5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ffbe5-106">Abrufen einer Liste von [Vereinbarung](../resources/agreement.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-106">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffbe5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ffbe5-107">Permissions</span></span>
<span data-ttu-id="ffbe5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffbe5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffbe5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffbe5-110">Permission type</span></span>                        | <span data-ttu-id="ffbe5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffbe5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffbe5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffbe5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffbe5-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffbe5-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="ffbe5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffbe5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffbe5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffbe5-115">Not supported.</span></span> |
|<span data-ttu-id="ffbe5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffbe5-116">Application</span></span>                            | <span data-ttu-id="ffbe5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffbe5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffbe5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffbe5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="ffbe5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffbe5-119">Request headers</span></span>
| <span data-ttu-id="ffbe5-120">Name</span><span class="sxs-lookup"><span data-stu-id="ffbe5-120">Name</span></span>         | <span data-ttu-id="ffbe5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ffbe5-121">Type</span></span>        | <span data-ttu-id="ffbe5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffbe5-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ffbe5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffbe5-123">Authorization</span></span> | <span data-ttu-id="ffbe5-124">string</span><span class="sxs-lookup"><span data-stu-id="ffbe5-124">string</span></span> | <span data-ttu-id="ffbe5-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-125">Bearer \{token\}.</span></span> <span data-ttu-id="ffbe5-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffbe5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffbe5-127">Request body</span></span>
<span data-ttu-id="ffbe5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ffbe5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffbe5-129">Response</span></span>
<span data-ttu-id="ffbe5-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Vereinbarung](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="ffbe5-130">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ffbe5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffbe5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffbe5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffbe5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="ffbe5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffbe5-133">Response</span></span>
><span data-ttu-id="ffbe5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ffbe5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
