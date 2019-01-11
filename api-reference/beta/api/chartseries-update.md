---
title: ChartSeries aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartSeries-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4b7d80aca2aa0d98d37fabd7820f0d6752d9da3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833278"
---
# <a name="update-chartseries"></a><span data-ttu-id="776bf-103">ChartSeries aktualisieren</span><span class="sxs-lookup"><span data-stu-id="776bf-103">Update chartseries</span></span>

> <span data-ttu-id="776bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="776bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="776bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="776bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="776bf-106">Dient zum Aktualisieren der Eigenschaften des ChartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="776bf-106">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="776bf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="776bf-107">Permissions</span></span>
<span data-ttu-id="776bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="776bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="776bf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="776bf-110">Permission type</span></span>      | <span data-ttu-id="776bf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="776bf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="776bf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="776bf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="776bf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="776bf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="776bf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="776bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="776bf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="776bf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="776bf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="776bf-116">Application</span></span> | <span data-ttu-id="776bf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="776bf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="776bf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="776bf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="776bf-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="776bf-119">Optional request headers</span></span>
| <span data-ttu-id="776bf-120">Name</span><span class="sxs-lookup"><span data-stu-id="776bf-120">Name</span></span>       | <span data-ttu-id="776bf-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="776bf-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="776bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="776bf-122">Authorization</span></span>  | <span data-ttu-id="776bf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="776bf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="776bf-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="776bf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="776bf-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="776bf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="776bf-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="776bf-128">Request body</span></span>
<span data-ttu-id="776bf-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="776bf-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="776bf-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="776bf-132">Property</span></span>     | <span data-ttu-id="776bf-133">Typ</span><span class="sxs-lookup"><span data-stu-id="776bf-133">Type</span></span>   |<span data-ttu-id="776bf-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="776bf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="776bf-135">name</span><span class="sxs-lookup"><span data-stu-id="776bf-135">name</span></span>|<span data-ttu-id="776bf-136">string</span><span class="sxs-lookup"><span data-stu-id="776bf-136">string</span></span>|<span data-ttu-id="776bf-137">Gibt den Namen einer Datenreihe in einem Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="776bf-137">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="776bf-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="776bf-138">Response</span></span>

<span data-ttu-id="776bf-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="776bf-139">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="776bf-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="776bf-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="776bf-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="776bf-141">Request</span></span>
<span data-ttu-id="776bf-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="776bf-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="776bf-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="776bf-143">Response</span></span>
<span data-ttu-id="776bf-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="776bf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
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
