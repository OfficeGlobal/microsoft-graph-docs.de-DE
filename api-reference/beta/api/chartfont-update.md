---
title: ChartFont aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartFont-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6030bd9a5ab39f56ecb84da4f60457b4c8d8ba53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864953"
---
# <a name="update-chartfont"></a><span data-ttu-id="3e165-103">ChartFont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3e165-103">Update chartfont</span></span>

> <span data-ttu-id="3e165-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e165-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e165-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e165-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e165-106">Dient zum Aktualisieren der Eigenschaften des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e165-106">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e165-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e165-107">Permissions</span></span>
<span data-ttu-id="3e165-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e165-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e165-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e165-110">Permission type</span></span>      | <span data-ttu-id="3e165-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e165-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e165-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e165-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e165-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e165-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e165-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e165-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e165-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e165-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e165-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e165-116">Application</span></span> | <span data-ttu-id="3e165-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e165-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e165-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e165-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="3e165-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e165-119">Optional request headers</span></span>
| <span data-ttu-id="3e165-120">Name</span><span class="sxs-lookup"><span data-stu-id="3e165-120">Name</span></span>       | <span data-ttu-id="3e165-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e165-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3e165-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e165-122">Authorization</span></span>  | <span data-ttu-id="3e165-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e165-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e165-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3e165-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e165-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3e165-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e165-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e165-128">Request body</span></span>
<span data-ttu-id="3e165-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="3e165-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e165-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e165-132">Property</span></span>     | <span data-ttu-id="3e165-133">Typ</span><span class="sxs-lookup"><span data-stu-id="3e165-133">Type</span></span>   |<span data-ttu-id="3e165-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e165-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e165-135">bold</span><span class="sxs-lookup"><span data-stu-id="3e165-135">bold</span></span>|<span data-ttu-id="3e165-136">boolean</span><span class="sxs-lookup"><span data-stu-id="3e165-136">boolean</span></span>|<span data-ttu-id="3e165-137">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="3e165-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3e165-138">color</span><span class="sxs-lookup"><span data-stu-id="3e165-138">color</span></span>|<span data-ttu-id="3e165-139">string</span><span class="sxs-lookup"><span data-stu-id="3e165-139">string</span></span>|<span data-ttu-id="3e165-p106">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="3e165-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3e165-143">italic</span><span class="sxs-lookup"><span data-stu-id="3e165-143">italic</span></span>|<span data-ttu-id="3e165-144">boolean</span><span class="sxs-lookup"><span data-stu-id="3e165-144">boolean</span></span>|<span data-ttu-id="3e165-145">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="3e165-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3e165-146">name</span><span class="sxs-lookup"><span data-stu-id="3e165-146">name</span></span>|<span data-ttu-id="3e165-147">string</span><span class="sxs-lookup"><span data-stu-id="3e165-147">string</span></span>|<span data-ttu-id="3e165-148">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="3e165-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3e165-149">size</span><span class="sxs-lookup"><span data-stu-id="3e165-149">size</span></span>|<span data-ttu-id="3e165-150">double</span><span class="sxs-lookup"><span data-stu-id="3e165-150">double</span></span>|<span data-ttu-id="3e165-151">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="3e165-151">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="3e165-152">underline</span><span class="sxs-lookup"><span data-stu-id="3e165-152">underline</span></span>|<span data-ttu-id="3e165-153">string</span><span class="sxs-lookup"><span data-stu-id="3e165-153">string</span></span>|<span data-ttu-id="3e165-p107">Art der auf die Schriftart angewendeten Unterstreichung. Mögliche Werte: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="3e165-p107">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="3e165-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e165-156">Response</span></span>

<span data-ttu-id="3e165-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartFont](../resources/chartfont.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e165-157">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e165-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e165-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e165-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e165-159">Request</span></span>
<span data-ttu-id="3e165-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e165-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
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
##### <a name="response"></a><span data-ttu-id="3e165-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e165-161">Response</span></span>
<span data-ttu-id="3e165-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e165-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
