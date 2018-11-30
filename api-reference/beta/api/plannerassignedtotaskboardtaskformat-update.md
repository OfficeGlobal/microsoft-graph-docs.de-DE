---
title: 'plannerAssignedToTaskBoardTaskFormat aktualisieren '
description: Dient zum Aktualisieren der Eigenschaften eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.
ms.openlocfilehash: 7bf559b5962c895c1ce7b5d3192ab743bca3acb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060670"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="fa09b-103">plannerAssignedToTaskBoardTaskFormat aktualisieren </span><span class="sxs-lookup"><span data-stu-id="fa09b-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

> <span data-ttu-id="fa09b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa09b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa09b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa09b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa09b-106">Dient zum Aktualisieren der Eigenschaften eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa09b-106">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa09b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fa09b-107">Permissions</span></span>
<span data-ttu-id="fa09b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa09b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa09b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa09b-110">Permission type</span></span>      | <span data-ttu-id="fa09b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa09b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa09b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa09b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa09b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa09b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa09b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa09b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa09b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa09b-115">Not supported.</span></span>    |
|<span data-ttu-id="fa09b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa09b-116">Application</span></span> | <span data-ttu-id="fa09b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa09b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa09b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa09b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="fa09b-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa09b-119">Optional request headers</span></span>
| <span data-ttu-id="fa09b-120">Name</span><span class="sxs-lookup"><span data-stu-id="fa09b-120">Name</span></span>       | <span data-ttu-id="fa09b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa09b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fa09b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa09b-122">Authorization</span></span>  | <span data-ttu-id="fa09b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa09b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa09b-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="fa09b-125">If-Match</span></span>  | <span data-ttu-id="fa09b-p104">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerAssignedToTaskBoardTaskFormat**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa09b-p104">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa09b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa09b-128">Request body</span></span>
<span data-ttu-id="fa09b-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="fa09b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa09b-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa09b-132">Property</span></span>     | <span data-ttu-id="fa09b-133">Typ</span><span class="sxs-lookup"><span data-stu-id="fa09b-133">Type</span></span>   |<span data-ttu-id="fa09b-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa09b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa09b-135">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="fa09b-135">orderHintsByAssignee</span></span>|[<span data-ttu-id="fa09b-136">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="fa09b-136">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="fa09b-137">Wörterbuch verwendet, um die Reihenfolge Aufgaben in der Ansicht AssignedTo, der die Aufgabe Pinnwand hinweisen.</span><span class="sxs-lookup"><span data-stu-id="fa09b-137">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="fa09b-138">Der Schlüssel für jeden Eintrag eines Benutzer an, die, denen die Aufgabe zugewiesen ist, und der Wert ist der Order-Hinweis.</span><span class="sxs-lookup"><span data-stu-id="fa09b-138">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="fa09b-139">Das Format von jeder Wert wird definiert [mit Reihenfolge Hinweise in Planner (... / resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="fa09b-139">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="fa09b-140">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="fa09b-140">unassignedOrderHint</span></span>|<span data-ttu-id="fa09b-141">String</span><span class="sxs-lookup"><span data-stu-id="fa09b-141">String</span></span>|<span data-ttu-id="fa09b-142">Hinweiswert verwendet, um den Vorgang in der Ansicht AssignedTo der Aufgabe-Karte bestellen, wenn die Aufgabe nicht einem Benutzer zugewiesen wird, oder wenn das Wörterbuch OrderHintsByAssignee Order-Hinweis für den Benutzer die Aufgabe nicht bereitstellt zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="fa09b-142">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="fa09b-143">Das Format ist in [Using Reihenfolge Hinweise in Planner](../resources/planner-order-hint-format.md)definiert.</span><span class="sxs-lookup"><span data-stu-id="fa09b-143">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="fa09b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa09b-144">Response</span></span>

<span data-ttu-id="fa09b-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa09b-145">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="fa09b-p108">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fa09b-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fa09b-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa09b-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa09b-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa09b-150">Request</span></span>
<span data-ttu-id="fa09b-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa09b-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="fa09b-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa09b-152">Response</span></span>
<span data-ttu-id="fa09b-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa09b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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