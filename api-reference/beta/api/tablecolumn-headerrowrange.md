---
title: 'TableColumn: HeaderRowRange'
description: Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 147e12d3fb8dd26a194b1210b91e5b5d4bbb22ab
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522231"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="ae4f0-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="ae4f0-103">TableColumn: HeaderRowRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae4f0-104">Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae4f0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae4f0-105">Permissions</span></span>
<span data-ttu-id="ae4f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae4f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae4f0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae4f0-108">Permission type</span></span>      | <span data-ttu-id="ae4f0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae4f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae4f0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae4f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae4f0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae4f0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae4f0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae4f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae4f0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae4f0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae4f0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae4f0-114">Application</span></span> | <span data-ttu-id="ae4f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae4f0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae4f0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae4f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="ae4f0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae4f0-117">Request headers</span></span>
| <span data-ttu-id="ae4f0-118">Name</span><span class="sxs-lookup"><span data-stu-id="ae4f0-118">Name</span></span>       | <span data-ttu-id="ae4f0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae4f0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae4f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae4f0-120">Authorization</span></span>  | <span data-ttu-id="ae4f0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae4f0-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ae4f0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae4f0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae4f0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae4f0-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ae4f0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae4f0-127">Response</span></span>

<span data-ttu-id="ae4f0-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae4f0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae4f0-129">Example</span></span>
<span data-ttu-id="ae4f0-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae4f0-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae4f0-131">Request</span></span>
<span data-ttu-id="ae4f0-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="ae4f0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae4f0-133">Response</span></span>
<span data-ttu-id="ae4f0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae4f0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-headerrowrange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
