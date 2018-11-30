---
title: 'workbookRange: resizedRange'
description: Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.
ms.openlocfilehash: cd2851e1b4f65162fca6e617878851b2cc8e910b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060465"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="e981a-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="e981a-103">workbookRange: resizedRange</span></span>

> <span data-ttu-id="e981a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e981a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e981a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e981a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e981a-106">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="e981a-106">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="e981a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e981a-107">Permissions</span></span>
<span data-ttu-id="e981a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e981a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e981a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e981a-110">Permission type</span></span>      | <span data-ttu-id="e981a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e981a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e981a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e981a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e981a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e981a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e981a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e981a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e981a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e981a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e981a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e981a-116">Application</span></span> | <span data-ttu-id="e981a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e981a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e981a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e981a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="e981a-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e981a-119">Function parameters</span></span>

| <span data-ttu-id="e981a-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="e981a-120">Parameter</span></span>    | <span data-ttu-id="e981a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e981a-121">Type</span></span>   |<span data-ttu-id="e981a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e981a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e981a-123">deltarows</span><span class="sxs-lookup"><span data-stu-id="e981a-123">deltarows</span></span>|<span data-ttu-id="e981a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e981a-124">Int32</span></span>|<span data-ttu-id="e981a-p103">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="e981a-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="e981a-127">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="e981a-127">deltaColumns</span></span>|<span data-ttu-id="e981a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e981a-128">Int32</span></span>|<span data-ttu-id="e981a-p104">Die Anzahl von Spalten, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="e981a-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e981a-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e981a-131">Request headers</span></span>
| <span data-ttu-id="e981a-132">Name</span><span class="sxs-lookup"><span data-stu-id="e981a-132">Name</span></span>       | <span data-ttu-id="e981a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e981a-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e981a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="e981a-134">Authorization</span></span>  | <span data-ttu-id="e981a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e981a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e981a-137">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e981a-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="e981a-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e981a-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e981a-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e981a-140">Request body</span></span>
<span data-ttu-id="e981a-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e981a-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e981a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e981a-142">Response</span></span>

<span data-ttu-id="e981a-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e981a-143">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e981a-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e981a-144">Example</span></span>
<span data-ttu-id="e981a-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e981a-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e981a-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e981a-146">Request</span></span>
<span data-ttu-id="e981a-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e981a-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="e981a-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="e981a-148">Response</span></span>
<span data-ttu-id="e981a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e981a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
