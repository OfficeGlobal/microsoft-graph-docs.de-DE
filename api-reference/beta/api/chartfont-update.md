---
title: ChartFont aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartFont-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4878e78690cc0b28f686d4f0c3c678325397cc07
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642303"
---
# <a name="update-chartfont"></a><span data-ttu-id="56d77-103">ChartFont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56d77-103">Update chartfont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56d77-104">Dient zum Aktualisieren der Eigenschaften des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56d77-104">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="56d77-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="56d77-105">Permissions</span></span>
<span data-ttu-id="56d77-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d77-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56d77-108">Permission type</span></span>      | <span data-ttu-id="56d77-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56d77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d77-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56d77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56d77-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d77-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56d77-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56d77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d77-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d77-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56d77-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56d77-114">Application</span></span> | <span data-ttu-id="56d77-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56d77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d77-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56d77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="56d77-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56d77-117">Optional request headers</span></span>
| <span data-ttu-id="56d77-118">Name</span><span class="sxs-lookup"><span data-stu-id="56d77-118">Name</span></span>       | <span data-ttu-id="56d77-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56d77-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="56d77-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="56d77-120">Authorization</span></span>  | <span data-ttu-id="56d77-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56d77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56d77-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="56d77-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="56d77-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="56d77-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56d77-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56d77-126">Request body</span></span>
<span data-ttu-id="56d77-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="56d77-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="56d77-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56d77-130">Property</span></span>     | <span data-ttu-id="56d77-131">Typ</span><span class="sxs-lookup"><span data-stu-id="56d77-131">Type</span></span>   |<span data-ttu-id="56d77-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56d77-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56d77-133">bold</span><span class="sxs-lookup"><span data-stu-id="56d77-133">bold</span></span>|<span data-ttu-id="56d77-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="56d77-134">boolean</span></span>|<span data-ttu-id="56d77-135">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="56d77-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="56d77-136">color</span><span class="sxs-lookup"><span data-stu-id="56d77-136">color</span></span>|<span data-ttu-id="56d77-137">string</span><span class="sxs-lookup"><span data-stu-id="56d77-137">string</span></span>|<span data-ttu-id="56d77-p105">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="56d77-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="56d77-141">italic</span><span class="sxs-lookup"><span data-stu-id="56d77-141">italic</span></span>|<span data-ttu-id="56d77-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="56d77-142">boolean</span></span>|<span data-ttu-id="56d77-143">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="56d77-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="56d77-144">name</span><span class="sxs-lookup"><span data-stu-id="56d77-144">name</span></span>|<span data-ttu-id="56d77-145">string</span><span class="sxs-lookup"><span data-stu-id="56d77-145">string</span></span>|<span data-ttu-id="56d77-146">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="56d77-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="56d77-147">size</span><span class="sxs-lookup"><span data-stu-id="56d77-147">size</span></span>|<span data-ttu-id="56d77-148">double</span><span class="sxs-lookup"><span data-stu-id="56d77-148">double</span></span>|<span data-ttu-id="56d77-149">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="56d77-149">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="56d77-150">underline</span><span class="sxs-lookup"><span data-stu-id="56d77-150">underline</span></span>|<span data-ttu-id="56d77-151">string</span><span class="sxs-lookup"><span data-stu-id="56d77-151">string</span></span>|<span data-ttu-id="56d77-p106">Art der auf die Schriftart angewendeten Unterstreichung. Mögliche Werte: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="56d77-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="56d77-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="56d77-154">Response</span></span>

<span data-ttu-id="56d77-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartFont](../resources/chartfont.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56d77-155">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56d77-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56d77-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56d77-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56d77-157">Request</span></span>
<span data-ttu-id="56d77-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56d77-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="56d77-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="56d77-159">Response</span></span>
<span data-ttu-id="56d77-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56d77-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfont-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
