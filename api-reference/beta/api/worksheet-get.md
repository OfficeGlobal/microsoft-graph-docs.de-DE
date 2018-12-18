---
title: Arbeitsblatt abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des worksheet-Objekts.
author: lumine2008
ms.openlocfilehash: dbf6cd6f00c746c1c0f95f4aee07986d6eb87a7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345808"
---
# <a name="get-worksheet"></a><span data-ttu-id="e2f63-103">Arbeitsblatt abrufen</span><span class="sxs-lookup"><span data-stu-id="e2f63-103">Get Worksheet</span></span>

> <span data-ttu-id="e2f63-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2f63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2f63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2f63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2f63-106">Dient zum Abrufen der Eigenschaften und der Beziehungen des worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e2f63-106">Retrieve the properties and relationships of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2f63-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2f63-107">Permissions</span></span>
<span data-ttu-id="e2f63-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2f63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2f63-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2f63-110">Permission type</span></span>      | <span data-ttu-id="e2f63-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2f63-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2f63-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2f63-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2f63-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2f63-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2f63-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2f63-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2f63-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2f63-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2f63-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2f63-116">Application</span></span> | <span data-ttu-id="e2f63-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2f63-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2f63-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2f63-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2f63-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e2f63-119">Optional query parameters</span></span>
<span data-ttu-id="e2f63-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2f63-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2f63-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2f63-121">Request headers</span></span>
| <span data-ttu-id="e2f63-122">Name</span><span class="sxs-lookup"><span data-stu-id="e2f63-122">Name</span></span>      |<span data-ttu-id="e2f63-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2f63-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2f63-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2f63-124">Authorization</span></span>  | <span data-ttu-id="e2f63-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2f63-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2f63-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e2f63-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="e2f63-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e2f63-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2f63-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2f63-130">Request body</span></span>
<span data-ttu-id="e2f63-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2f63-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2f63-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2f63-132">Response</span></span>

<span data-ttu-id="e2f63-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Worksheet](../resources/worksheet.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2f63-133">If successful, this method returns a `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2f63-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2f63-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2f63-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2f63-135">Request</span></span>
<span data-ttu-id="e2f63-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2f63-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheet"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
```
##### <a name="response"></a><span data-ttu-id="e2f63-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2f63-137">Response</span></span>
<span data-ttu-id="e2f63-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2f63-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->