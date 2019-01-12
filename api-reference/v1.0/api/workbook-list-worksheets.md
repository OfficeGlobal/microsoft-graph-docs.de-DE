---
title: Arbeitsblätter auflisten
description: Dient zum Abrufen einer Liste von Arbeitsblattobjekten.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dc460f702089496f3de46aaca45b4b1b3ff49d58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980580"
---
# <a name="list-worksheets"></a><span data-ttu-id="bb993-103">Arbeitsblätter auflisten</span><span class="sxs-lookup"><span data-stu-id="bb993-103">List worksheets</span></span>

<span data-ttu-id="bb993-104">Dient zum Abrufen einer Liste von Arbeitsblattobjekten.</span><span class="sxs-lookup"><span data-stu-id="bb993-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb993-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb993-105">Permissions</span></span>
<span data-ttu-id="bb993-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb993-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb993-108">Permission type</span></span>      | <span data-ttu-id="bb993-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb993-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb993-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb993-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb993-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb993-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb993-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb993-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb993-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb993-113">Not supported.</span></span>    |
|<span data-ttu-id="bb993-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb993-114">Application</span></span> | <span data-ttu-id="bb993-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb993-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb993-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb993-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb993-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bb993-117">Optional query parameters</span></span>
<span data-ttu-id="bb993-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bb993-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb993-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb993-119">Request headers</span></span>
| <span data-ttu-id="bb993-120">Name</span><span class="sxs-lookup"><span data-stu-id="bb993-120">Name</span></span>      |<span data-ttu-id="bb993-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb993-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb993-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb993-122">Authorization</span></span>  | <span data-ttu-id="bb993-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb993-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb993-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="bb993-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb993-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="bb993-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb993-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb993-128">Request body</span></span>
<span data-ttu-id="bb993-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb993-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb993-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb993-130">Response</span></span>

<span data-ttu-id="bb993-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [WorkbookWorksheet](../resources/worksheet.md) .</span><span class="sxs-lookup"><span data-stu-id="bb993-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb993-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb993-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb993-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb993-133">Request</span></span>
<span data-ttu-id="bb993-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb993-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="bb993-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb993-135">Response</span></span>
<span data-ttu-id="bb993-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb993-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
