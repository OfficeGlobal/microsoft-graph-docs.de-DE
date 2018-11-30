---
title: rangefont aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.
ms.openlocfilehash: 199fb62bdc50ab3826cdbd02914412e461022287
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063688"
---
# <a name="update-rangefont"></a><span data-ttu-id="1f7b3-103">rangefont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f7b3-103">Update rangefont</span></span>

> <span data-ttu-id="1f7b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f7b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f7b3-106">Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-106">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f7b3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f7b3-107">Permissions</span></span>
<span data-ttu-id="1f7b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f7b3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f7b3-110">Permission type</span></span>      | <span data-ttu-id="1f7b3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f7b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f7b3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f7b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1f7b3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f7b3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f7b3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f7b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f7b3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f7b3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f7b3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f7b3-116">Application</span></span> | <span data-ttu-id="1f7b3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f7b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f7b3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f7b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="1f7b3-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f7b3-119">Optional request headers</span></span>
| <span data-ttu-id="1f7b3-120">Name</span><span class="sxs-lookup"><span data-stu-id="1f7b3-120">Name</span></span>       | <span data-ttu-id="1f7b3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f7b3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1f7b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f7b3-122">Authorization</span></span>  | <span data-ttu-id="1f7b3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f7b3-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1f7b3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f7b3-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f7b3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f7b3-128">Request body</span></span>
<span data-ttu-id="1f7b3-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f7b3-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f7b3-132">Property</span></span>     | <span data-ttu-id="1f7b3-133">Typ</span><span class="sxs-lookup"><span data-stu-id="1f7b3-133">Type</span></span>   |<span data-ttu-id="1f7b3-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f7b3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f7b3-135">bold</span><span class="sxs-lookup"><span data-stu-id="1f7b3-135">bold</span></span>|<span data-ttu-id="1f7b3-136">boolean</span><span class="sxs-lookup"><span data-stu-id="1f7b3-136">boolean</span></span>|<span data-ttu-id="1f7b3-137">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="1f7b3-138">color</span><span class="sxs-lookup"><span data-stu-id="1f7b3-138">color</span></span>|<span data-ttu-id="1f7b3-139">string</span><span class="sxs-lookup"><span data-stu-id="1f7b3-139">string</span></span>|<span data-ttu-id="1f7b3-p106">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="1f7b3-143">italic</span><span class="sxs-lookup"><span data-stu-id="1f7b3-143">italic</span></span>|<span data-ttu-id="1f7b3-144">boolean</span><span class="sxs-lookup"><span data-stu-id="1f7b3-144">boolean</span></span>|<span data-ttu-id="1f7b3-145">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="1f7b3-146">name</span><span class="sxs-lookup"><span data-stu-id="1f7b3-146">name</span></span>|<span data-ttu-id="1f7b3-147">string</span><span class="sxs-lookup"><span data-stu-id="1f7b3-147">string</span></span>|<span data-ttu-id="1f7b3-148">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="1f7b3-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="1f7b3-149">size</span><span class="sxs-lookup"><span data-stu-id="1f7b3-149">size</span></span>|<span data-ttu-id="1f7b3-150">double</span><span class="sxs-lookup"><span data-stu-id="1f7b3-150">double</span></span>|<span data-ttu-id="1f7b3-151">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="1f7b3-151">Font size.</span></span>|
|<span data-ttu-id="1f7b3-152">underline</span><span class="sxs-lookup"><span data-stu-id="1f7b3-152">underline</span></span>|<span data-ttu-id="1f7b3-153">string</span><span class="sxs-lookup"><span data-stu-id="1f7b3-153">string</span></span>|<span data-ttu-id="1f7b3-p107">Art der auf die Schriftart angewendete Unterstreichung. Die folgenden Werte sind möglich: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p107">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="1f7b3-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f7b3-156">Response</span></span>

<span data-ttu-id="1f7b3-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFont](../resources/rangefont.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-157">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f7b3-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f7b3-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f7b3-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f7b3-159">Request</span></span>
<span data-ttu-id="1f7b3-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="1f7b3-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f7b3-161">Response</span></span>
<span data-ttu-id="1f7b3-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f7b3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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