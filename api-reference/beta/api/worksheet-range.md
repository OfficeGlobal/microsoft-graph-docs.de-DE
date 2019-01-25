---
title: 'Arbeitsblatt: Range'
description: Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 81c88cd8cd454c5b31d143cd22f61412a77074c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530090"
---
# <a name="worksheet-range"></a><span data-ttu-id="9233a-103">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="9233a-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9233a-104">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="9233a-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="9233a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9233a-105">Permissions</span></span>
<span data-ttu-id="9233a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9233a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9233a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9233a-108">Permission type</span></span>      | <span data-ttu-id="9233a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9233a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9233a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9233a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9233a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9233a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9233a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9233a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9233a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9233a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9233a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9233a-114">Application</span></span> | <span data-ttu-id="9233a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9233a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9233a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9233a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="9233a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9233a-117">Request headers</span></span>
| <span data-ttu-id="9233a-118">Name</span><span class="sxs-lookup"><span data-stu-id="9233a-118">Name</span></span>       | <span data-ttu-id="9233a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9233a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9233a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9233a-120">Authorization</span></span>  | <span data-ttu-id="9233a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9233a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9233a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9233a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9233a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9233a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9233a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9233a-126">Request body</span></span>
<span data-ttu-id="9233a-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9233a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9233a-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="9233a-128">Parameter</span></span>    | <span data-ttu-id="9233a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9233a-129">Type</span></span>   |<span data-ttu-id="9233a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9233a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9233a-131">address</span><span class="sxs-lookup"><span data-stu-id="9233a-131">address</span></span>|<span data-ttu-id="9233a-132">string</span><span class="sxs-lookup"><span data-stu-id="9233a-132">string</span></span>|<span data-ttu-id="9233a-p104">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9233a-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="9233a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9233a-136">Response</span></span>

<span data-ttu-id="9233a-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9233a-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9233a-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9233a-138">Example</span></span>
<span data-ttu-id="9233a-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9233a-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9233a-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9233a-140">Request</span></span>
<span data-ttu-id="9233a-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9233a-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="9233a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="9233a-142">Response</span></span>
<span data-ttu-id="9233a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9233a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
