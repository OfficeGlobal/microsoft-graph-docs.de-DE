---
title: rangefont aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 40dfe68ec16415dbfa4abcbdb46da8cc9f89c961
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927303"
---
# <a name="update-rangefont"></a><span data-ttu-id="36eb3-103">rangefont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="36eb3-103">Update rangefont</span></span>

<span data-ttu-id="36eb3-104">Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36eb3-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36eb3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="36eb3-105">Permissions</span></span>
<span data-ttu-id="36eb3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36eb3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36eb3-108">Permission type</span></span>      | <span data-ttu-id="36eb3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36eb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36eb3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36eb3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36eb3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36eb3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36eb3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36eb3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36eb3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36eb3-113">Not supported.</span></span>    |
|<span data-ttu-id="36eb3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36eb3-114">Application</span></span> | <span data-ttu-id="36eb3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36eb3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36eb3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36eb3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="request-headers"></a><span data-ttu-id="36eb3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36eb3-117">Request headers</span></span>
| <span data-ttu-id="36eb3-118">Name</span><span class="sxs-lookup"><span data-stu-id="36eb3-118">Name</span></span>       | <span data-ttu-id="36eb3-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36eb3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36eb3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="36eb3-120">Authorization</span></span>  | <span data-ttu-id="36eb3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36eb3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36eb3-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="36eb3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="36eb3-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="36eb3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36eb3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36eb3-126">Request body</span></span>
<span data-ttu-id="36eb3-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="36eb3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36eb3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36eb3-130">Property</span></span>     | <span data-ttu-id="36eb3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="36eb3-131">Type</span></span>   |<span data-ttu-id="36eb3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36eb3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36eb3-133">bold</span><span class="sxs-lookup"><span data-stu-id="36eb3-133">bold</span></span>|<span data-ttu-id="36eb3-134">boolean</span><span class="sxs-lookup"><span data-stu-id="36eb3-134">boolean</span></span>|<span data-ttu-id="36eb3-135">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="36eb3-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="36eb3-136">color</span><span class="sxs-lookup"><span data-stu-id="36eb3-136">color</span></span>|<span data-ttu-id="36eb3-137">string</span><span class="sxs-lookup"><span data-stu-id="36eb3-137">string</span></span>|<span data-ttu-id="36eb3-p105">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="36eb3-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="36eb3-141">italic</span><span class="sxs-lookup"><span data-stu-id="36eb3-141">italic</span></span>|<span data-ttu-id="36eb3-142">boolean</span><span class="sxs-lookup"><span data-stu-id="36eb3-142">boolean</span></span>|<span data-ttu-id="36eb3-143">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="36eb3-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="36eb3-144">name</span><span class="sxs-lookup"><span data-stu-id="36eb3-144">name</span></span>|<span data-ttu-id="36eb3-145">string</span><span class="sxs-lookup"><span data-stu-id="36eb3-145">string</span></span>|<span data-ttu-id="36eb3-146">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="36eb3-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="36eb3-147">size</span><span class="sxs-lookup"><span data-stu-id="36eb3-147">size</span></span>|<span data-ttu-id="36eb3-148">double</span><span class="sxs-lookup"><span data-stu-id="36eb3-148">double</span></span>|<span data-ttu-id="36eb3-149">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="36eb3-149">Font size.</span></span>|
|<span data-ttu-id="36eb3-150">underline</span><span class="sxs-lookup"><span data-stu-id="36eb3-150">underline</span></span>|<span data-ttu-id="36eb3-151">string</span><span class="sxs-lookup"><span data-stu-id="36eb3-151">string</span></span>|<span data-ttu-id="36eb3-152">Typ der Unterstreichung auf die Schriftart.</span><span class="sxs-lookup"><span data-stu-id="36eb3-152">Type of underline applied to the font.</span></span> <span data-ttu-id="36eb3-153">Die möglichen Werte sind: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="36eb3-153">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="36eb3-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="36eb3-154">Response</span></span>

<span data-ttu-id="36eb3-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookRangeFont](../resources/rangefont.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="36eb3-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36eb3-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36eb3-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36eb3-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36eb3-157">Request</span></span>
<span data-ttu-id="36eb3-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36eb3-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="36eb3-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="36eb3-159">Response</span></span>
<span data-ttu-id="36eb3-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36eb3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
