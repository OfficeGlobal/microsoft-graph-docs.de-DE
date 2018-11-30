---
title: ChartLineFormat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartLineFormat-Objekts.
ms.openlocfilehash: 9bd1a267a463b9ba7a12f743b25571d2825b09a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058045"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="2be7d-103">ChartLineFormat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2be7d-103">Update chartlineformat</span></span>

> <span data-ttu-id="2be7d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2be7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2be7d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2be7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2be7d-106">Dient zum Aktualisieren der Eigenschaften des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2be7d-106">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2be7d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2be7d-107">Permissions</span></span>
<span data-ttu-id="2be7d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2be7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2be7d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2be7d-110">Permission type</span></span>      | <span data-ttu-id="2be7d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2be7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2be7d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2be7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2be7d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2be7d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2be7d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2be7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2be7d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2be7d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2be7d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2be7d-116">Application</span></span> | <span data-ttu-id="2be7d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2be7d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2be7d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2be7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="2be7d-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2be7d-119">Optional request headers</span></span>
| <span data-ttu-id="2be7d-120">Name</span><span class="sxs-lookup"><span data-stu-id="2be7d-120">Name</span></span>       | <span data-ttu-id="2be7d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2be7d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2be7d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2be7d-122">Authorization</span></span>  | <span data-ttu-id="2be7d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2be7d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2be7d-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2be7d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2be7d-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2be7d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2be7d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2be7d-128">Request body</span></span>
<span data-ttu-id="2be7d-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2be7d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2be7d-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2be7d-132">Property</span></span>     | <span data-ttu-id="2be7d-133">Typ</span><span class="sxs-lookup"><span data-stu-id="2be7d-133">Type</span></span>   |<span data-ttu-id="2be7d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2be7d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2be7d-135">color</span><span class="sxs-lookup"><span data-stu-id="2be7d-135">color</span></span>|<span data-ttu-id="2be7d-136">string</span><span class="sxs-lookup"><span data-stu-id="2be7d-136">string</span></span>|<span data-ttu-id="2be7d-137">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="2be7d-137">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="2be7d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2be7d-138">Response</span></span>

<span data-ttu-id="2be7d-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLineFormat](../resources/chartlineformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2be7d-139">If successful, this method returns a `200 OK` response code and updated [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2be7d-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2be7d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2be7d-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2be7d-141">Request</span></span>
<span data-ttu-id="2be7d-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2be7d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="2be7d-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2be7d-143">Response</span></span>
<span data-ttu-id="2be7d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2be7d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->