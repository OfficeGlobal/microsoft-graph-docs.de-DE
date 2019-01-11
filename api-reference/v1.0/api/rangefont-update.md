---
title: rangefont aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4a9e73842a664ab11c7b61a5b3851e83b410938c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816660"
---
# <a name="update-rangefont"></a><span data-ttu-id="24a32-103">rangefont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="24a32-103">Update rangefont</span></span>

<span data-ttu-id="24a32-104">Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="24a32-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="24a32-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24a32-105">Permissions</span></span>
<span data-ttu-id="24a32-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24a32-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24a32-108">Permission type</span></span>      | <span data-ttu-id="24a32-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24a32-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24a32-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24a32-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24a32-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24a32-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24a32-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24a32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24a32-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24a32-113">Not supported.</span></span>    |
|<span data-ttu-id="24a32-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24a32-114">Application</span></span> | <span data-ttu-id="24a32-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24a32-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24a32-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24a32-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="request-headers"></a><span data-ttu-id="24a32-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24a32-117">Request headers</span></span>
| <span data-ttu-id="24a32-118">Name</span><span class="sxs-lookup"><span data-stu-id="24a32-118">Name</span></span>       | <span data-ttu-id="24a32-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24a32-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="24a32-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="24a32-120">Authorization</span></span>  | <span data-ttu-id="24a32-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24a32-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24a32-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="24a32-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="24a32-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="24a32-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24a32-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24a32-126">Request body</span></span>
<span data-ttu-id="24a32-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="24a32-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="24a32-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24a32-130">Property</span></span>     | <span data-ttu-id="24a32-131">Typ</span><span class="sxs-lookup"><span data-stu-id="24a32-131">Type</span></span>   |<span data-ttu-id="24a32-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24a32-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24a32-133">bold</span><span class="sxs-lookup"><span data-stu-id="24a32-133">bold</span></span>|<span data-ttu-id="24a32-134">boolean</span><span class="sxs-lookup"><span data-stu-id="24a32-134">boolean</span></span>|<span data-ttu-id="24a32-135">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="24a32-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="24a32-136">color</span><span class="sxs-lookup"><span data-stu-id="24a32-136">color</span></span>|<span data-ttu-id="24a32-137">string</span><span class="sxs-lookup"><span data-stu-id="24a32-137">string</span></span>|<span data-ttu-id="24a32-p105">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="24a32-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="24a32-141">italic</span><span class="sxs-lookup"><span data-stu-id="24a32-141">italic</span></span>|<span data-ttu-id="24a32-142">boolean</span><span class="sxs-lookup"><span data-stu-id="24a32-142">boolean</span></span>|<span data-ttu-id="24a32-143">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="24a32-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="24a32-144">name</span><span class="sxs-lookup"><span data-stu-id="24a32-144">name</span></span>|<span data-ttu-id="24a32-145">string</span><span class="sxs-lookup"><span data-stu-id="24a32-145">string</span></span>|<span data-ttu-id="24a32-146">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="24a32-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="24a32-147">size</span><span class="sxs-lookup"><span data-stu-id="24a32-147">size</span></span>|<span data-ttu-id="24a32-148">double</span><span class="sxs-lookup"><span data-stu-id="24a32-148">double</span></span>|<span data-ttu-id="24a32-149">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="24a32-149">Font size.</span></span>|
|<span data-ttu-id="24a32-150">underline</span><span class="sxs-lookup"><span data-stu-id="24a32-150">underline</span></span>|<span data-ttu-id="24a32-151">string</span><span class="sxs-lookup"><span data-stu-id="24a32-151">string</span></span>|<span data-ttu-id="24a32-152">Typ der Unterstreichung auf die Schriftart.</span><span class="sxs-lookup"><span data-stu-id="24a32-152">Type of underline applied to the font.</span></span> <span data-ttu-id="24a32-153">Die möglichen Werte sind: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="24a32-153">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="24a32-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="24a32-154">Response</span></span>

<span data-ttu-id="24a32-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookRangeFont](../resources/rangefont.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24a32-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24a32-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24a32-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24a32-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24a32-157">Request</span></span>
<span data-ttu-id="24a32-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24a32-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="24a32-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="24a32-159">Response</span></span>
<span data-ttu-id="24a32-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24a32-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
