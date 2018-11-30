---
title: RangeFormat abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.
ms.openlocfilehash: a91adf741299b9d74a41f46359119866429085ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063161"
---
# <a name="get-rangeformat"></a><span data-ttu-id="54a3f-103">RangeFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="54a3f-103">Get RangeFormat</span></span>

> <span data-ttu-id="54a3f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54a3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54a3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54a3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54a3f-106">Dient zum Abrufen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="54a3f-106">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54a3f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="54a3f-107">Permissions</span></span>
<span data-ttu-id="54a3f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54a3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54a3f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54a3f-110">Permission type</span></span>      | <span data-ttu-id="54a3f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54a3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54a3f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54a3f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54a3f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54a3f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="54a3f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54a3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54a3f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54a3f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="54a3f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54a3f-116">Application</span></span> | <span data-ttu-id="54a3f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54a3f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54a3f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54a3f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54a3f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="54a3f-119">Optional query parameters</span></span>
<span data-ttu-id="54a3f-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="54a3f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54a3f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54a3f-121">Request headers</span></span>
| <span data-ttu-id="54a3f-122">Name</span><span class="sxs-lookup"><span data-stu-id="54a3f-122">Name</span></span>      |<span data-ttu-id="54a3f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54a3f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54a3f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54a3f-124">Authorization</span></span>  | <span data-ttu-id="54a3f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="54a3f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54a3f-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="54a3f-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="54a3f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="54a3f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54a3f-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54a3f-130">Request body</span></span>
<span data-ttu-id="54a3f-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="54a3f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54a3f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="54a3f-132">Response</span></span>

<span data-ttu-id="54a3f-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFormat](../resources/rangeformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54a3f-133">If successful, this method returns a `200 OK` response code and [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54a3f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54a3f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54a3f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54a3f-135">Request</span></span>
<span data-ttu-id="54a3f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54a3f-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format
```
##### <a name="response"></a><span data-ttu-id="54a3f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="54a3f-137">Response</span></span>
<span data-ttu-id="54a3f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54a3f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->