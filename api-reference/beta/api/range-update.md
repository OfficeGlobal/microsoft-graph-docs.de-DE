---
title: range aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Bereichsobjekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f4a1cce20e8d11879dc4fc11b55feee5b02cfb49
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789655"
---
# <a name="update-range"></a><span data-ttu-id="1f12a-103">range aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f12a-103">Update range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f12a-104">Dient zum Aktualisieren der Eigenschaften des Bereichsobjekts.</span><span class="sxs-lookup"><span data-stu-id="1f12a-104">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f12a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f12a-105">Permissions</span></span>
<span data-ttu-id="1f12a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f12a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f12a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f12a-108">Permission type</span></span>      | <span data-ttu-id="1f12a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f12a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f12a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f12a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f12a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f12a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f12a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f12a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f12a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f12a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f12a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f12a-114">Application</span></span> | <span data-ttu-id="1f12a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f12a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f12a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f12a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="1f12a-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f12a-117">Optional request headers</span></span>
| <span data-ttu-id="1f12a-118">Name</span><span class="sxs-lookup"><span data-stu-id="1f12a-118">Name</span></span>       | <span data-ttu-id="1f12a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f12a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1f12a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f12a-120">Authorization</span></span>  | <span data-ttu-id="1f12a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f12a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1f12a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f12a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f12a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f12a-126">Request body</span></span>
<span data-ttu-id="1f12a-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f12a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f12a-130">Property</span></span>     | <span data-ttu-id="1f12a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1f12a-131">Type</span></span>   |<span data-ttu-id="1f12a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f12a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f12a-133">columnHidden</span><span class="sxs-lookup"><span data-stu-id="1f12a-133">columnHidden</span></span>|<span data-ttu-id="1f12a-134">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1f12a-134">boolean</span></span>|<span data-ttu-id="1f12a-135">Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="1f12a-135">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="1f12a-136">formulas</span><span class="sxs-lookup"><span data-stu-id="1f12a-136">formulas</span></span>|<span data-ttu-id="1f12a-137">Json</span><span class="sxs-lookup"><span data-stu-id="1f12a-137">Json</span></span>|<span data-ttu-id="1f12a-138">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="1f12a-138">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="1f12a-139">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="1f12a-139">formulasLocal</span></span>|<span data-ttu-id="1f12a-140">Json</span><span class="sxs-lookup"><span data-stu-id="1f12a-140">Json</span></span>|<span data-ttu-id="1f12a-p105">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="1f12a-143">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="1f12a-143">formulasR1C1</span></span>|<span data-ttu-id="1f12a-144">Json</span><span class="sxs-lookup"><span data-stu-id="1f12a-144">Json</span></span>|<span data-ttu-id="1f12a-145">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="1f12a-145">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="1f12a-146">numberFormat</span><span class="sxs-lookup"><span data-stu-id="1f12a-146">numberFormat</span></span>|<span data-ttu-id="1f12a-147">Json</span><span class="sxs-lookup"><span data-stu-id="1f12a-147">Json</span></span>|<span data-ttu-id="1f12a-148">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.</span><span class="sxs-lookup"><span data-stu-id="1f12a-148">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="1f12a-149">rowHidden</span><span class="sxs-lookup"><span data-stu-id="1f12a-149">rowHidden</span></span>|<span data-ttu-id="1f12a-150">boolean</span><span class="sxs-lookup"><span data-stu-id="1f12a-150">boolean</span></span>|<span data-ttu-id="1f12a-151">Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="1f12a-151">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="1f12a-152">values</span><span class="sxs-lookup"><span data-stu-id="1f12a-152">values</span></span>|<span data-ttu-id="1f12a-153">Json</span><span class="sxs-lookup"><span data-stu-id="1f12a-153">Json</span></span>|<span data-ttu-id="1f12a-p106">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="1f12a-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f12a-157">Response</span></span>

<span data-ttu-id="1f12a-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f12a-158">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f12a-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f12a-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f12a-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f12a-160">Request</span></span>
<span data-ttu-id="1f12a-p107">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es wird ein Bereich aktualisiert (Werte, Zahlenformate und Formeln) aktualisiert. Die `null`-Eingabe dient dazu, die API anzuweisen, die Zelle für diese bestimmte Eingabe zu ignorieren. Die Werte, Zahlenformate und Formeln können unabhängig aktualisiert im gleichen API-Aufruf miteinander kombiniert werden.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="1f12a-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f12a-165">Response</span></span>
<span data-ttu-id="1f12a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f12a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
