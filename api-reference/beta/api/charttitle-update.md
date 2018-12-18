---
title: ChartTitle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.
author: lumine2008
ms.openlocfilehash: 2a3dd005b7932325685e9efa23acf1accd9320f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353368"
---
# <a name="update-charttitle"></a><span data-ttu-id="6f36c-103">ChartTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6f36c-103">Update charttitle</span></span>

> <span data-ttu-id="6f36c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f36c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f36c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f36c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f36c-106">Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f36c-106">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f36c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f36c-107">Permissions</span></span>
<span data-ttu-id="6f36c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f36c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f36c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f36c-110">Permission type</span></span>      | <span data-ttu-id="6f36c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f36c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f36c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f36c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f36c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f36c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6f36c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f36c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f36c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f36c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6f36c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f36c-116">Application</span></span> | <span data-ttu-id="6f36c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f36c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f36c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f36c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="6f36c-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f36c-119">Optional request headers</span></span>
| <span data-ttu-id="6f36c-120">Name</span><span class="sxs-lookup"><span data-stu-id="6f36c-120">Name</span></span>       | <span data-ttu-id="6f36c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f36c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6f36c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f36c-122">Authorization</span></span>  | <span data-ttu-id="6f36c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f36c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f36c-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="6f36c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6f36c-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="6f36c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f36c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f36c-128">Request body</span></span>
<span data-ttu-id="6f36c-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="6f36c-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6f36c-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f36c-132">Property</span></span>     | <span data-ttu-id="6f36c-133">Typ</span><span class="sxs-lookup"><span data-stu-id="6f36c-133">Type</span></span>   |<span data-ttu-id="6f36c-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f36c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f36c-135">Overlay</span><span class="sxs-lookup"><span data-stu-id="6f36c-135">overlay</span></span>|<span data-ttu-id="6f36c-136">boolean</span><span class="sxs-lookup"><span data-stu-id="6f36c-136">boolean</span></span>|<span data-ttu-id="6f36c-137">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="6f36c-137">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="6f36c-138">text</span><span class="sxs-lookup"><span data-stu-id="6f36c-138">text</span></span>|<span data-ttu-id="6f36c-139">string</span><span class="sxs-lookup"><span data-stu-id="6f36c-139">string</span></span>|<span data-ttu-id="6f36c-140">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="6f36c-140">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="6f36c-141">visible</span><span class="sxs-lookup"><span data-stu-id="6f36c-141">visible</span></span>|<span data-ttu-id="6f36c-142">boolean</span><span class="sxs-lookup"><span data-stu-id="6f36c-142">boolean</span></span>|<span data-ttu-id="6f36c-143">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="6f36c-143">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="6f36c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f36c-144">Response</span></span>

<span data-ttu-id="6f36c-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartTitle](../resources/charttitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f36c-145">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f36c-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f36c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f36c-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f36c-147">Request</span></span>
<span data-ttu-id="6f36c-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f36c-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6f36c-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f36c-149">Response</span></span>
<span data-ttu-id="6f36c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f36c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->