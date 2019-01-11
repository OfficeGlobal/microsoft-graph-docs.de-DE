---
title: ChartAxis aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartAxis-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 843aad2b3d6ea822078834439a085ba4bb10bf8b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813699"
---
# <a name="update-chartaxis"></a><span data-ttu-id="67b55-103">ChartAxis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="67b55-103">Update chartaxis</span></span>

> <span data-ttu-id="67b55-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67b55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67b55-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67b55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67b55-106">Dient zum Aktualisieren der Eigenschaften des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="67b55-106">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67b55-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67b55-107">Permissions</span></span>
<span data-ttu-id="67b55-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67b55-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67b55-110">Permission type</span></span>      | <span data-ttu-id="67b55-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67b55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67b55-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67b55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="67b55-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67b55-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67b55-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67b55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67b55-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67b55-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67b55-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67b55-116">Application</span></span> | <span data-ttu-id="67b55-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67b55-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67b55-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67b55-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="67b55-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67b55-119">Optional request headers</span></span>
| <span data-ttu-id="67b55-120">Name</span><span class="sxs-lookup"><span data-stu-id="67b55-120">Name</span></span>       | <span data-ttu-id="67b55-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67b55-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="67b55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67b55-122">Authorization</span></span>  | <span data-ttu-id="67b55-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67b55-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67b55-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="67b55-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="67b55-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="67b55-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b55-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67b55-128">Request body</span></span>
<span data-ttu-id="67b55-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="67b55-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67b55-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67b55-132">Property</span></span>     | <span data-ttu-id="67b55-133">Typ</span><span class="sxs-lookup"><span data-stu-id="67b55-133">Type</span></span>   |<span data-ttu-id="67b55-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67b55-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67b55-135">majorUnit</span><span class="sxs-lookup"><span data-stu-id="67b55-135">majorUnit</span></span>|<span data-ttu-id="67b55-136">object</span><span class="sxs-lookup"><span data-stu-id="67b55-136">object</span></span>|<span data-ttu-id="67b55-p106">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="67b55-p106">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="67b55-140">maximum</span><span class="sxs-lookup"><span data-stu-id="67b55-140">maximum</span></span>|<span data-ttu-id="67b55-141">object</span><span class="sxs-lookup"><span data-stu-id="67b55-141">object</span></span>|<span data-ttu-id="67b55-p107">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="67b55-p107">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="67b55-145">minimum</span><span class="sxs-lookup"><span data-stu-id="67b55-145">minimum</span></span>|<span data-ttu-id="67b55-146">object</span><span class="sxs-lookup"><span data-stu-id="67b55-146">object</span></span>|<span data-ttu-id="67b55-p108">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="67b55-p108">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="67b55-150">minorUnit</span><span class="sxs-lookup"><span data-stu-id="67b55-150">minorUnit</span></span>|<span data-ttu-id="67b55-151">object</span><span class="sxs-lookup"><span data-stu-id="67b55-151">object</span></span>|<span data-ttu-id="67b55-p109">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="67b55-p109">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="67b55-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="67b55-155">Response</span></span>

<span data-ttu-id="67b55-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartAxis](../resources/chartaxis.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67b55-156">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67b55-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67b55-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67b55-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67b55-158">Request</span></span>
<span data-ttu-id="67b55-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67b55-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="67b55-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="67b55-160">Response</span></span>
<span data-ttu-id="67b55-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67b55-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
