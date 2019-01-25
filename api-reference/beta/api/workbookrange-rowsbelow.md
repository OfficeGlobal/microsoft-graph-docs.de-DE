---
title: 'workbookRange: rowsBelow'
description: Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 42d53ce3aa9d26c7c499b19af3d5330259786520
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529474"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="b700b-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="b700b-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b700b-104">Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="b700b-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="b700b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b700b-105">Permissions</span></span>
<span data-ttu-id="b700b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b700b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b700b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b700b-108">Permission type</span></span>      | <span data-ttu-id="b700b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b700b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b700b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b700b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b700b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b700b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b700b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b700b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b700b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b700b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b700b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b700b-114">Application</span></span> | <span data-ttu-id="b700b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b700b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b700b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b700b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="b700b-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b700b-117">Function parameters</span></span>

| <span data-ttu-id="b700b-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="b700b-118">Parameter</span></span>    | <span data-ttu-id="b700b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b700b-119">Type</span></span>   |<span data-ttu-id="b700b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b700b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b700b-121">count</span><span class="sxs-lookup"><span data-stu-id="b700b-121">count</span></span>|<span data-ttu-id="b700b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b700b-122">Int32</span></span>|<span data-ttu-id="b700b-p102">Optional. Die Anzahl von Zeilen, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="b700b-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b700b-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b700b-128">Request headers</span></span>
| <span data-ttu-id="b700b-129">Name</span><span class="sxs-lookup"><span data-stu-id="b700b-129">Name</span></span>       | <span data-ttu-id="b700b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b700b-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b700b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b700b-131">Authorization</span></span>  | <span data-ttu-id="b700b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b700b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b700b-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b700b-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="b700b-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b700b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b700b-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b700b-137">Request body</span></span>
<span data-ttu-id="b700b-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b700b-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b700b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b700b-139">Response</span></span>

<span data-ttu-id="b700b-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b700b-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b700b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b700b-141">Example</span></span>
<span data-ttu-id="b700b-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b700b-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b700b-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b700b-143">Request</span></span>
<span data-ttu-id="b700b-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b700b-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="b700b-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b700b-145">Response</span></span>
<span data-ttu-id="b700b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b700b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
