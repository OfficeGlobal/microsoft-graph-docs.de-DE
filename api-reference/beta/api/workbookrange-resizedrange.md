---
title: 'workbookRange: resizedRange'
description: Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 667393920d936b0227affe178cb38f6bb54d49ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514838"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="b5b39-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="b5b39-103">workbookRange: resizedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5b39-104">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="b5b39-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5b39-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b5b39-105">Permissions</span></span>
<span data-ttu-id="b5b39-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5b39-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5b39-108">Permission type</span></span>      | <span data-ttu-id="b5b39-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5b39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5b39-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5b39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5b39-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5b39-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b5b39-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5b39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5b39-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5b39-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b5b39-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5b39-114">Application</span></span> | <span data-ttu-id="b5b39-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5b39-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5b39-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b39-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="b5b39-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b5b39-117">Function parameters</span></span>

| <span data-ttu-id="b5b39-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="b5b39-118">Parameter</span></span>    | <span data-ttu-id="b5b39-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b5b39-119">Type</span></span>   |<span data-ttu-id="b5b39-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5b39-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5b39-121">deltarows</span><span class="sxs-lookup"><span data-stu-id="b5b39-121">deltarows</span></span>|<span data-ttu-id="b5b39-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b5b39-122">Int32</span></span>|<span data-ttu-id="b5b39-p102">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="b5b39-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="b5b39-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="b5b39-125">deltaColumns</span></span>|<span data-ttu-id="b5b39-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b5b39-126">Int32</span></span>|<span data-ttu-id="b5b39-p103">Die Anzahl von Spalten, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="b5b39-p103">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b5b39-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5b39-129">Request headers</span></span>
| <span data-ttu-id="b5b39-130">Name</span><span class="sxs-lookup"><span data-stu-id="b5b39-130">Name</span></span>       | <span data-ttu-id="b5b39-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5b39-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5b39-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5b39-132">Authorization</span></span>  | <span data-ttu-id="b5b39-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5b39-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5b39-135">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b5b39-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="b5b39-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b5b39-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5b39-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5b39-138">Request body</span></span>
<span data-ttu-id="b5b39-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b5b39-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5b39-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b39-140">Response</span></span>

<span data-ttu-id="b5b39-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5b39-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5b39-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5b39-142">Example</span></span>
<span data-ttu-id="b5b39-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b5b39-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b5b39-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b39-144">Request</span></span>
<span data-ttu-id="b5b39-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5b39-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="b5b39-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b39-146">Response</span></span>
<span data-ttu-id="b5b39-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5b39-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-resizedrange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
