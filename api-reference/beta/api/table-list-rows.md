---
title: Zeilen auflisten
description: Dient zum Abrufen einer Liste von tablerow-Objekten.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d5edeb8027a7e6d75af2244fce988eac92c2edc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970150"
---
# <a name="list-rows"></a><span data-ttu-id="c8a40-103">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="c8a40-103">List rows</span></span>

> <span data-ttu-id="c8a40-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8a40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8a40-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8a40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8a40-106">Dient zum Abrufen einer Liste von tablerow-Objekten.</span><span class="sxs-lookup"><span data-stu-id="c8a40-106">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8a40-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8a40-107">Permissions</span></span>
<span data-ttu-id="c8a40-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8a40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8a40-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8a40-110">Permission type</span></span>      | <span data-ttu-id="c8a40-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8a40-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8a40-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8a40-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c8a40-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8a40-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8a40-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8a40-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8a40-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8a40-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8a40-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8a40-116">Application</span></span> | <span data-ttu-id="c8a40-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8a40-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8a40-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8a40-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8a40-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c8a40-119">Optional query parameters</span></span>
<span data-ttu-id="c8a40-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8a40-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="c8a40-121">Verwenden Sie für zuverlässige Ergebnisse die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) zum Blättern durch die Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="c8a40-121">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="c8a40-122">Dies hilft, Leistungsprobleme im Zusammenhang mit großen Resultsets zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="c8a40-122">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8a40-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8a40-123">Request headers</span></span>
| <span data-ttu-id="c8a40-124">Name</span><span class="sxs-lookup"><span data-stu-id="c8a40-124">Name</span></span>      |<span data-ttu-id="c8a40-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8a40-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8a40-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8a40-126">Authorization</span></span>  | <span data-ttu-id="c8a40-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8a40-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8a40-129">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c8a40-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8a40-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c8a40-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8a40-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8a40-132">Request body</span></span>
<span data-ttu-id="c8a40-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8a40-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8a40-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8a40-134">Response</span></span>

<span data-ttu-id="c8a40-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [TableRow](../resources/tablerow.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8a40-135">If successful, this method returns a `200 OK` response code and collection of [TableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8a40-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8a40-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8a40-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8a40-137">Request</span></span>
<span data-ttu-id="c8a40-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8a40-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="c8a40-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8a40-139">Response</span></span>
<span data-ttu-id="c8a40-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8a40-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="c8a40-143">
  \*\*Hinweis:\*\* Verwenden Sie die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) zum Blättern durch eine große Anzahl von Zeilen.</span><span class="sxs-lookup"><span data-stu-id="c8a40-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="c8a40-144">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c8a40-144">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
