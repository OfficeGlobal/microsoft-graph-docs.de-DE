# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="799b1-101">plannerProgressTaskBoardTaskFormat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="799b1-101">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="799b1-102">Dient zum Aktualisieren der Eigenschaften eines **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="799b1-102">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="799b1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="799b1-103">Permissions</span></span>
<span data-ttu-id="799b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="799b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="799b1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="799b1-106">Permission type</span></span>      | <span data-ttu-id="799b1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="799b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="799b1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="799b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="799b1-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="799b1-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="799b1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="799b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="799b1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="799b1-111">Not supported.</span></span>    |
|<span data-ttu-id="799b1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="799b1-112">Application</span></span> | <span data-ttu-id="799b1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="799b1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="799b1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="799b1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="799b1-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="799b1-115">Optional request headers</span></span>
| <span data-ttu-id="799b1-116">Name</span><span class="sxs-lookup"><span data-stu-id="799b1-116">Name</span></span>       | <span data-ttu-id="799b1-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="799b1-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="799b1-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="799b1-118">Authorization</span></span>  | <span data-ttu-id="799b1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="799b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="799b1-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="799b1-121">If-Match</span></span>  | <span data-ttu-id="799b1-p103">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerProgressTaskBoardTaskFormat**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="799b1-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="799b1-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="799b1-124">Request body</span></span>
<span data-ttu-id="799b1-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="799b1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="799b1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="799b1-128">Property</span></span>     | <span data-ttu-id="799b1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="799b1-129">Type</span></span>   |<span data-ttu-id="799b1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="799b1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="799b1-131">orderHint</span><span class="sxs-lookup"><span data-stu-id="799b1-131">orderHint</span></span>|<span data-ttu-id="799b1-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="799b1-132">String</span></span>|<span data-ttu-id="799b1-p105">Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](../resources/planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="799b1-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="799b1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="799b1-135">Response</span></span>

<span data-ttu-id="799b1-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="799b1-136">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="799b1-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="799b1-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="799b1-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="799b1-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="799b1-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="799b1-141">Request</span></span>
<span data-ttu-id="799b1-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="799b1-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="799b1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="799b1-143">Response</span></span>
<span data-ttu-id="799b1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="799b1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->