---
title: 'workbookRange: columnsBefore'
description: Ruft eine bestimmte Anzahl von Spalten links vom gegebenen Bereich ab.
ms.openlocfilehash: c6214baadd520637554038b0f344efaa066533ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019663"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="29b26-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="29b26-103">workbookRange: columnsBefore</span></span>

<span data-ttu-id="29b26-104">Ruft eine bestimmte Anzahl von Spalten links vom gegebenen Bereich ab.</span><span class="sxs-lookup"><span data-stu-id="29b26-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="29b26-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29b26-105">Permissions</span></span>
<span data-ttu-id="29b26-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b26-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29b26-108">Permission type</span></span>      | <span data-ttu-id="29b26-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29b26-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29b26-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29b26-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29b26-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29b26-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29b26-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29b26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29b26-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29b26-113">Not supported.</span></span>    |
|<span data-ttu-id="29b26-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29b26-114">Application</span></span> | <span data-ttu-id="29b26-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29b26-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29b26-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29b26-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="29b26-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="29b26-117">Function parameters</span></span>

| <span data-ttu-id="29b26-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="29b26-118">Parameter</span></span>    | <span data-ttu-id="29b26-119">Typ</span><span class="sxs-lookup"><span data-stu-id="29b26-119">Type</span></span>   |<span data-ttu-id="29b26-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29b26-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29b26-121">count</span><span class="sxs-lookup"><span data-stu-id="29b26-121">count</span></span>|<span data-ttu-id="29b26-122">Int32</span><span class="sxs-lookup"><span data-stu-id="29b26-122">Int32</span></span>|<span data-ttu-id="29b26-p102">Optional. Die Anzahl von Spalten, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="29b26-p102">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="29b26-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29b26-128">Request headers</span></span>
| <span data-ttu-id="29b26-129">Name</span><span class="sxs-lookup"><span data-stu-id="29b26-129">Name</span></span>       | <span data-ttu-id="29b26-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29b26-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29b26-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="29b26-131">Authorization</span></span>  | <span data-ttu-id="29b26-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29b26-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29b26-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="29b26-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="29b26-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="29b26-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b26-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29b26-137">Request body</span></span>
<span data-ttu-id="29b26-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29b26-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29b26-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="29b26-139">Response</span></span>
<span data-ttu-id="29b26-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29b26-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29b26-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29b26-141">Example</span></span>
<span data-ttu-id="29b26-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="29b26-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29b26-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29b26-143">Request</span></span>
<span data-ttu-id="29b26-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29b26-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="29b26-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="29b26-145">Response</span></span>
<span data-ttu-id="29b26-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29b26-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
