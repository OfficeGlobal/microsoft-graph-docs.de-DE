---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19155801297caf56a9ba944b4220c4ba8db0bb36
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526718"
---
# <a name="range-boundingrect"></a><span data-ttu-id="06417-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="06417-103">Range: BoundingRect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06417-p101">Ruft das kleinste Bereichsobjekt ab, das die angegebenen Bereiche umfasst. Beispielsweise das GetBoundingRect von "B2:C5" und "D10:E15" lautet "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="06417-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="06417-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06417-106">Permissions</span></span>
<span data-ttu-id="06417-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06417-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06417-109">Permission type</span></span>      | <span data-ttu-id="06417-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06417-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06417-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06417-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06417-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06417-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06417-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06417-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06417-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06417-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06417-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06417-115">Application</span></span> | <span data-ttu-id="06417-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06417-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06417-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06417-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="06417-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06417-118">Request headers</span></span>
| <span data-ttu-id="06417-119">Name</span><span class="sxs-lookup"><span data-stu-id="06417-119">Name</span></span>       | <span data-ttu-id="06417-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06417-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06417-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06417-121">Authorization</span></span>  | <span data-ttu-id="06417-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06417-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06417-124">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="06417-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="06417-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="06417-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06417-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06417-127">Request body</span></span>
<span data-ttu-id="06417-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="06417-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06417-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="06417-129">Parameter</span></span>    | <span data-ttu-id="06417-130">Typ</span><span class="sxs-lookup"><span data-stu-id="06417-130">Type</span></span>   |<span data-ttu-id="06417-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06417-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06417-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="06417-132">anotherRange</span></span>|<span data-ttu-id="06417-133">string</span><span class="sxs-lookup"><span data-stu-id="06417-133">string</span></span>|<span data-ttu-id="06417-134">Das Bereichsobjekt oder die Adresse oder der Bereichsname.</span><span class="sxs-lookup"><span data-stu-id="06417-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="06417-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="06417-135">Response</span></span>

<span data-ttu-id="06417-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06417-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06417-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06417-137">Example</span></span>
<span data-ttu-id="06417-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="06417-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06417-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06417-139">Request</span></span>
<span data-ttu-id="06417-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06417-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="06417-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="06417-141">Response</span></span>
<span data-ttu-id="06417-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06417-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-boundingrect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
