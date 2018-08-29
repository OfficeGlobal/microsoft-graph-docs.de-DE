# <a name="update-plannerbucket"></a><span data-ttu-id="854ab-101">plannerBucket aktualisieren</span><span class="sxs-lookup"><span data-stu-id="854ab-101">Update plannerbucket</span></span>

<span data-ttu-id="854ab-102">Dient zum Aktualisieren der Eigenschaften eines **plannerbucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="854ab-102">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="854ab-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="854ab-103">Permissions</span></span>
<span data-ttu-id="854ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="854ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="854ab-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="854ab-106">Permission type</span></span>      | <span data-ttu-id="854ab-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="854ab-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="854ab-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="854ab-108">Delegated (work or school account)</span></span> | <span data-ttu-id="854ab-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="854ab-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="854ab-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="854ab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="854ab-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="854ab-111">Not supported.</span></span>    |
|<span data-ttu-id="854ab-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="854ab-112">Application</span></span> | <span data-ttu-id="854ab-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="854ab-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="854ab-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="854ab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="854ab-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="854ab-115">Optional request headers</span></span>
| <span data-ttu-id="854ab-116">Name</span><span class="sxs-lookup"><span data-stu-id="854ab-116">Name</span></span>       | <span data-ttu-id="854ab-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="854ab-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="854ab-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="854ab-118">Authorization</span></span>  | <span data-ttu-id="854ab-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="854ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="854ab-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="854ab-121">If-Match</span></span>  | <span data-ttu-id="854ab-p103">Letzter bekannter ETag-Wert für den zu aktualisierenden **plannerBucket**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="854ab-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="854ab-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="854ab-124">Request body</span></span>
<span data-ttu-id="854ab-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="854ab-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="854ab-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="854ab-128">Property</span></span>     | <span data-ttu-id="854ab-129">Typ</span><span class="sxs-lookup"><span data-stu-id="854ab-129">Type</span></span>   |<span data-ttu-id="854ab-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="854ab-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="854ab-131">name</span><span class="sxs-lookup"><span data-stu-id="854ab-131">name</span></span>|<span data-ttu-id="854ab-132">String</span><span class="sxs-lookup"><span data-stu-id="854ab-132">String</span></span>|<span data-ttu-id="854ab-133">Name des Buckets.</span><span class="sxs-lookup"><span data-stu-id="854ab-133">Name of the bucket.</span></span>|
|<span data-ttu-id="854ab-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="854ab-134">orderHint</span></span>|<span data-ttu-id="854ab-135">String</span><span class="sxs-lookup"><span data-stu-id="854ab-135">String</span></span>|<span data-ttu-id="854ab-p105">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](../resources/planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="854ab-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="854ab-138">planId</span><span class="sxs-lookup"><span data-stu-id="854ab-138">planId</span></span>|<span data-ttu-id="854ab-139">String</span><span class="sxs-lookup"><span data-stu-id="854ab-139">String</span></span>|<span data-ttu-id="854ab-140">Plan-ID, zu der der Bucket gehört.</span><span class="sxs-lookup"><span data-stu-id="854ab-140">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="854ab-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="854ab-141">Response</span></span>

<span data-ttu-id="854ab-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerBucket](../resources/plannerbucket.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="854ab-142">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="854ab-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="854ab-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="854ab-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="854ab-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="854ab-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="854ab-147">Request</span></span>
<span data-ttu-id="854ab-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="854ab-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="854ab-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="854ab-149">Response</span></span>
<span data-ttu-id="854ab-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="854ab-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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