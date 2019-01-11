---
title: rangeborder aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a85bd70b3e8448dd460c2d572ab319142c17bd52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818291"
---
# <a name="update-rangeborder"></a><span data-ttu-id="8eba1-103">rangeborder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8eba1-103">Update rangeborder</span></span>

<span data-ttu-id="8eba1-104">Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8eba1-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8eba1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8eba1-105">Permissions</span></span>
<span data-ttu-id="8eba1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eba1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8eba1-108">Permission type</span></span>      | <span data-ttu-id="8eba1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8eba1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eba1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8eba1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8eba1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8eba1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8eba1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8eba1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eba1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8eba1-113">Not supported.</span></span>    |
|<span data-ttu-id="8eba1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8eba1-114">Application</span></span> | <span data-ttu-id="8eba1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8eba1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8eba1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8eba1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8eba1-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8eba1-117">Optional request headers</span></span>
| <span data-ttu-id="8eba1-118">Name</span><span class="sxs-lookup"><span data-stu-id="8eba1-118">Name</span></span>       | <span data-ttu-id="8eba1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8eba1-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8eba1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eba1-120">Authorization</span></span>  | <span data-ttu-id="8eba1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8eba1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8eba1-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8eba1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8eba1-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8eba1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eba1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8eba1-126">Request body</span></span>
<span data-ttu-id="8eba1-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="8eba1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8eba1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8eba1-130">Property</span></span>     | <span data-ttu-id="8eba1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8eba1-131">Type</span></span>   |<span data-ttu-id="8eba1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8eba1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eba1-133">color</span><span class="sxs-lookup"><span data-stu-id="8eba1-133">color</span></span>|<span data-ttu-id="8eba1-134">string</span><span class="sxs-lookup"><span data-stu-id="8eba1-134">string</span></span>|<span data-ttu-id="8eba1-135">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="8eba1-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="8eba1-136">style</span><span class="sxs-lookup"><span data-stu-id="8eba1-136">style</span></span>|<span data-ttu-id="8eba1-137">string</span><span class="sxs-lookup"><span data-stu-id="8eba1-137">string</span></span>|<span data-ttu-id="8eba1-138">Eine der Konstanten der Linienart die Linienart für den Rahmen angeben.</span><span class="sxs-lookup"><span data-stu-id="8eba1-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="8eba1-139">Die möglichen Werte sind: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="8eba1-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="8eba1-140">weight</span><span class="sxs-lookup"><span data-stu-id="8eba1-140">weight</span></span>|<span data-ttu-id="8eba1-141">string</span><span class="sxs-lookup"><span data-stu-id="8eba1-141">string</span></span>|<span data-ttu-id="8eba1-142">Gibt die Stärke des Rahmens um einen Bereich an.</span><span class="sxs-lookup"><span data-stu-id="8eba1-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="8eba1-143">Die möglichen Werte sind: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="8eba1-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="8eba1-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="8eba1-144">Response</span></span>

<span data-ttu-id="8eba1-145">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookRangeBorder](../resources/rangeborder.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8eba1-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8eba1-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8eba1-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8eba1-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8eba1-147">Request</span></span>
<span data-ttu-id="8eba1-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8eba1-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="8eba1-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8eba1-149">Response</span></span>
<span data-ttu-id="8eba1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8eba1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
