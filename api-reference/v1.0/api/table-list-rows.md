---
title: Zeilen auflisten
description: Dient zum Abrufen einer Liste von tablerow-Objekten.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 974d22b8a6118ee3b50c9e765facc06c9e7b496a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923775"
---
# <a name="list-rows"></a><span data-ttu-id="b8d03-103">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="b8d03-103">List rows</span></span>

<span data-ttu-id="b8d03-104">Dient zum Abrufen einer Liste von tablerow-Objekten.</span><span class="sxs-lookup"><span data-stu-id="b8d03-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8d03-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8d03-105">Permissions</span></span>
<span data-ttu-id="b8d03-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d03-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8d03-108">Permission type</span></span>      | <span data-ttu-id="b8d03-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8d03-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8d03-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8d03-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8d03-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8d03-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b8d03-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8d03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8d03-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8d03-113">Not supported.</span></span>    |
|<span data-ttu-id="b8d03-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8d03-114">Application</span></span> | <span data-ttu-id="b8d03-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8d03-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8d03-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8d03-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8d03-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8d03-117">Optional query parameters</span></span>
<span data-ttu-id="b8d03-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8d03-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="b8d03-119">Verwenden Sie für zuverlässige Ergebnisse die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) zum Blättern durch die Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="b8d03-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="b8d03-120">Dies hilft, Leistungsprobleme im Zusammenhang mit großen Resultsets zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="b8d03-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8d03-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8d03-121">Request headers</span></span>
| <span data-ttu-id="b8d03-122">Name</span><span class="sxs-lookup"><span data-stu-id="b8d03-122">Name</span></span>      |<span data-ttu-id="b8d03-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8d03-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8d03-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d03-124">Authorization</span></span>  | <span data-ttu-id="b8d03-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8d03-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8d03-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b8d03-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="b8d03-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b8d03-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8d03-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8d03-130">Request body</span></span>
<span data-ttu-id="b8d03-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8d03-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8d03-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8d03-132">Response</span></span>

<span data-ttu-id="b8d03-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [WorkbookTableRow](../resources/tablerow.md) .</span><span class="sxs-lookup"><span data-stu-id="b8d03-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8d03-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8d03-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8d03-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8d03-135">Request</span></span>
<span data-ttu-id="b8d03-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8d03-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="b8d03-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8d03-137">Response</span></span>
<span data-ttu-id="b8d03-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8d03-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
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
> <span data-ttu-id="b8d03-141">
  \*\*Hinweis:\*\* Verwenden Sie die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) zum Blättern durch eine große Anzahl von Zeilen.</span><span class="sxs-lookup"><span data-stu-id="b8d03-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="b8d03-142">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="b8d03-142">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
