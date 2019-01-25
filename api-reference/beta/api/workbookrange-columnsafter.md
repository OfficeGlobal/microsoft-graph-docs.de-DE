---
title: 'workbookRange: columnsAfter'
description: Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3623cfb0b4dc487a1e15e6b1c29726433700b04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522014"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="e6895-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="e6895-103">workbookRange: columnsAfter</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6895-104">Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.</span><span class="sxs-lookup"><span data-stu-id="e6895-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6895-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6895-105">Permissions</span></span>
<span data-ttu-id="e6895-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6895-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6895-108">Permission type</span></span>      | <span data-ttu-id="e6895-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6895-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6895-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6895-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6895-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6895-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6895-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6895-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6895-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6895-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6895-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6895-114">Application</span></span> | <span data-ttu-id="e6895-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6895-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6895-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6895-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="e6895-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e6895-117">Function parameters</span></span>

| <span data-ttu-id="e6895-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="e6895-118">Parameter</span></span>    | <span data-ttu-id="e6895-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e6895-119">Type</span></span>   |<span data-ttu-id="e6895-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6895-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6895-121">count</span><span class="sxs-lookup"><span data-stu-id="e6895-121">count</span></span>|<span data-ttu-id="e6895-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e6895-122">Int32</span></span>|<span data-ttu-id="e6895-p102">Die Anzahl von Spalten, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="e6895-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e6895-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6895-127">Request headers</span></span>
| <span data-ttu-id="e6895-128">Name</span><span class="sxs-lookup"><span data-stu-id="e6895-128">Name</span></span>       | <span data-ttu-id="e6895-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6895-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6895-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6895-130">Authorization</span></span>  | <span data-ttu-id="e6895-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6895-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6895-133">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e6895-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6895-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e6895-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6895-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6895-136">Request body</span></span>
<span data-ttu-id="e6895-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6895-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6895-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6895-138">Response</span></span>

<span data-ttu-id="e6895-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6895-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6895-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6895-140">Example</span></span>
<span data-ttu-id="e6895-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e6895-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6895-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6895-142">Request</span></span>
<span data-ttu-id="e6895-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6895-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="e6895-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6895-144">Response</span></span>
<span data-ttu-id="e6895-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6895-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
