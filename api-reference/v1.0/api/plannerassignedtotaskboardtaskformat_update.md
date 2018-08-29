# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="ee0ff-101">plannerAssignedToTaskBoardTaskFormat aktualisieren </span><span class="sxs-lookup"><span data-stu-id="ee0ff-101">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="ee0ff-102">Dient zum Aktualisieren der Eigenschaften eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-102">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee0ff-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ee0ff-103">Permissions</span></span>
<span data-ttu-id="ee0ff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee0ff-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee0ff-106">Permission type</span></span>      | <span data-ttu-id="ee0ff-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee0ff-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee0ff-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee0ff-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ee0ff-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0ff-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee0ff-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee0ff-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee0ff-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee0ff-111">Not supported.</span></span>    |
|<span data-ttu-id="ee0ff-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee0ff-112">Application</span></span> | <span data-ttu-id="ee0ff-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee0ff-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee0ff-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee0ff-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="ee0ff-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee0ff-115">Optional request headers</span></span>
| <span data-ttu-id="ee0ff-116">Name</span><span class="sxs-lookup"><span data-stu-id="ee0ff-116">Name</span></span>       | <span data-ttu-id="ee0ff-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee0ff-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee0ff-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ee0ff-118">Authorization</span></span>  | <span data-ttu-id="ee0ff-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee0ff-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="ee0ff-121">If-Match</span></span>  | <span data-ttu-id="ee0ff-p103">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerAssignedToTaskBoardTaskFormat**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0ff-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee0ff-124">Request body</span></span>
<span data-ttu-id="ee0ff-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee0ff-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee0ff-128">Property</span></span>     | <span data-ttu-id="ee0ff-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ee0ff-129">Type</span></span>   |<span data-ttu-id="ee0ff-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee0ff-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee0ff-131">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="ee0ff-131">orderHintsByAssignee</span></span>|[<span data-ttu-id="ee0ff-132">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="ee0ff-132">plannerOrderHintsByAssignee</span></span>](../resources/plannerOrderHintsByAssignee.md)|<span data-ttu-id="ee0ff-p105">Wörterbuch von Hinweisen, die verwendet werden, um Aufgaben in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen. Der Schlüssel für jeden Eintrag ist einer der Benutzer, denen die Aufgabe zugewiesen ist, und der Wert ist der Anordnungshinweis. Das Format der einzelnen Werte ist wie [hier](../resources/planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="ee0ff-136">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="ee0ff-136">unassignedOrderHint</span></span>|<span data-ttu-id="ee0ff-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee0ff-137">String</span></span>|<span data-ttu-id="ee0ff-p106">Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](../resources/planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ee0ff-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee0ff-140">Response</span></span>

<span data-ttu-id="ee0ff-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-141">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="ee0ff-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p107">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ee0ff-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee0ff-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee0ff-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee0ff-146">Request</span></span>
<span data-ttu-id="ee0ff-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-147">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ee0ff-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee0ff-148">Response</span></span>
<span data-ttu-id="ee0ff-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee0ff-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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