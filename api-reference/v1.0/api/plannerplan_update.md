# <a name="update-plannerplan"></a><span data-ttu-id="97f76-101">Aktualisierung des plannerPlan</span><span class="sxs-lookup"><span data-stu-id="97f76-101">Update plannerplan</span></span>

<span data-ttu-id="97f76-102">Dient zum Aktualisieren der Eigenschaften eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="97f76-102">Update the properties of **plannerplan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97f76-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97f76-103">Permissions</span></span>
<span data-ttu-id="97f76-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97f76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97f76-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97f76-106">Permission type</span></span>      | <span data-ttu-id="97f76-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97f76-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97f76-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97f76-108">Delegated (work or school account)</span></span> | <span data-ttu-id="97f76-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f76-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97f76-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97f76-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f76-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97f76-111">Not supported.</span></span>    |
|<span data-ttu-id="97f76-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97f76-112">Application</span></span> | <span data-ttu-id="97f76-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97f76-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97f76-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97f76-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97f76-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97f76-115">Request headers</span></span>

| <span data-ttu-id="97f76-116">Name</span><span class="sxs-lookup"><span data-stu-id="97f76-116">Name</span></span>       | <span data-ttu-id="97f76-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f76-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97f76-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="97f76-118">Authorization</span></span>  | <span data-ttu-id="97f76-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97f76-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97f76-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="97f76-121">If-Match</span></span>  | <span data-ttu-id="97f76-p103">Letzter bekannter ETag-Wert für den zu aktualisierenden plannerPlan. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97f76-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97f76-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97f76-124">Request body</span></span>
<span data-ttu-id="97f76-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="97f76-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97f76-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97f76-128">Property</span></span>     | <span data-ttu-id="97f76-129">Typ</span><span class="sxs-lookup"><span data-stu-id="97f76-129">Type</span></span>   |<span data-ttu-id="97f76-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f76-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97f76-131">owner</span><span class="sxs-lookup"><span data-stu-id="97f76-131">owner</span></span>|<span data-ttu-id="97f76-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97f76-132">String</span></span>|<span data-ttu-id="97f76-p105">[Gruppe](../resources/group.md) `id`, in deren Besitz der Plan ist. Dieses Feld kann erst festgelegt werden, wenn eine gültige Gruppe vorhanden ist. Nachdem dieses festgelegt wurde, kann es nur noch vom Besitzer aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="97f76-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="97f76-136">title</span><span class="sxs-lookup"><span data-stu-id="97f76-136">title</span></span>|<span data-ttu-id="97f76-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97f76-137">String</span></span>|<span data-ttu-id="97f76-138">Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="97f76-138">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="97f76-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="97f76-139">Response</span></span>

<span data-ttu-id="97f76-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97f76-140">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="97f76-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="97f76-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="97f76-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97f76-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97f76-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97f76-145">Request</span></span>
<span data-ttu-id="97f76-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97f76-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="97f76-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="97f76-147">Response</span></span>
<span data-ttu-id="97f76-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97f76-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->