# <a name="list-buckets"></a><span data-ttu-id="b76b6-101">Buckets auflisten</span><span class="sxs-lookup"><span data-stu-id="b76b6-101">List buckets</span></span>

<span data-ttu-id="b76b6-102">Dient zum Abrufen einer Liste von **plannerbucket**-Objekten, die in einem [plannerPlan](../resources/plannerplan.md)-Objekt enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="b76b6-102">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b76b6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b76b6-103">Permissions</span></span>
<span data-ttu-id="b76b6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b76b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b76b6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b76b6-106">Permission type</span></span>      | <span data-ttu-id="b76b6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b76b6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b76b6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b76b6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b76b6-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b76b6-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b76b6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b76b6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b76b6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b76b6-111">Not supported.</span></span>    |
|<span data-ttu-id="b76b6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b76b6-112">Application</span></span> | <span data-ttu-id="b76b6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b76b6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b76b6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b76b6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="b76b6-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b76b6-115">Request headers</span></span>
| <span data-ttu-id="b76b6-116">Name</span><span class="sxs-lookup"><span data-stu-id="b76b6-116">Name</span></span>      |<span data-ttu-id="b76b6-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b76b6-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b76b6-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b76b6-118">Authorization</span></span>  | <span data-ttu-id="b76b6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b76b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b76b6-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b76b6-121">Request body</span></span>
<span data-ttu-id="b76b6-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b76b6-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b76b6-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="b76b6-123">Response</span></span>

<span data-ttu-id="b76b6-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerBucket](../resources/plannerbucket.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b76b6-124">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="b76b6-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b76b6-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="b76b6-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b76b6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b76b6-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b76b6-129">Request</span></span>
<span data-ttu-id="b76b6-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b76b6-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
##### <a name="response"></a><span data-ttu-id="b76b6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b76b6-131">Response</span></span>
<span data-ttu-id="b76b6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b76b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->