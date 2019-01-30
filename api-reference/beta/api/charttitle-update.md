---
title: ChartTitle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e67790672f2e31baaacd0eba500684f7b2275e97
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640378"
---
# <a name="update-charttitle"></a><span data-ttu-id="e8711-103">ChartTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e8711-103">Update charttitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8711-104">Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8711-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8711-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8711-105">Permissions</span></span>
<span data-ttu-id="e8711-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8711-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8711-108">Permission type</span></span>      | <span data-ttu-id="e8711-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8711-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8711-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8711-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8711-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8711-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8711-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8711-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8711-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8711-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8711-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8711-114">Application</span></span> | <span data-ttu-id="e8711-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8711-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8711-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8711-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="e8711-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8711-117">Optional request headers</span></span>
| <span data-ttu-id="e8711-118">Name</span><span class="sxs-lookup"><span data-stu-id="e8711-118">Name</span></span>       | <span data-ttu-id="e8711-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8711-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e8711-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8711-120">Authorization</span></span>  | <span data-ttu-id="e8711-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8711-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8711-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e8711-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8711-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e8711-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8711-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8711-126">Request body</span></span>
<span data-ttu-id="e8711-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="e8711-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8711-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8711-130">Property</span></span>     | <span data-ttu-id="e8711-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e8711-131">Type</span></span>   |<span data-ttu-id="e8711-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8711-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8711-133">Overlay</span><span class="sxs-lookup"><span data-stu-id="e8711-133">overlay</span></span>|<span data-ttu-id="e8711-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e8711-134">boolean</span></span>|<span data-ttu-id="e8711-135">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="e8711-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="e8711-136">text</span><span class="sxs-lookup"><span data-stu-id="e8711-136">text</span></span>|<span data-ttu-id="e8711-137">string</span><span class="sxs-lookup"><span data-stu-id="e8711-137">string</span></span>|<span data-ttu-id="e8711-138">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="e8711-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="e8711-139">visible</span><span class="sxs-lookup"><span data-stu-id="e8711-139">visible</span></span>|<span data-ttu-id="e8711-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e8711-140">boolean</span></span>|<span data-ttu-id="e8711-141">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="e8711-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="e8711-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8711-142">Response</span></span>

<span data-ttu-id="e8711-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartTitle](../resources/charttitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8711-143">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8711-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8711-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8711-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8711-145">Request</span></span>
<span data-ttu-id="e8711-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8711-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="e8711-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8711-147">Response</span></span>
<span data-ttu-id="e8711-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8711-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/charttitle-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
