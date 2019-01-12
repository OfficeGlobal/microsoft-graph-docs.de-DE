---
title: 'Arbeitsblatt: UsedRange'
description: Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 444a88dfaad3983948a139f2a3db304c200a1153
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975302"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="10a3f-104">Arbeitsblatt: UsedRange</span><span class="sxs-lookup"><span data-stu-id="10a3f-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="10a3f-p102">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="10a3f-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="10a3f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="10a3f-107">Permissions</span></span>
<span data-ttu-id="10a3f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10a3f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10a3f-110">Permission type</span></span>      | <span data-ttu-id="10a3f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10a3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10a3f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10a3f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10a3f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10a3f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10a3f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10a3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10a3f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10a3f-115">Not supported.</span></span>    |
|<span data-ttu-id="10a3f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10a3f-116">Application</span></span> | <span data-ttu-id="10a3f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10a3f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10a3f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10a3f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="10a3f-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="10a3f-119">Function parameters</span></span>
<span data-ttu-id="10a3f-120">In der Anforderungs-URL können Sie optionale Parameter angeben.</span><span class="sxs-lookup"><span data-stu-id="10a3f-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="10a3f-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="10a3f-121">Parameter</span></span>    | <span data-ttu-id="10a3f-122">Typ</span><span class="sxs-lookup"><span data-stu-id="10a3f-122">Type</span></span>   |<span data-ttu-id="10a3f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10a3f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10a3f-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="10a3f-124">valuesOnly</span></span>|<span data-ttu-id="10a3f-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="10a3f-125">Boolean</span></span>|<span data-ttu-id="10a3f-p104">Optional. Betrachtet nur Zellen mit Werten als verwendet (ignoriert die Formatierung).</span><span class="sxs-lookup"><span data-stu-id="10a3f-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="10a3f-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10a3f-128">Request headers</span></span>
| <span data-ttu-id="10a3f-129">Name</span><span class="sxs-lookup"><span data-stu-id="10a3f-129">Name</span></span>       | <span data-ttu-id="10a3f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10a3f-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="10a3f-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="10a3f-131">Authorization</span></span>  | <span data-ttu-id="10a3f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10a3f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10a3f-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="10a3f-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="10a3f-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="10a3f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10a3f-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10a3f-137">Request body</span></span>
<span data-ttu-id="10a3f-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="10a3f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10a3f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="10a3f-139">Response</span></span>

<span data-ttu-id="10a3f-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10a3f-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10a3f-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10a3f-141">Example</span></span>
<span data-ttu-id="10a3f-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="10a3f-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="10a3f-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10a3f-143">Request</span></span>
<span data-ttu-id="10a3f-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10a3f-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="10a3f-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="10a3f-145">Response</span></span>
<span data-ttu-id="10a3f-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10a3f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="10a3f-149">Alternativ kann diese Funktion aufgerufen werden, mit dem optionalen `valuesOnly` Parameter.</span><span class="sxs-lookup"><span data-stu-id="10a3f-149">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="10a3f-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10a3f-150">Request</span></span>
<span data-ttu-id="10a3f-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10a3f-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="10a3f-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="10a3f-152">Response</span></span>
<span data-ttu-id="10a3f-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10a3f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
