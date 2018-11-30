---
title: 'Arbeitsblatt: UsedRange'
description: Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.
ms.openlocfilehash: 6da0ad6ab5fe71491d30eac1e95255d39ba37a18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016474"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="0d0d1-104">Arbeitsblatt: UsedRange</span><span class="sxs-lookup"><span data-stu-id="0d0d1-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="0d0d1-p102">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d0d1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d0d1-107">Permissions</span></span>
<span data-ttu-id="0d0d1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d0d1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d0d1-110">Permission type</span></span>      | <span data-ttu-id="0d0d1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d0d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d0d1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d0d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d0d1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d0d1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0d0d1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d0d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d0d1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d0d1-115">Not supported.</span></span>    |
|<span data-ttu-id="0d0d1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d0d1-116">Application</span></span> | <span data-ttu-id="0d0d1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d0d1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d0d1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d0d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="0d0d1-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0d0d1-119">Function parameters</span></span>
<span data-ttu-id="0d0d1-120">In der Anforderungs-URL können Sie optionale Parameter angeben.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="0d0d1-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="0d0d1-121">Parameter</span></span>    | <span data-ttu-id="0d0d1-122">Typ</span><span class="sxs-lookup"><span data-stu-id="0d0d1-122">Type</span></span>   |<span data-ttu-id="0d0d1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d0d1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d0d1-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="0d0d1-124">valuesOnly</span></span>|<span data-ttu-id="0d0d1-125">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0d0d1-125">Boolean</span></span>|<span data-ttu-id="0d0d1-p104">Optional. Betrachtet nur Zellen mit Werten als verwendet (ignoriert die Formatierung).</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0d0d1-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d0d1-128">Request headers</span></span>
| <span data-ttu-id="0d0d1-129">Name</span><span class="sxs-lookup"><span data-stu-id="0d0d1-129">Name</span></span>       | <span data-ttu-id="0d0d1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d0d1-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d0d1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d0d1-131">Authorization</span></span>  | <span data-ttu-id="0d0d1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d0d1-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0d0d1-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="0d0d1-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d0d1-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d0d1-137">Request body</span></span>
<span data-ttu-id="0d0d1-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d0d1-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d0d1-139">Response</span></span>

<span data-ttu-id="0d0d1-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d0d1-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d0d1-141">Example</span></span>
<span data-ttu-id="0d0d1-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0d0d1-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d0d1-143">Request</span></span>
<span data-ttu-id="0d0d1-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="0d0d1-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d0d1-145">Response</span></span>
<span data-ttu-id="0d0d1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="0d0d1-149">Alternativ kann diese Funktion aufgerufen werden, mit dem optionalen `valuesOnly` Parameter.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-149">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="0d0d1-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d0d1-150">Request</span></span>
<span data-ttu-id="0d0d1-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="0d0d1-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d0d1-152">Response</span></span>
<span data-ttu-id="0d0d1-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d0d1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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