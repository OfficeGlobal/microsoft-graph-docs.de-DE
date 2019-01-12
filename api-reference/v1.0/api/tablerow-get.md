---
title: TableRow abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des tableRow-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 849f7348773060a4d3a572e1be4f89b1fa470f00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936816"
---
# <a name="get-tablerow"></a><span data-ttu-id="87cc0-103">TableRow abrufen</span><span class="sxs-lookup"><span data-stu-id="87cc0-103">Get TableRow</span></span>

<span data-ttu-id="87cc0-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des tableRow-Objekts.</span><span class="sxs-lookup"><span data-stu-id="87cc0-104">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87cc0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87cc0-105">Permissions</span></span>
<span data-ttu-id="87cc0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87cc0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87cc0-108">Permission type</span></span>      | <span data-ttu-id="87cc0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87cc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87cc0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87cc0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87cc0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87cc0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87cc0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87cc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87cc0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87cc0-113">Not supported.</span></span>    |
|<span data-ttu-id="87cc0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87cc0-114">Application</span></span> | <span data-ttu-id="87cc0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87cc0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87cc0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87cc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87cc0-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87cc0-117">Optional query parameters</span></span>
<span data-ttu-id="87cc0-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87cc0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87cc0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87cc0-119">Request headers</span></span>
| <span data-ttu-id="87cc0-120">Name</span><span class="sxs-lookup"><span data-stu-id="87cc0-120">Name</span></span>      |<span data-ttu-id="87cc0-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87cc0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87cc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87cc0-122">Authorization</span></span>  | <span data-ttu-id="87cc0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87cc0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87cc0-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="87cc0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="87cc0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="87cc0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87cc0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87cc0-128">Request body</span></span>
<span data-ttu-id="87cc0-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87cc0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87cc0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="87cc0-130">Response</span></span>

<span data-ttu-id="87cc0-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und [WorkbookTableRow](../resources/tablerow.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="87cc0-131">If successful, this method returns a `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87cc0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87cc0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87cc0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87cc0-133">Request</span></span>
<span data-ttu-id="87cc0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87cc0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```
##### <a name="response"></a><span data-ttu-id="87cc0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="87cc0-135">Response</span></span>
<span data-ttu-id="87cc0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87cc0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
