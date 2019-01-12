---
title: 'workbookRange: resizedRange'
description: Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4068da86c1653a01a478d385c5c854c700e50ae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931335"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="2f403-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="2f403-103">workbookRange: resizedRange</span></span>

> <span data-ttu-id="2f403-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2f403-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f403-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f403-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f403-106">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="2f403-106">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f403-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f403-107">Permissions</span></span>
<span data-ttu-id="2f403-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f403-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f403-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f403-110">Permission type</span></span>      | <span data-ttu-id="2f403-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f403-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f403-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f403-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2f403-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f403-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f403-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f403-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f403-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f403-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f403-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f403-116">Application</span></span> | <span data-ttu-id="2f403-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f403-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f403-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f403-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="2f403-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="2f403-119">Function parameters</span></span>

| <span data-ttu-id="2f403-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="2f403-120">Parameter</span></span>    | <span data-ttu-id="2f403-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2f403-121">Type</span></span>   |<span data-ttu-id="2f403-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f403-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f403-123">deltarows</span><span class="sxs-lookup"><span data-stu-id="2f403-123">deltarows</span></span>|<span data-ttu-id="2f403-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2f403-124">Int32</span></span>|<span data-ttu-id="2f403-p103">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="2f403-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="2f403-127">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="2f403-127">deltaColumns</span></span>|<span data-ttu-id="2f403-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2f403-128">Int32</span></span>|<span data-ttu-id="2f403-p104">Die Anzahl von Spalten, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="2f403-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2f403-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f403-131">Request headers</span></span>
| <span data-ttu-id="2f403-132">Name</span><span class="sxs-lookup"><span data-stu-id="2f403-132">Name</span></span>       | <span data-ttu-id="2f403-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f403-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f403-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f403-134">Authorization</span></span>  | <span data-ttu-id="2f403-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f403-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f403-137">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2f403-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="2f403-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2f403-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f403-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f403-140">Request body</span></span>
<span data-ttu-id="2f403-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f403-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f403-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f403-142">Response</span></span>

<span data-ttu-id="2f403-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f403-143">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f403-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f403-144">Example</span></span>
<span data-ttu-id="2f403-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2f403-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f403-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f403-146">Request</span></span>
<span data-ttu-id="2f403-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f403-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="2f403-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f403-148">Response</span></span>
<span data-ttu-id="2f403-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f403-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
