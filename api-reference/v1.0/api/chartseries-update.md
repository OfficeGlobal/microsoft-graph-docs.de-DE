---
title: ChartSeries aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartSeries-Objekts.
ms.openlocfilehash: ea238fcf9cd3b03b99527bb0f9ab11440a8ed111
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27015967"
---
# <a name="update-chartseries"></a><span data-ttu-id="d05db-103">ChartSeries aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d05db-103">Update chartseries</span></span>

<span data-ttu-id="d05db-104">Dient zum Aktualisieren der Eigenschaften des ChartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d05db-104">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d05db-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d05db-105">Permissions</span></span>
<span data-ttu-id="d05db-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d05db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d05db-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d05db-108">Permission type</span></span>      | <span data-ttu-id="d05db-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d05db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d05db-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d05db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d05db-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d05db-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d05db-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d05db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d05db-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d05db-113">Not supported.</span></span>    |
|<span data-ttu-id="d05db-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d05db-114">Application</span></span> | <span data-ttu-id="d05db-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d05db-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d05db-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d05db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d05db-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d05db-117">Optional request headers</span></span>
| <span data-ttu-id="d05db-118">Name</span><span class="sxs-lookup"><span data-stu-id="d05db-118">Name</span></span>       | <span data-ttu-id="d05db-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d05db-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d05db-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d05db-120">Authorization</span></span>  | <span data-ttu-id="d05db-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d05db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d05db-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d05db-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d05db-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d05db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d05db-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d05db-126">Request body</span></span>
<span data-ttu-id="d05db-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d05db-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d05db-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d05db-130">Property</span></span>     | <span data-ttu-id="d05db-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d05db-131">Type</span></span>   |<span data-ttu-id="d05db-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d05db-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d05db-133">name</span><span class="sxs-lookup"><span data-stu-id="d05db-133">name</span></span>|<span data-ttu-id="d05db-134">string</span><span class="sxs-lookup"><span data-stu-id="d05db-134">string</span></span>|<span data-ttu-id="d05db-135">Gibt den Namen einer Datenreihe in einem Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="d05db-135">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="d05db-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d05db-136">Response</span></span>

<span data-ttu-id="d05db-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartSeries](../resources/chartseries.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d05db-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d05db-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d05db-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d05db-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d05db-139">Request</span></span>
<span data-ttu-id="d05db-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d05db-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="d05db-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d05db-141">Response</span></span>
<span data-ttu-id="d05db-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d05db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->