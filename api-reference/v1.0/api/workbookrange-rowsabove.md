---
title: 'workbookRange: rowsAbove'
description: Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.
ms.openlocfilehash: 9534a69f9afbc41c6d6803951d35b132f1685e54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017721"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="b9e77-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="b9e77-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="b9e77-104">Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="b9e77-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e77-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9e77-105">Permissions</span></span>
<span data-ttu-id="b9e77-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e77-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9e77-108">Permission type</span></span>      | <span data-ttu-id="b9e77-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9e77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9e77-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9e77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9e77-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e77-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9e77-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9e77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e77-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9e77-113">Not supported.</span></span>    |
|<span data-ttu-id="b9e77-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9e77-114">Application</span></span> | <span data-ttu-id="b9e77-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9e77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9e77-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="b9e77-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b9e77-117">Function parameters</span></span>

| <span data-ttu-id="b9e77-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="b9e77-118">Parameter</span></span>    | <span data-ttu-id="b9e77-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b9e77-119">Type</span></span>   |<span data-ttu-id="b9e77-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9e77-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9e77-121">count</span><span class="sxs-lookup"><span data-stu-id="b9e77-121">count</span></span>|<span data-ttu-id="b9e77-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b9e77-122">Int32</span></span>|<span data-ttu-id="b9e77-p102">Optional. Die Anzahl von Zeilen, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="b9e77-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b9e77-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9e77-128">Request headers</span></span>
| <span data-ttu-id="b9e77-129">Name</span><span class="sxs-lookup"><span data-stu-id="b9e77-129">Name</span></span>       | <span data-ttu-id="b9e77-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9e77-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9e77-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e77-131">Authorization</span></span>  | <span data-ttu-id="b9e77-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9e77-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9e77-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b9e77-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9e77-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b9e77-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e77-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9e77-137">Request body</span></span>
<span data-ttu-id="b9e77-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9e77-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e77-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e77-139">Response</span></span>
<span data-ttu-id="b9e77-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9e77-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e77-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9e77-141">Example</span></span>
<span data-ttu-id="b9e77-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b9e77-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9e77-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e77-143">Request</span></span>
<span data-ttu-id="b9e77-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9e77-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="b9e77-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e77-145">Response</span></span>
<span data-ttu-id="b9e77-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9e77-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="b9e77-149">Wenn Sie ohne den optionalen aufgerufen `count` Parameter, diese Funktion gibt nur eine Zeile oberhalb des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="b9e77-149">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="b9e77-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e77-150">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="b9e77-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e77-151">Response</span></span>
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