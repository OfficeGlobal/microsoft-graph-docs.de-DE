---
title: rangefill aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangefill-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 166550959cd6ce4b481b85d4dbff344f1a070ae5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836715"
---
# <a name="update-rangefill"></a><span data-ttu-id="3e197-103">rangefill aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3e197-103">Update rangefill</span></span>

> <span data-ttu-id="3e197-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e197-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e197-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e197-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e197-106">Dient zum Aktualisieren der Eigenschaften des rangefill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e197-106">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e197-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e197-107">Permissions</span></span>
<span data-ttu-id="3e197-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e197-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e197-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e197-110">Permission type</span></span>      | <span data-ttu-id="3e197-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e197-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e197-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e197-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e197-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e197-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e197-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e197-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e197-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e197-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e197-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e197-116">Application</span></span> | <span data-ttu-id="3e197-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e197-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e197-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e197-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="3e197-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e197-119">Optional request headers</span></span>
| <span data-ttu-id="3e197-120">Name</span><span class="sxs-lookup"><span data-stu-id="3e197-120">Name</span></span>       | <span data-ttu-id="3e197-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e197-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3e197-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e197-122">Authorization</span></span>  | <span data-ttu-id="3e197-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e197-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e197-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3e197-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e197-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3e197-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e197-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e197-128">Request body</span></span>
<span data-ttu-id="3e197-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="3e197-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e197-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e197-132">Property</span></span>     | <span data-ttu-id="3e197-133">Typ</span><span class="sxs-lookup"><span data-stu-id="3e197-133">Type</span></span>   |<span data-ttu-id="3e197-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e197-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e197-135">color</span><span class="sxs-lookup"><span data-stu-id="3e197-135">color</span></span>|<span data-ttu-id="3e197-136">string</span><span class="sxs-lookup"><span data-stu-id="3e197-136">string</span></span>|<span data-ttu-id="3e197-137">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="3e197-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="3e197-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e197-138">Response</span></span>

<span data-ttu-id="3e197-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFill](../resources/rangefill.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e197-139">If successful, this method returns a `200 OK` response code and updated [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e197-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e197-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e197-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e197-141">Request</span></span>
<span data-ttu-id="3e197-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e197-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="3e197-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e197-143">Response</span></span>
<span data-ttu-id="3e197-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e197-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
