---
title: range aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Bereichsobjekts.
ms.openlocfilehash: 462649816075a31c51e89b5fb54320fb9d86830b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062876"
---
# <a name="update-range"></a><span data-ttu-id="9fb4e-103">range aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9fb4e-103">Update range</span></span>

> <span data-ttu-id="9fb4e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fb4e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fb4e-106">Dient zum Aktualisieren der Eigenschaften des Bereichsobjekts.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-106">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9fb4e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9fb4e-107">Permissions</span></span>
<span data-ttu-id="9fb4e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9fb4e-110">Permission type</span></span>      | <span data-ttu-id="9fb4e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9fb4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fb4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9fb4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9fb4e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fb4e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9fb4e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9fb4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb4e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fb4e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9fb4e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9fb4e-116">Application</span></span> | <span data-ttu-id="9fb4e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9fb4e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb4e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb4e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="9fb4e-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9fb4e-119">Optional request headers</span></span>
| <span data-ttu-id="9fb4e-120">Name</span><span class="sxs-lookup"><span data-stu-id="9fb4e-120">Name</span></span>       | <span data-ttu-id="9fb4e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb4e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9fb4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fb4e-122">Authorization</span></span>  | <span data-ttu-id="9fb4e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fb4e-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9fb4e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9fb4e-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fb4e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9fb4e-128">Request body</span></span>
<span data-ttu-id="9fb4e-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9fb4e-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fb4e-132">Property</span></span>     | <span data-ttu-id="9fb4e-133">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb4e-133">Type</span></span>   |<span data-ttu-id="9fb4e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb4e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fb4e-135">columnHidden</span><span class="sxs-lookup"><span data-stu-id="9fb4e-135">columnHidden</span></span>|<span data-ttu-id="9fb4e-136">boolean</span><span class="sxs-lookup"><span data-stu-id="9fb4e-136">boolean</span></span>|<span data-ttu-id="9fb4e-137">Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-137">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="9fb4e-138">formulas</span><span class="sxs-lookup"><span data-stu-id="9fb4e-138">formulas</span></span>|<span data-ttu-id="9fb4e-139">json</span><span class="sxs-lookup"><span data-stu-id="9fb4e-139">json</span></span>|<span data-ttu-id="9fb4e-140">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-140">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="9fb4e-141">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="9fb4e-141">formulasLocal</span></span>|<span data-ttu-id="9fb4e-142">json</span><span class="sxs-lookup"><span data-stu-id="9fb4e-142">json</span></span>|<span data-ttu-id="9fb4e-p106">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p106">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="9fb4e-145">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="9fb4e-145">formulasR1C1</span></span>|<span data-ttu-id="9fb4e-146">json</span><span class="sxs-lookup"><span data-stu-id="9fb4e-146">json</span></span>|<span data-ttu-id="9fb4e-147">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-147">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="9fb4e-148">numberFormat</span><span class="sxs-lookup"><span data-stu-id="9fb4e-148">numberFormat</span></span>|<span data-ttu-id="9fb4e-149">json</span><span class="sxs-lookup"><span data-stu-id="9fb4e-149">json</span></span>|<span data-ttu-id="9fb4e-150">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-150">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="9fb4e-151">rowHidden</span><span class="sxs-lookup"><span data-stu-id="9fb4e-151">rowHidden</span></span>|<span data-ttu-id="9fb4e-152">boolean</span><span class="sxs-lookup"><span data-stu-id="9fb4e-152">boolean</span></span>|<span data-ttu-id="9fb4e-153">Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-153">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="9fb4e-154">values</span><span class="sxs-lookup"><span data-stu-id="9fb4e-154">values</span></span>|<span data-ttu-id="9fb4e-155">json</span><span class="sxs-lookup"><span data-stu-id="9fb4e-155">json</span></span>|<span data-ttu-id="9fb4e-p107">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p107">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="9fb4e-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb4e-159">Response</span></span>

<span data-ttu-id="9fb4e-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-160">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9fb4e-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9fb4e-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fb4e-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb4e-162">Request</span></span>
<span data-ttu-id="9fb4e-p108">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es wird ein Bereich aktualisiert (Werte, Zahlenformate und Formeln) aktualisiert. Die `null`-Eingabe dient dazu, die API anzuweisen, die Zelle für diese bestimmte Eingabe zu ignorieren. Die Werte, Zahlenformate und Formeln können unabhängig aktualisiert im gleichen API-Aufruf miteinander kombiniert werden.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p108">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="9fb4e-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb4e-167">Response</span></span>
<span data-ttu-id="9fb4e-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fb4e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
