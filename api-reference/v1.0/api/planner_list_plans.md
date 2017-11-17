# <a name="list-plans"></a><span data-ttu-id="85fca-101">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="85fca-101">List plans</span></span>

<span data-ttu-id="85fca-102">Dient zum Abrufen einer Liste von **plannerplan**-Objekten.</span><span class="sxs-lookup"><span data-stu-id="85fca-102">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="85fca-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="85fca-103">Permissions</span></span>
<span data-ttu-id="85fca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="85fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="85fca-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85fca-106">Permission type</span></span>      | <span data-ttu-id="85fca-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85fca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85fca-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85fca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="85fca-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85fca-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="85fca-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85fca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85fca-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85fca-111">Not supported.</span></span>    |
|<span data-ttu-id="85fca-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85fca-112">Application</span></span> | <span data-ttu-id="85fca-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85fca-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85fca-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85fca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85fca-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="85fca-115">Optional query parameters</span></span>
<span data-ttu-id="85fca-116">Für diese Methode müssen [Filter](http://graph.microsoft.io/docs/overview/query_parameters) für „owner“ angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="85fca-116">This method requires owner [filter](http://graph.microsoft.io/docs/overview/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85fca-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85fca-117">Request headers</span></span>
| <span data-ttu-id="85fca-118">Name</span><span class="sxs-lookup"><span data-stu-id="85fca-118">Name</span></span>      |<span data-ttu-id="85fca-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85fca-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85fca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="85fca-120">Authorization</span></span>  | <span data-ttu-id="85fca-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85fca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85fca-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85fca-123">Request body</span></span>
<span data-ttu-id="85fca-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85fca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85fca-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="85fca-125">Response</span></span>

<span data-ttu-id="85fca-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerPlan](../resources/plannerplan.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85fca-126">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="85fca-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="85fca-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="85fca-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85fca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85fca-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85fca-131">Request</span></span>
<span data-ttu-id="85fca-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85fca-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans
```
##### <a name="response"></a><span data-ttu-id="85fca-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="85fca-133">Response</span></span>
<span data-ttu-id="85fca-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85fca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->