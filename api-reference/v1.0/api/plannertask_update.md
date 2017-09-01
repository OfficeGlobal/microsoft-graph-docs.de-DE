# <a name="update-plannertask"></a><span data-ttu-id="b0fc7-101">plannerTask aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b0fc7-101">Update plannertask</span></span>

<span data-ttu-id="b0fc7-102">Dient zum Aktualisieren der Eigenschaften des **plannertask**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-102">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0fc7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b0fc7-103">Permissions</span></span>
<span data-ttu-id="b0fc7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0fc7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0fc7-106">Permission type</span></span>      | <span data-ttu-id="b0fc7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0fc7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0fc7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0fc7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b0fc7-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0fc7-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0fc7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0fc7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0fc7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0fc7-111">Not supported.</span></span>    |
|<span data-ttu-id="b0fc7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0fc7-112">Application</span></span> | <span data-ttu-id="b0fc7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0fc7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0fc7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0fc7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="b0fc7-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0fc7-115">Optional request headers</span></span>
| <span data-ttu-id="b0fc7-116">Name</span><span class="sxs-lookup"><span data-stu-id="b0fc7-116">Name</span></span>       | <span data-ttu-id="b0fc7-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0fc7-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b0fc7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0fc7-118">Authorization</span></span>  | <span data-ttu-id="b0fc7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0fc7-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="b0fc7-121">If-Match</span></span>  | <span data-ttu-id="b0fc7-p103">Letzter bekannter ETag-Wert für die zu aktualisierende **plannerTask**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0fc7-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0fc7-124">Request body</span></span>
<span data-ttu-id="b0fc7-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b0fc7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0fc7-128">Property</span></span>     | <span data-ttu-id="b0fc7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b0fc7-129">Type</span></span>   |<span data-ttu-id="b0fc7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0fc7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0fc7-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="b0fc7-131">appliedCategories</span></span>|[<span data-ttu-id="b0fc7-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="b0fc7-132">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="b0fc7-p105">Die Kategorien, auf die die Aufgabe angewendet wurde. Mögliche Werte finden Sie unter [angewendete Kategorien](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="b0fc7-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="b0fc7-135">assigneePriority</span></span>|<span data-ttu-id="b0fc7-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0fc7-136">String</span></span>|<span data-ttu-id="b0fc7-p106">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist unter [Verwenden von Anordnungshinweisen in Planner](../resources/planner_order_hint_format.md) definiert.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="b0fc7-139">assignments</span><span class="sxs-lookup"><span data-stu-id="b0fc7-139">assignments</span></span>|[<span data-ttu-id="b0fc7-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="b0fc7-140">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="b0fc7-141">Der Satz von Benutzern, denen die Aufgabe zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-141">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="b0fc7-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="b0fc7-142">bucketId</span></span>|<span data-ttu-id="b0fc7-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0fc7-143">String</span></span>|<span data-ttu-id="b0fc7-p107">Bucket-ID, zu der die Aufgabe gehört. Der Bucket muss in dem Plan enthalten sein, in dem sich die Aufgabe befindet. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](../resources/planner_identifiers_disclaimer.md) durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p107">Bucket id to which the task belongs. The bucket needs to be in the plan that the task is in. It is 28 characters long and case sensitive. [Format validation](../resources/planner_identifiers_disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="b0fc7-148">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="b0fc7-148">conversationThreadId</span></span>|<span data-ttu-id="b0fc7-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0fc7-149">String</span></span>|<span data-ttu-id="b0fc7-p108">Thread-ID der Unterhaltung zur Aufgabe. Dies ist die ID des Unterhaltungsthreadobjekts, das in der Gruppe erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="b0fc7-152">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b0fc7-152">dueDateTime</span></span>|<span data-ttu-id="b0fc7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0fc7-153">DateTimeOffset</span></span>|<span data-ttu-id="b0fc7-p109">Datum und Uhrzeit der Fälligkeit der Aufgabe. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b0fc7-157">orderHint</span><span class="sxs-lookup"><span data-stu-id="b0fc7-157">orderHint</span></span>|<span data-ttu-id="b0fc7-158">String</span><span class="sxs-lookup"><span data-stu-id="b0fc7-158">String</span></span>|<span data-ttu-id="b0fc7-p110">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist unter [Verwenden von Anordnungshinweisen in Planner](../resources/planner_order_hint_format.md) definiert.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p110">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="b0fc7-161">percentComplete</span><span class="sxs-lookup"><span data-stu-id="b0fc7-161">percentComplete</span></span>|<span data-ttu-id="b0fc7-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fc7-162">Int32</span></span>|<span data-ttu-id="b0fc7-p111">Abgeschlossener Prozentsatz der Aufgabe. Bei Festlegung auf `100` wird die Aufgabe als abgeschlossen betrachtet.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="b0fc7-165">planId</span><span class="sxs-lookup"><span data-stu-id="b0fc7-165">planId</span></span>|<span data-ttu-id="b0fc7-166">String</span><span class="sxs-lookup"><span data-stu-id="b0fc7-166">String</span></span>|<span data-ttu-id="b0fc7-167">Plan-ID, zu der die Aufgabe gehört.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-167">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="b0fc7-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0fc7-168">startDateTime</span></span>|<span data-ttu-id="b0fc7-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0fc7-169">DateTimeOffset</span></span>|<span data-ttu-id="b0fc7-p112">Datum und Uhrzeit des Aufgabenbeginns. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b0fc7-173">title</span><span class="sxs-lookup"><span data-stu-id="b0fc7-173">title</span></span>|<span data-ttu-id="b0fc7-174">String</span><span class="sxs-lookup"><span data-stu-id="b0fc7-174">String</span></span>|<span data-ttu-id="b0fc7-175">Titel der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="b0fc7-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0fc7-176">Response</span></span>

<span data-ttu-id="b0fc7-177">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerTask](../resources/plannertask.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-177">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="b0fc7-p113">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p113">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b0fc7-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0fc7-181">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0fc7-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0fc7-182">Request</span></span>
<span data-ttu-id="b0fc7-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-183">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
Content-type: application/json
Content-length: 247
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": "N9917 U2883!"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category4": false
  }
}
```
##### <a name="response"></a><span data-ttu-id="b0fc7-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0fc7-184">Response</span></span>
<span data-ttu-id="b0fc7-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0fc7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1423

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-24T18:36:49.2407981Z",
  "assignments": {
    "6463a5ce-2119-4198-9f2a-628761df4a62": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "N9917"
    },
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2017-04-24T22:40:44.5665917",
      "orderHint": "RWk1"
    },
    "aaa27244-1db4-476a-a5cb-004607466324": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "U2883"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category5": true,
    "category6": true,
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->