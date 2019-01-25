---
title: ChartAxisTitle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartAxisTitle-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6f8e1ba265246678bb930c1135fbf465147c1c7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522616"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="850e0-103">ChartAxisTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="850e0-103">Update chartaxistitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="850e0-104">Dient zum Aktualisieren der Eigenschaften des ChartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="850e0-104">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="850e0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="850e0-105">Permissions</span></span>
<span data-ttu-id="850e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="850e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="850e0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="850e0-108">Permission type</span></span>      | <span data-ttu-id="850e0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="850e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="850e0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="850e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="850e0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="850e0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="850e0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="850e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="850e0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="850e0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="850e0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="850e0-114">Application</span></span> | <span data-ttu-id="850e0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="850e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="850e0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="850e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="850e0-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="850e0-117">Optional request headers</span></span>
| <span data-ttu-id="850e0-118">Name</span><span class="sxs-lookup"><span data-stu-id="850e0-118">Name</span></span>       | <span data-ttu-id="850e0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="850e0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="850e0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="850e0-120">Authorization</span></span>  | <span data-ttu-id="850e0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="850e0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="850e0-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="850e0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="850e0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="850e0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="850e0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="850e0-126">Request body</span></span>
<span data-ttu-id="850e0-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="850e0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="850e0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="850e0-130">Property</span></span>     | <span data-ttu-id="850e0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="850e0-131">Type</span></span>   |<span data-ttu-id="850e0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="850e0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="850e0-133">text</span><span class="sxs-lookup"><span data-stu-id="850e0-133">text</span></span>|<span data-ttu-id="850e0-134">string</span><span class="sxs-lookup"><span data-stu-id="850e0-134">string</span></span>|<span data-ttu-id="850e0-135">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="850e0-135">Represents the axis title.</span></span>|
|<span data-ttu-id="850e0-136">visible</span><span class="sxs-lookup"><span data-stu-id="850e0-136">visible</span></span>|<span data-ttu-id="850e0-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="850e0-137">boolean</span></span>|<span data-ttu-id="850e0-138">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="850e0-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="850e0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="850e0-139">Response</span></span>

<span data-ttu-id="850e0-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartAxisTitle](../resources/chartaxistitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="850e0-140">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="850e0-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="850e0-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="850e0-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="850e0-142">Request</span></span>
<span data-ttu-id="850e0-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="850e0-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="850e0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="850e0-144">Response</span></span>
<span data-ttu-id="850e0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="850e0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
