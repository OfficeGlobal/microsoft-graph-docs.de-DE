---
title: 'workbookRange: columnsAfter'
description: Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.
author: lumine2008
ms.openlocfilehash: f597d117a4b182656e636108b8a821e0db31be6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305194"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="aa163-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="aa163-103">workbookRange: columnsAfter</span></span>

> <span data-ttu-id="aa163-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aa163-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa163-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa163-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa163-106">Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.</span><span class="sxs-lookup"><span data-stu-id="aa163-106">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa163-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa163-107">Permissions</span></span>
<span data-ttu-id="aa163-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa163-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa163-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa163-110">Permission type</span></span>      | <span data-ttu-id="aa163-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa163-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa163-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa163-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa163-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa163-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa163-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa163-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa163-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa163-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa163-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa163-116">Application</span></span> | <span data-ttu-id="aa163-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa163-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa163-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa163-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="aa163-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="aa163-119">Function parameters</span></span>

| <span data-ttu-id="aa163-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="aa163-120">Parameter</span></span>    | <span data-ttu-id="aa163-121">Typ</span><span class="sxs-lookup"><span data-stu-id="aa163-121">Type</span></span>   |<span data-ttu-id="aa163-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa163-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa163-123">count</span><span class="sxs-lookup"><span data-stu-id="aa163-123">count</span></span>|<span data-ttu-id="aa163-124">Int32</span><span class="sxs-lookup"><span data-stu-id="aa163-124">Int32</span></span>|<span data-ttu-id="aa163-p103">Die Anzahl von Spalten, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="aa163-p103">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="aa163-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa163-129">Request headers</span></span>
| <span data-ttu-id="aa163-130">Name</span><span class="sxs-lookup"><span data-stu-id="aa163-130">Name</span></span>       | <span data-ttu-id="aa163-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa163-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa163-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa163-132">Authorization</span></span>  | <span data-ttu-id="aa163-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa163-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa163-135">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="aa163-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa163-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="aa163-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa163-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa163-138">Request body</span></span>
<span data-ttu-id="aa163-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa163-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa163-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa163-140">Response</span></span>

<span data-ttu-id="aa163-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa163-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa163-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa163-142">Example</span></span>
<span data-ttu-id="aa163-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="aa163-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aa163-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa163-144">Request</span></span>
<span data-ttu-id="aa163-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa163-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="aa163-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa163-146">Response</span></span>
<span data-ttu-id="aa163-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa163-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
