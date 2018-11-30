---
title: 'workbookRange: resizedRange'
description: Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.
ms.openlocfilehash: 167aef7a1d7c975298b80d9e27aad7043b276b35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016883"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="4a1de-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="4a1de-103">workbookRange: resizedRange</span></span>
<span data-ttu-id="4a1de-104">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="4a1de-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a1de-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a1de-105">Permissions</span></span>
<span data-ttu-id="4a1de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a1de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a1de-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a1de-108">Permission type</span></span>      | <span data-ttu-id="4a1de-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a1de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a1de-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a1de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a1de-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a1de-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a1de-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a1de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a1de-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a1de-113">Not supported.</span></span>    |
|<span data-ttu-id="4a1de-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a1de-114">Application</span></span> | <span data-ttu-id="4a1de-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a1de-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a1de-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a1de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="4a1de-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4a1de-117">Function parameters</span></span>

| <span data-ttu-id="4a1de-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="4a1de-118">Parameter</span></span>    | <span data-ttu-id="4a1de-119">Typ</span><span class="sxs-lookup"><span data-stu-id="4a1de-119">Type</span></span>   |<span data-ttu-id="4a1de-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a1de-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a1de-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="4a1de-121">deltaRows</span></span>|<span data-ttu-id="4a1de-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4a1de-122">Int32</span></span>|<span data-ttu-id="4a1de-p102">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="4a1de-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="4a1de-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="4a1de-125">deltaColumns</span></span>|<span data-ttu-id="4a1de-126">Int32</span><span class="sxs-lookup"><span data-stu-id="4a1de-126">Int32</span></span>|<span data-ttu-id="4a1de-127">Die Anzahl der Spalten, um der unteren rechten Ecke, relativ zum aktuellen Bereich erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="4a1de-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="4a1de-128">Verwenden Sie eine positive Zahl, erweitern den Bereich oder eine negative Zahl zu verringern.</span><span class="sxs-lookup"><span data-stu-id="4a1de-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4a1de-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a1de-129">Request headers</span></span>
| <span data-ttu-id="4a1de-130">Name</span><span class="sxs-lookup"><span data-stu-id="4a1de-130">Name</span></span>       | <span data-ttu-id="4a1de-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a1de-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a1de-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a1de-132">Authorization</span></span>  | <span data-ttu-id="4a1de-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a1de-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a1de-135">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4a1de-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a1de-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4a1de-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a1de-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a1de-138">Request body</span></span>
<span data-ttu-id="4a1de-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4a1de-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4a1de-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a1de-140">Response</span></span>
<span data-ttu-id="4a1de-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a1de-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a1de-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a1de-142">Example</span></span>
<span data-ttu-id="4a1de-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4a1de-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a1de-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a1de-144">Request</span></span>
<span data-ttu-id="4a1de-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a1de-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="4a1de-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a1de-146">Response</span></span>
<span data-ttu-id="4a1de-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a1de-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->