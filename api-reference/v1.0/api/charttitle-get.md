---
title: ChartTitle abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartTitle-Objekts.
ms.openlocfilehash: b338b46a77e153a500277f762b6f2792453d1505
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019489"
---
# <a name="get-charttitle"></a><span data-ttu-id="9f082-103">ChartTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="9f082-103">Get ChartTitle</span></span>

<span data-ttu-id="9f082-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9f082-104">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f082-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f082-105">Permissions</span></span>
<span data-ttu-id="9f082-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f082-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f082-108">Permission type</span></span>      | <span data-ttu-id="9f082-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f082-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f082-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f082-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f082-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f082-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f082-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f082-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f082-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f082-113">Not supported.</span></span>    |
|<span data-ttu-id="9f082-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f082-114">Application</span></span> | <span data-ttu-id="9f082-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f082-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f082-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f082-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f082-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9f082-117">Optional query parameters</span></span>
<span data-ttu-id="9f082-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f082-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f082-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f082-119">Request headers</span></span>
| <span data-ttu-id="9f082-120">Name</span><span class="sxs-lookup"><span data-stu-id="9f082-120">Name</span></span>      |<span data-ttu-id="9f082-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f082-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f082-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f082-122">Authorization</span></span>  | <span data-ttu-id="9f082-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f082-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f082-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9f082-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f082-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9f082-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f082-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f082-128">Request body</span></span>
<span data-ttu-id="9f082-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f082-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f082-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f082-130">Response</span></span>

<span data-ttu-id="9f082-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und [WorkbookChartTitle](../resources/charttitle.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9f082-131">If successful, this method returns a `200 OK` response code and [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f082-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f082-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f082-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f082-133">Request</span></span>
<span data-ttu-id="9f082-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f082-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
##### <a name="response"></a><span data-ttu-id="9f082-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f082-135">Response</span></span>
<span data-ttu-id="9f082-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f082-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->