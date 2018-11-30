---
title: Rahmen auflisten
description: Dient zum Abrufen einer Liste von rangeborder-Objekten.
ms.openlocfilehash: 26648b7d713b76a6f5d4d5171d2f20a0816a0dc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063669"
---
# <a name="list-borders"></a><span data-ttu-id="1f515-103">Rahmen auflisten</span><span class="sxs-lookup"><span data-stu-id="1f515-103">List borders</span></span>

> <span data-ttu-id="1f515-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f515-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f515-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f515-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f515-106">Dient zum Abrufen einer Liste von rangeborder-Objekten.</span><span class="sxs-lookup"><span data-stu-id="1f515-106">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f515-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f515-107">Permissions</span></span>
<span data-ttu-id="1f515-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f515-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f515-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f515-110">Permission type</span></span>      | <span data-ttu-id="1f515-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f515-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f515-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f515-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1f515-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f515-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f515-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f515-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f515-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f515-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f515-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f515-116">Application</span></span> | <span data-ttu-id="1f515-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f515-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f515-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f515-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f515-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1f515-119">Optional query parameters</span></span>
<span data-ttu-id="1f515-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f515-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f515-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f515-121">Request headers</span></span>
| <span data-ttu-id="1f515-122">Name</span><span class="sxs-lookup"><span data-stu-id="1f515-122">Name</span></span>      |<span data-ttu-id="1f515-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f515-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f515-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f515-124">Authorization</span></span>  | <span data-ttu-id="1f515-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f515-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f515-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1f515-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f515-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1f515-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f515-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f515-130">Request body</span></span>
<span data-ttu-id="1f515-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f515-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f515-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f515-132">Response</span></span>

<span data-ttu-id="1f515-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [RangeBorder](../resources/rangeborder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f515-133">If successful, this method returns a `200 OK` response code and collection of [RangeBorder](../resources/rangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f515-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f515-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f515-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f515-135">Request</span></span>
<span data-ttu-id="1f515-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f515-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
```
##### <a name="response"></a><span data-ttu-id="1f515-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f515-137">Response</span></span>
<span data-ttu-id="1f515-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f515-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->