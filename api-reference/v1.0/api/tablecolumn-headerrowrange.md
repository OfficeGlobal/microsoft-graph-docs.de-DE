---
title: 'TableColumn: HeaderRowRange'
description: Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2588ae415866d1d68d3edf605aade1f1ca76f667
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858758"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="5f91c-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="5f91c-103">TableColumn: HeaderRowRange</span></span>

<span data-ttu-id="5f91c-104">Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="5f91c-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f91c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5f91c-105">Permissions</span></span>
<span data-ttu-id="5f91c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f91c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f91c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f91c-108">Permission type</span></span>      | <span data-ttu-id="5f91c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f91c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f91c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f91c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f91c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f91c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f91c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f91c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f91c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f91c-113">Not supported.</span></span>    |
|<span data-ttu-id="5f91c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f91c-114">Application</span></span> | <span data-ttu-id="5f91c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f91c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f91c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f91c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="5f91c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f91c-117">Request headers</span></span>
| <span data-ttu-id="5f91c-118">Name</span><span class="sxs-lookup"><span data-stu-id="5f91c-118">Name</span></span>       | <span data-ttu-id="5f91c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f91c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5f91c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f91c-120">Authorization</span></span>  | <span data-ttu-id="5f91c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f91c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f91c-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5f91c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5f91c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5f91c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f91c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f91c-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5f91c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f91c-127">Response</span></span>

<span data-ttu-id="5f91c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f91c-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f91c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f91c-129">Example</span></span>
<span data-ttu-id="5f91c-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5f91c-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f91c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f91c-131">Request</span></span>
<span data-ttu-id="5f91c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f91c-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="5f91c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f91c-133">Response</span></span>
<span data-ttu-id="5f91c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f91c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
