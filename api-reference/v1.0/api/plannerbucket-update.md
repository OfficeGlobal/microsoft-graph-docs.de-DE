---
title: plannerBucket aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannerbucket**-Objekts.
ms.openlocfilehash: 88c4cd83be2c76ab7f7d220d4a35bd5b90f7edb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018409"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="15eb0-103">plannerBucket aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15eb0-103">Update plannerbucket</span></span>

<span data-ttu-id="15eb0-104">Dient zum Aktualisieren der Eigenschaften eines **plannerbucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="15eb0-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="15eb0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15eb0-105">Permissions</span></span>
<span data-ttu-id="15eb0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15eb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15eb0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15eb0-108">Permission type</span></span>      | <span data-ttu-id="15eb0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15eb0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15eb0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15eb0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15eb0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15eb0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="15eb0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15eb0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15eb0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15eb0-113">Not supported.</span></span>    |
|<span data-ttu-id="15eb0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15eb0-114">Application</span></span> | <span data-ttu-id="15eb0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15eb0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15eb0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15eb0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="15eb0-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15eb0-117">Optional request headers</span></span>
| <span data-ttu-id="15eb0-118">Name</span><span class="sxs-lookup"><span data-stu-id="15eb0-118">Name</span></span>       | <span data-ttu-id="15eb0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15eb0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15eb0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="15eb0-120">Authorization</span></span>  | <span data-ttu-id="15eb0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15eb0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15eb0-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="15eb0-123">If-Match</span></span>  | <span data-ttu-id="15eb0-p103">Letzter bekannter ETag-Wert für den zu aktualisierenden **plannerBucket**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15eb0-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15eb0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15eb0-126">Request body</span></span>
<span data-ttu-id="15eb0-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="15eb0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15eb0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15eb0-130">Property</span></span>     | <span data-ttu-id="15eb0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="15eb0-131">Type</span></span>   |<span data-ttu-id="15eb0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15eb0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15eb0-133">name</span><span class="sxs-lookup"><span data-stu-id="15eb0-133">name</span></span>|<span data-ttu-id="15eb0-134">String</span><span class="sxs-lookup"><span data-stu-id="15eb0-134">String</span></span>|<span data-ttu-id="15eb0-135">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="15eb0-135">Name of the bucket.</span></span>|
|<span data-ttu-id="15eb0-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="15eb0-136">orderHint</span></span>|<span data-ttu-id="15eb0-137">String</span><span class="sxs-lookup"><span data-stu-id="15eb0-137">String</span></span>|<span data-ttu-id="15eb0-p105">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](../resources/planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="15eb0-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="15eb0-140">planId</span><span class="sxs-lookup"><span data-stu-id="15eb0-140">planId</span></span>|<span data-ttu-id="15eb0-141">String</span><span class="sxs-lookup"><span data-stu-id="15eb0-141">String</span></span>|<span data-ttu-id="15eb0-142">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="15eb0-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="15eb0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="15eb0-143">Response</span></span>

<span data-ttu-id="15eb0-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerBucket](../resources/plannerbucket.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15eb0-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="15eb0-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="15eb0-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="15eb0-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15eb0-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15eb0-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15eb0-149">Request</span></span>
<span data-ttu-id="15eb0-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15eb0-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="15eb0-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="15eb0-151">Response</span></span>
<span data-ttu-id="15eb0-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15eb0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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