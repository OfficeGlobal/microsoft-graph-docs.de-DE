---
title: Abrufen von WorksheetProtection
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a175eb5bf4804c294807428405255b7627e54a73
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577389"
---
# <a name="get-worksheetprotection"></a><span data-ttu-id="619dd-103">Abrufen von WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="619dd-103">Get WorksheetProtection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="619dd-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="619dd-104">Retrieve the properties and relationships of worksheetprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="619dd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="619dd-105">Permissions</span></span>
<span data-ttu-id="619dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="619dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="619dd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="619dd-108">Permission type</span></span>      | <span data-ttu-id="619dd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="619dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="619dd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="619dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="619dd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="619dd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="619dd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="619dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="619dd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="619dd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="619dd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="619dd-114">Application</span></span> | <span data-ttu-id="619dd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="619dd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="619dd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="619dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="619dd-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="619dd-117">Optional query parameters</span></span>
<span data-ttu-id="619dd-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="619dd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="619dd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="619dd-119">Request headers</span></span>
| <span data-ttu-id="619dd-120">Name</span><span class="sxs-lookup"><span data-stu-id="619dd-120">Name</span></span>      |<span data-ttu-id="619dd-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="619dd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="619dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="619dd-122">Authorization</span></span>  | <span data-ttu-id="619dd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="619dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="619dd-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="619dd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="619dd-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="619dd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="619dd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="619dd-128">Request body</span></span>
<span data-ttu-id="619dd-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="619dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="619dd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="619dd-130">Response</span></span>

<span data-ttu-id="619dd-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [WorksheetProtection](../resources/worksheetprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="619dd-131">If successful, this method returns a `200 OK` response code and [WorksheetProtection](../resources/worksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="619dd-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="619dd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="619dd-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="619dd-133">Request</span></span>
<span data-ttu-id="619dd-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="619dd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
##### <a name="response"></a><span data-ttu-id="619dd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="619dd-135">Response</span></span>
<span data-ttu-id="619dd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="619dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
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
<!--
{
  "type": "#page.annotation",
  "description": "Get WorksheetProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
