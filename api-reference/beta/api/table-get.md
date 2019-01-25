---
title: Tabelle abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des Tabellenobjekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: faae44f86428b55aae24fb83a5d68f2ad1d3e562
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524422"
---
# <a name="get-table"></a><span data-ttu-id="3aebc-103">Tabelle abrufen</span><span class="sxs-lookup"><span data-stu-id="3aebc-103">Get Table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aebc-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des Tabellenobjekts.</span><span class="sxs-lookup"><span data-stu-id="3aebc-104">Retrieve the properties and relationships of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3aebc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3aebc-105">Permissions</span></span>
<span data-ttu-id="3aebc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aebc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3aebc-108">Permission type</span></span>      | <span data-ttu-id="3aebc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3aebc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aebc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3aebc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3aebc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aebc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3aebc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3aebc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aebc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aebc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3aebc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3aebc-114">Application</span></span> | <span data-ttu-id="3aebc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3aebc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aebc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3aebc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3aebc-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3aebc-117">Optional query parameters</span></span>
<span data-ttu-id="3aebc-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3aebc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aebc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3aebc-119">Request headers</span></span>
| <span data-ttu-id="3aebc-120">Name</span><span class="sxs-lookup"><span data-stu-id="3aebc-120">Name</span></span>      |<span data-ttu-id="3aebc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3aebc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3aebc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aebc-122">Authorization</span></span>  | <span data-ttu-id="3aebc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3aebc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aebc-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3aebc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3aebc-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3aebc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aebc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3aebc-128">Request body</span></span>
<span data-ttu-id="3aebc-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3aebc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aebc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3aebc-130">Response</span></span>

<span data-ttu-id="3aebc-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aebc-131">If successful, this method returns a `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3aebc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3aebc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3aebc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3aebc-133">Request</span></span>
<span data-ttu-id="3aebc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3aebc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_table"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
```
##### <a name="response"></a><span data-ttu-id="3aebc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3aebc-135">Response</span></span>
<span data-ttu-id="3aebc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aebc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
