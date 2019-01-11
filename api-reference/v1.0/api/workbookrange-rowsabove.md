---
title: 'workbookRange: rowsAbove'
description: Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0eb7a9ec6539854d4148148e2d283df0eaa366d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875012"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="c1d6f-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="c1d6f-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="c1d6f-104">Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1d6f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1d6f-105">Permissions</span></span>
<span data-ttu-id="c1d6f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d6f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1d6f-108">Permission type</span></span>      | <span data-ttu-id="c1d6f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1d6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1d6f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1d6f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1d6f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1d6f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1d6f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1d6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1d6f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d6f-113">Not supported.</span></span>    |
|<span data-ttu-id="c1d6f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1d6f-114">Application</span></span> | <span data-ttu-id="c1d6f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d6f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1d6f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d6f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="c1d6f-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="c1d6f-117">Function parameters</span></span>

| <span data-ttu-id="c1d6f-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="c1d6f-118">Parameter</span></span>    | <span data-ttu-id="c1d6f-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c1d6f-119">Type</span></span>   |<span data-ttu-id="c1d6f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1d6f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1d6f-121">count</span><span class="sxs-lookup"><span data-stu-id="c1d6f-121">count</span></span>|<span data-ttu-id="c1d6f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c1d6f-122">Int32</span></span>|<span data-ttu-id="c1d6f-p102">Optional. Die Anzahl von Zeilen, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c1d6f-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1d6f-128">Request headers</span></span>
| <span data-ttu-id="c1d6f-129">Name</span><span class="sxs-lookup"><span data-stu-id="c1d6f-129">Name</span></span>       | <span data-ttu-id="c1d6f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1d6f-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1d6f-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1d6f-131">Authorization</span></span>  | <span data-ttu-id="c1d6f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1d6f-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c1d6f-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="c1d6f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d6f-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1d6f-137">Request body</span></span>
<span data-ttu-id="c1d6f-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1d6f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d6f-139">Response</span></span>
<span data-ttu-id="c1d6f-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1d6f-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1d6f-141">Example</span></span>
<span data-ttu-id="c1d6f-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1d6f-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d6f-143">Request</span></span>
<span data-ttu-id="c1d6f-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="c1d6f-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d6f-145">Response</span></span>
<span data-ttu-id="c1d6f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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

<span data-ttu-id="c1d6f-149">Wenn Sie ohne den optionalen aufgerufen `count` Parameter, diese Funktion gibt nur eine Zeile oberhalb des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="c1d6f-149">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="c1d6f-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d6f-150">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="c1d6f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d6f-151">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
