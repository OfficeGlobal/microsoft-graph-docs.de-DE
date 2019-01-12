---
title: plannerBucketTaskBoardTaskFormat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannerBucketTaskBoardTaskFormat**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 7dad7a639ce8243fe6138d813a1de0bde2da11e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936039"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="6ec97-103">plannerBucketTaskBoardTaskFormat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6ec97-103">Update plannerBucketTaskBoardTaskFormat</span></span>

> <span data-ttu-id="6ec97-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ec97-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ec97-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ec97-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ec97-106">Dient zum Aktualisieren der Eigenschaften eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ec97-106">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ec97-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6ec97-107">Permissions</span></span>
<span data-ttu-id="6ec97-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ec97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ec97-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ec97-110">Permission type</span></span>      | <span data-ttu-id="6ec97-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ec97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ec97-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ec97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ec97-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ec97-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ec97-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ec97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ec97-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ec97-115">Not supported.</span></span>    |
|<span data-ttu-id="6ec97-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ec97-116">Application</span></span> | <span data-ttu-id="6ec97-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ec97-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ec97-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ec97-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="6ec97-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ec97-119">Optional request headers</span></span>
| <span data-ttu-id="6ec97-120">Name</span><span class="sxs-lookup"><span data-stu-id="6ec97-120">Name</span></span>       | <span data-ttu-id="6ec97-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ec97-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6ec97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ec97-122">Authorization</span></span>  | <span data-ttu-id="6ec97-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ec97-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ec97-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="6ec97-125">If-Match</span></span>  | <span data-ttu-id="6ec97-p104">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerBucketTaskBoardTaskFormat**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ec97-p104">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ec97-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ec97-128">Request body</span></span>
<span data-ttu-id="6ec97-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="6ec97-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6ec97-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ec97-132">Property</span></span>     | <span data-ttu-id="6ec97-133">Typ</span><span class="sxs-lookup"><span data-stu-id="6ec97-133">Type</span></span>   |<span data-ttu-id="6ec97-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ec97-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ec97-135">orderHint</span><span class="sxs-lookup"><span data-stu-id="6ec97-135">orderHint</span></span>|<span data-ttu-id="6ec97-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ec97-136">String</span></span>|<span data-ttu-id="6ec97-p106">Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](../resources/planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="6ec97-p106">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="6ec97-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ec97-139">Response</span></span>

<span data-ttu-id="6ec97-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ec97-140">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="6ec97-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6ec97-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6ec97-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ec97-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ec97-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ec97-145">Request</span></span>
<span data-ttu-id="6ec97-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ec97-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="6ec97-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ec97-147">Response</span></span>
<span data-ttu-id="6ec97-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ec97-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
