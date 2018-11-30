---
title: Buckets auflisten
description: Dient zum Abrufen einer Liste von **plannerbucket**-Objekten.
ms.openlocfilehash: 8010a8ac283aa93f1a00ff505143ec6f6eec76c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019979"
---
# <a name="list-buckets"></a><span data-ttu-id="748cb-103">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="748cb-103">List buckets</span></span>

<span data-ttu-id="748cb-104">Dient zum Abrufen einer Liste von **plannerbucket**-Objekten.</span><span class="sxs-lookup"><span data-stu-id="748cb-104">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="748cb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="748cb-105">Permissions</span></span>
<span data-ttu-id="748cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="748cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="748cb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="748cb-108">Permission type</span></span>      | <span data-ttu-id="748cb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="748cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="748cb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="748cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="748cb-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="748cb-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="748cb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="748cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="748cb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="748cb-113">Not supported.</span></span>    |
|<span data-ttu-id="748cb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="748cb-114">Application</span></span> | <span data-ttu-id="748cb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="748cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="748cb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="748cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="748cb-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="748cb-117">Optional query parameters</span></span>
<span data-ttu-id="748cb-118">Für diese Methode müssen [Filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) für planID angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="748cb-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="748cb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="748cb-119">Request headers</span></span>
| <span data-ttu-id="748cb-120">Name</span><span class="sxs-lookup"><span data-stu-id="748cb-120">Name</span></span>      |<span data-ttu-id="748cb-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="748cb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="748cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="748cb-122">Authorization</span></span>  | <span data-ttu-id="748cb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="748cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="748cb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="748cb-125">Request body</span></span>
<span data-ttu-id="748cb-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="748cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="748cb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="748cb-127">Response</span></span>

<span data-ttu-id="748cb-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerBucket](../resources/plannerbucket.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="748cb-128">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="748cb-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="748cb-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="748cb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="748cb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="748cb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="748cb-133">Request</span></span>
<span data-ttu-id="748cb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="748cb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="748cb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="748cb-135">Response</span></span>
<span data-ttu-id="748cb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="748cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->