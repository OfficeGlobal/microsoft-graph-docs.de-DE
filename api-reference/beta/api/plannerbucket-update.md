---
title: plannerBucket aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannerbucket**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 193b6ee4fcb26d0b4933a4458aa4c8c3891882b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940638"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="039ff-103">plannerBucket aktualisieren</span><span class="sxs-lookup"><span data-stu-id="039ff-103">Update plannerbucket</span></span>

> <span data-ttu-id="039ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="039ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="039ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="039ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="039ff-106">Dient zum Aktualisieren der Eigenschaften eines **plannerbucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="039ff-106">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="039ff-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="039ff-107">Permissions</span></span>
<span data-ttu-id="039ff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="039ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="039ff-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="039ff-110">Permission type</span></span>      | <span data-ttu-id="039ff-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="039ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="039ff-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="039ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="039ff-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039ff-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="039ff-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="039ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="039ff-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="039ff-115">Not supported.</span></span>    |
|<span data-ttu-id="039ff-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="039ff-116">Application</span></span> | <span data-ttu-id="039ff-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="039ff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="039ff-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="039ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="039ff-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="039ff-119">Optional request headers</span></span>
| <span data-ttu-id="039ff-120">Name</span><span class="sxs-lookup"><span data-stu-id="039ff-120">Name</span></span>       | <span data-ttu-id="039ff-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="039ff-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="039ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="039ff-122">Authorization</span></span>  | <span data-ttu-id="039ff-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="039ff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="039ff-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="039ff-125">If-Match</span></span>  | <span data-ttu-id="039ff-p104">Letzter bekannter ETag-Wert für den zu aktualisierenden **plannerBucket**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="039ff-p104">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="039ff-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="039ff-128">Request body</span></span>
<span data-ttu-id="039ff-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="039ff-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="039ff-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="039ff-132">Property</span></span>     | <span data-ttu-id="039ff-133">Typ</span><span class="sxs-lookup"><span data-stu-id="039ff-133">Type</span></span>   |<span data-ttu-id="039ff-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="039ff-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="039ff-135">name</span><span class="sxs-lookup"><span data-stu-id="039ff-135">name</span></span>|<span data-ttu-id="039ff-136">String</span><span class="sxs-lookup"><span data-stu-id="039ff-136">String</span></span>|<span data-ttu-id="039ff-137">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="039ff-137">Name of the bucket.</span></span>|
|<span data-ttu-id="039ff-138">orderHint</span><span class="sxs-lookup"><span data-stu-id="039ff-138">orderHint</span></span>|<span data-ttu-id="039ff-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="039ff-139">String</span></span>|<span data-ttu-id="039ff-p106">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist unter [Verwenden von Anordnungshinweisen in Planner](../resources/planner-order-hint-format.md) definiert.</span><span class="sxs-lookup"><span data-stu-id="039ff-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="039ff-142">planId</span><span class="sxs-lookup"><span data-stu-id="039ff-142">planId</span></span>|<span data-ttu-id="039ff-143">String</span><span class="sxs-lookup"><span data-stu-id="039ff-143">String</span></span>|<span data-ttu-id="039ff-144">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="039ff-144">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="039ff-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="039ff-145">Response</span></span>

<span data-ttu-id="039ff-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerBucket](../resources/plannerbucket.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="039ff-146">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="039ff-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="039ff-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="039ff-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="039ff-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="039ff-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="039ff-151">Request</span></span>
<span data-ttu-id="039ff-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="039ff-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="039ff-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="039ff-153">Response</span></span>
<span data-ttu-id="039ff-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="039ff-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
