# <a name="list-tasks"></a><span data-ttu-id="f32b1-101">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="f32b1-101">List tasks</span></span>

<span data-ttu-id="f32b1-102">Dient zum Abrufen einer Liste von **plannertask**-Objekten.</span><span class="sxs-lookup"><span data-stu-id="f32b1-102">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f32b1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f32b1-103">Permissions</span></span>
<span data-ttu-id="f32b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f32b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f32b1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f32b1-106">Permission type</span></span>      | <span data-ttu-id="f32b1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f32b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f32b1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f32b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f32b1-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32b1-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f32b1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f32b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f32b1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f32b1-111">Not supported.</span></span>    |
|<span data-ttu-id="f32b1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f32b1-112">Application</span></span> | <span data-ttu-id="f32b1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f32b1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f32b1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f32b1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f32b1-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f32b1-115">Optional query parameters</span></span>
<span data-ttu-id="f32b1-116">Für diese Methode müssen [Filter](http://graph.microsoft.io/docs/overview/query_parameters) für planID angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="f32b1-116">This method requires planId [filter](http://graph.microsoft.io/docs/overview/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f32b1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f32b1-117">Request headers</span></span>
| <span data-ttu-id="f32b1-118">Name</span><span class="sxs-lookup"><span data-stu-id="f32b1-118">Name</span></span>      |<span data-ttu-id="f32b1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f32b1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f32b1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f32b1-120">Authorization</span></span>  | <span data-ttu-id="f32b1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f32b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f32b1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f32b1-123">Request body</span></span>
<span data-ttu-id="f32b1-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f32b1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f32b1-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="f32b1-125">Response</span></span>

<span data-ttu-id="f32b1-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerTask](../resources/plannertask.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f32b1-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="f32b1-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f32b1-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="f32b1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f32b1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f32b1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f32b1-131">Request</span></span>
<span data-ttu-id="f32b1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f32b1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks
```
##### <a name="response"></a><span data-ttu-id="f32b1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f32b1-133">Response</span></span>
<span data-ttu-id="f32b1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f32b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
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
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerAssignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->