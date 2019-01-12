---
title: rangeborder aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ac989724f0e950a079479c8285cea64e2e24a8fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933777"
---
# <a name="update-rangeborder"></a><span data-ttu-id="58325-103">rangeborder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="58325-103">Update rangeborder</span></span>

> <span data-ttu-id="58325-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="58325-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58325-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58325-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58325-106">Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="58325-106">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="58325-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58325-107">Permissions</span></span>
<span data-ttu-id="58325-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58325-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58325-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58325-110">Permission type</span></span>      | <span data-ttu-id="58325-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58325-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58325-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58325-112">Delegated (work or school account)</span></span> | <span data-ttu-id="58325-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58325-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58325-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58325-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58325-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58325-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58325-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58325-116">Application</span></span> | <span data-ttu-id="58325-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58325-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58325-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58325-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="58325-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58325-119">Optional request headers</span></span>
| <span data-ttu-id="58325-120">Name</span><span class="sxs-lookup"><span data-stu-id="58325-120">Name</span></span>       | <span data-ttu-id="58325-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58325-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="58325-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58325-122">Authorization</span></span>  | <span data-ttu-id="58325-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58325-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58325-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="58325-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="58325-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="58325-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58325-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58325-128">Request body</span></span>
<span data-ttu-id="58325-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="58325-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="58325-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58325-132">Property</span></span>     | <span data-ttu-id="58325-133">Typ</span><span class="sxs-lookup"><span data-stu-id="58325-133">Type</span></span>   |<span data-ttu-id="58325-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58325-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58325-135">color</span><span class="sxs-lookup"><span data-stu-id="58325-135">color</span></span>|<span data-ttu-id="58325-136">string</span><span class="sxs-lookup"><span data-stu-id="58325-136">string</span></span>|<span data-ttu-id="58325-137">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="58325-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="58325-138">style</span><span class="sxs-lookup"><span data-stu-id="58325-138">style</span></span>|<span data-ttu-id="58325-139">string</span><span class="sxs-lookup"><span data-stu-id="58325-139">string</span></span>|<span data-ttu-id="58325-p106">Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="58325-p106">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="58325-142">weight</span><span class="sxs-lookup"><span data-stu-id="58325-142">weight</span></span>|<span data-ttu-id="58325-143">string</span><span class="sxs-lookup"><span data-stu-id="58325-143">string</span></span>|<span data-ttu-id="58325-p107">Gibt die Stärke des Rahmens um einen Bereich an. Mögliche Werte: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="58325-p107">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="58325-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="58325-146">Response</span></span>

<span data-ttu-id="58325-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58325-147">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58325-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58325-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58325-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58325-149">Request</span></span>
<span data-ttu-id="58325-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58325-150">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="58325-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="58325-151">Response</span></span>
<span data-ttu-id="58325-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58325-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
