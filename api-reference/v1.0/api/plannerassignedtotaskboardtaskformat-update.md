---
title: 'plannerAssignedToTaskBoardTaskFormat aktualisieren '
description: Dient zum Aktualisieren der Eigenschaften eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.
localization_priority: Normal
ms.openlocfilehash: 9efb07bd8bda108497f77d4f982b42eb3c8e53b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855636"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="17763-103">plannerAssignedToTaskBoardTaskFormat aktualisieren </span><span class="sxs-lookup"><span data-stu-id="17763-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="17763-104">Dient zum Aktualisieren der Eigenschaften eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="17763-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="17763-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="17763-105">Permissions</span></span>
<span data-ttu-id="17763-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17763-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17763-108">Permission type</span></span>      | <span data-ttu-id="17763-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17763-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17763-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17763-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17763-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17763-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="17763-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17763-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17763-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17763-113">Not supported.</span></span>    |
|<span data-ttu-id="17763-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17763-114">Application</span></span> | <span data-ttu-id="17763-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17763-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17763-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17763-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="17763-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17763-117">Optional request headers</span></span>
| <span data-ttu-id="17763-118">Name</span><span class="sxs-lookup"><span data-stu-id="17763-118">Name</span></span>       | <span data-ttu-id="17763-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17763-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="17763-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="17763-120">Authorization</span></span>  | <span data-ttu-id="17763-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17763-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17763-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="17763-123">If-Match</span></span>  | <span data-ttu-id="17763-p103">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerAssignedToTaskBoardTaskFormat**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17763-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17763-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17763-126">Request body</span></span>
<span data-ttu-id="17763-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="17763-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17763-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17763-130">Property</span></span>     | <span data-ttu-id="17763-131">Typ</span><span class="sxs-lookup"><span data-stu-id="17763-131">Type</span></span>   |<span data-ttu-id="17763-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17763-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17763-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="17763-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="17763-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="17763-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="17763-p105">Wörterbuch von Hinweisen, die verwendet werden, um Aufgaben in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen. Der Schlüssel für jeden Eintrag ist einer der Benutzer, denen die Aufgabe zugewiesen ist, und der Wert ist der Anordnungshinweis. Das Format der einzelnen Werte ist wie [hier](../resources/planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="17763-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="17763-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="17763-138">unassignedOrderHint</span></span>|<span data-ttu-id="17763-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17763-139">String</span></span>|<span data-ttu-id="17763-p106">Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](../resources/planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="17763-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="17763-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="17763-142">Response</span></span>

<span data-ttu-id="17763-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17763-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="17763-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="17763-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="17763-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17763-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17763-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17763-148">Request</span></span>
<span data-ttu-id="17763-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17763-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="17763-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="17763-150">Response</span></span>
<span data-ttu-id="17763-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17763-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
