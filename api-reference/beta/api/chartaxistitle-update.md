---
title: ChartAxisTitle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartAxisTitle-Objekts.
ms.openlocfilehash: 4c76f10c150c15107be47f099c817284ecce6a55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060616"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="9fdb8-103">ChartAxisTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9fdb8-103">Update chartaxistitle</span></span>

> <span data-ttu-id="9fdb8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fdb8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fdb8-106">Dient zum Aktualisieren der Eigenschaften des ChartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-106">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9fdb8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9fdb8-107">Permissions</span></span>
<span data-ttu-id="9fdb8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fdb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fdb8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9fdb8-110">Permission type</span></span>      | <span data-ttu-id="9fdb8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9fdb8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fdb8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9fdb8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9fdb8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fdb8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9fdb8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9fdb8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fdb8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fdb8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9fdb8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9fdb8-116">Application</span></span> | <span data-ttu-id="9fdb8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9fdb8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fdb8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fdb8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="9fdb8-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9fdb8-119">Optional request headers</span></span>
| <span data-ttu-id="9fdb8-120">Name</span><span class="sxs-lookup"><span data-stu-id="9fdb8-120">Name</span></span>       | <span data-ttu-id="9fdb8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fdb8-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9fdb8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fdb8-122">Authorization</span></span>  | <span data-ttu-id="9fdb8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fdb8-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9fdb8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9fdb8-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fdb8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9fdb8-128">Request body</span></span>
<span data-ttu-id="9fdb8-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9fdb8-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fdb8-132">Property</span></span>     | <span data-ttu-id="9fdb8-133">Typ</span><span class="sxs-lookup"><span data-stu-id="9fdb8-133">Type</span></span>   |<span data-ttu-id="9fdb8-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fdb8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fdb8-135">text</span><span class="sxs-lookup"><span data-stu-id="9fdb8-135">text</span></span>|<span data-ttu-id="9fdb8-136">string</span><span class="sxs-lookup"><span data-stu-id="9fdb8-136">string</span></span>|<span data-ttu-id="9fdb8-137">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-137">Represents the axis title.</span></span>|
|<span data-ttu-id="9fdb8-138">visible</span><span class="sxs-lookup"><span data-stu-id="9fdb8-138">visible</span></span>|<span data-ttu-id="9fdb8-139">boolean</span><span class="sxs-lookup"><span data-stu-id="9fdb8-139">boolean</span></span>|<span data-ttu-id="9fdb8-140">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-140">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="9fdb8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fdb8-141">Response</span></span>

<span data-ttu-id="9fdb8-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartAxisTitle](../resources/chartaxistitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-142">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9fdb8-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9fdb8-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fdb8-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fdb8-144">Request</span></span>
<span data-ttu-id="9fdb8-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9fdb8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fdb8-146">Response</span></span>
<span data-ttu-id="9fdb8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fdb8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->