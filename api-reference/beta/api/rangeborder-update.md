---
title: rangeborder aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.
ms.openlocfilehash: ab026d857c7fac591993469f87da662cb4bec064
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066115"
---
# <a name="update-rangeborder"></a><span data-ttu-id="268f9-103">rangeborder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="268f9-103">Update rangeborder</span></span>

> <span data-ttu-id="268f9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="268f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="268f9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="268f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="268f9-106">Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="268f9-106">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="268f9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="268f9-107">Permissions</span></span>
<span data-ttu-id="268f9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="268f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="268f9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="268f9-110">Permission type</span></span>      | <span data-ttu-id="268f9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="268f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="268f9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="268f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="268f9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="268f9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="268f9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="268f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="268f9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="268f9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="268f9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="268f9-116">Application</span></span> | <span data-ttu-id="268f9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="268f9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="268f9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="268f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="268f9-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="268f9-119">Optional request headers</span></span>
| <span data-ttu-id="268f9-120">Name</span><span class="sxs-lookup"><span data-stu-id="268f9-120">Name</span></span>       | <span data-ttu-id="268f9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="268f9-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="268f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="268f9-122">Authorization</span></span>  | <span data-ttu-id="268f9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="268f9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="268f9-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="268f9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="268f9-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="268f9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="268f9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="268f9-128">Request body</span></span>
<span data-ttu-id="268f9-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="268f9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="268f9-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="268f9-132">Property</span></span>     | <span data-ttu-id="268f9-133">Typ</span><span class="sxs-lookup"><span data-stu-id="268f9-133">Type</span></span>   |<span data-ttu-id="268f9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="268f9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="268f9-135">color</span><span class="sxs-lookup"><span data-stu-id="268f9-135">color</span></span>|<span data-ttu-id="268f9-136">string</span><span class="sxs-lookup"><span data-stu-id="268f9-136">string</span></span>|<span data-ttu-id="268f9-137">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="268f9-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="268f9-138">style</span><span class="sxs-lookup"><span data-stu-id="268f9-138">style</span></span>|<span data-ttu-id="268f9-139">string</span><span class="sxs-lookup"><span data-stu-id="268f9-139">string</span></span>|<span data-ttu-id="268f9-p106">Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="268f9-p106">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="268f9-142">weight</span><span class="sxs-lookup"><span data-stu-id="268f9-142">weight</span></span>|<span data-ttu-id="268f9-143">string</span><span class="sxs-lookup"><span data-stu-id="268f9-143">string</span></span>|<span data-ttu-id="268f9-p107">Gibt die Stärke des Rahmens um einen Bereich an. Mögliche Werte: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="268f9-p107">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="268f9-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="268f9-146">Response</span></span>

<span data-ttu-id="268f9-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="268f9-147">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="268f9-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="268f9-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="268f9-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="268f9-149">Request</span></span>
<span data-ttu-id="268f9-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="268f9-150">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="268f9-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="268f9-151">Response</span></span>
<span data-ttu-id="268f9-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="268f9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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