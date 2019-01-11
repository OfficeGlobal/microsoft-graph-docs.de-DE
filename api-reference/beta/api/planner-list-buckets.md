---
title: Buckets auflisten
description: Dient zum Abrufen einer Liste von **plannerbucket**-Objekten.
localization_priority: Normal
ms.openlocfilehash: 0dcf8e50351a0f1ec3d7238d6e6ba8d30bb35ddc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861327"
---
# <a name="list-buckets"></a><span data-ttu-id="39a12-103">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="39a12-103">List buckets</span></span>

> <span data-ttu-id="39a12-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="39a12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39a12-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39a12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39a12-106">Dient zum Abrufen einer Liste von **plannerbucket**-Objekten.</span><span class="sxs-lookup"><span data-stu-id="39a12-106">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="39a12-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39a12-107">Permissions</span></span>
<span data-ttu-id="39a12-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39a12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39a12-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39a12-110">Permission type</span></span>      | <span data-ttu-id="39a12-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39a12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39a12-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39a12-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39a12-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39a12-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="39a12-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39a12-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39a12-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39a12-115">Not supported.</span></span>    |
|<span data-ttu-id="39a12-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39a12-116">Application</span></span> | <span data-ttu-id="39a12-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39a12-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39a12-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a12-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="39a12-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="39a12-119">Optional query parameters</span></span>
<span data-ttu-id="39a12-120">Für diese Methode müssen [Filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) für planID angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="39a12-120">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39a12-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39a12-121">Request headers</span></span>
| <span data-ttu-id="39a12-122">Name</span><span class="sxs-lookup"><span data-stu-id="39a12-122">Name</span></span>      |<span data-ttu-id="39a12-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39a12-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39a12-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="39a12-124">Authorization</span></span>  | <span data-ttu-id="39a12-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39a12-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39a12-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39a12-127">Request body</span></span>
<span data-ttu-id="39a12-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="39a12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39a12-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a12-129">Response</span></span>

<span data-ttu-id="39a12-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerBucket](../resources/plannerbucket.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39a12-130">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="39a12-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="39a12-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="39a12-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39a12-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39a12-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a12-135">Request</span></span>
<span data-ttu-id="39a12-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39a12-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="39a12-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a12-137">Response</span></span>
<span data-ttu-id="39a12-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39a12-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
