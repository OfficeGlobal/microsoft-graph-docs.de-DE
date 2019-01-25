---
title: rangeborder aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8b0aae47251aa9967501ce18d107cdd4c1b7ddd9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508132"
---
# <a name="update-rangeborder"></a><span data-ttu-id="67562-103">rangeborder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="67562-103">Update rangeborder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67562-104">Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="67562-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67562-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67562-105">Permissions</span></span>
<span data-ttu-id="67562-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67562-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67562-108">Permission type</span></span>      | <span data-ttu-id="67562-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67562-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67562-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67562-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67562-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67562-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67562-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67562-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67562-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67562-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67562-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67562-114">Application</span></span> | <span data-ttu-id="67562-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67562-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67562-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67562-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="67562-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67562-117">Optional request headers</span></span>
| <span data-ttu-id="67562-118">Name</span><span class="sxs-lookup"><span data-stu-id="67562-118">Name</span></span>       | <span data-ttu-id="67562-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67562-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="67562-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="67562-120">Authorization</span></span>  | <span data-ttu-id="67562-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67562-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67562-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="67562-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="67562-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="67562-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67562-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67562-126">Request body</span></span>
<span data-ttu-id="67562-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="67562-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67562-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67562-130">Property</span></span>     | <span data-ttu-id="67562-131">Typ</span><span class="sxs-lookup"><span data-stu-id="67562-131">Type</span></span>   |<span data-ttu-id="67562-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67562-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67562-133">color</span><span class="sxs-lookup"><span data-stu-id="67562-133">color</span></span>|<span data-ttu-id="67562-134">string</span><span class="sxs-lookup"><span data-stu-id="67562-134">string</span></span>|<span data-ttu-id="67562-135">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="67562-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="67562-136">style</span><span class="sxs-lookup"><span data-stu-id="67562-136">style</span></span>|<span data-ttu-id="67562-137">string</span><span class="sxs-lookup"><span data-stu-id="67562-137">string</span></span>|<span data-ttu-id="67562-p105">Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="67562-p105">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="67562-140">weight</span><span class="sxs-lookup"><span data-stu-id="67562-140">weight</span></span>|<span data-ttu-id="67562-141">string</span><span class="sxs-lookup"><span data-stu-id="67562-141">string</span></span>|<span data-ttu-id="67562-p106">Gibt die Stärke des Rahmens um einen Bereich an. Mögliche Werte: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="67562-p106">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="67562-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="67562-144">Response</span></span>

<span data-ttu-id="67562-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67562-145">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67562-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67562-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67562-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67562-147">Request</span></span>
<span data-ttu-id="67562-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67562-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="67562-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="67562-149">Response</span></span>
<span data-ttu-id="67562-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67562-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeborder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
