---
title: Abrufen von WorksheetProtection
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7fe61ce697f0d55dc456eee3a46279bdfdcbf0f8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982393"
---
# <a name="get-worksheetprotection"></a><span data-ttu-id="8c395-103">Abrufen von WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="8c395-103">Get WorksheetProtection</span></span>

> <span data-ttu-id="8c395-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c395-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c395-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c395-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c395-106">Dient zum Abrufen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c395-106">Retrieve the properties and relationships of worksheetprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c395-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8c395-107">Permissions</span></span>
<span data-ttu-id="8c395-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c395-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c395-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c395-110">Permission type</span></span>      | <span data-ttu-id="8c395-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c395-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c395-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c395-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c395-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c395-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c395-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c395-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c395-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c395-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c395-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c395-116">Application</span></span> | <span data-ttu-id="8c395-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c395-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c395-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c395-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c395-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8c395-119">Optional query parameters</span></span>
<span data-ttu-id="8c395-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c395-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c395-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c395-121">Request headers</span></span>
| <span data-ttu-id="8c395-122">Name</span><span class="sxs-lookup"><span data-stu-id="8c395-122">Name</span></span>      |<span data-ttu-id="8c395-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c395-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c395-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c395-124">Authorization</span></span>  | <span data-ttu-id="8c395-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c395-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c395-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8c395-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c395-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8c395-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c395-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c395-130">Request body</span></span>
<span data-ttu-id="8c395-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c395-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c395-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c395-132">Response</span></span>

<span data-ttu-id="8c395-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [WorksheetProtection](../resources/worksheetprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c395-133">If successful, this method returns a `200 OK` response code and [WorksheetProtection](../resources/worksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c395-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c395-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c395-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c395-135">Request</span></span>
<span data-ttu-id="8c395-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c395-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
##### <a name="response"></a><span data-ttu-id="8c395-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c395-137">Response</span></span>
<span data-ttu-id="8c395-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c395-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheetProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 23

{
  "protected": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get WorksheetProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
