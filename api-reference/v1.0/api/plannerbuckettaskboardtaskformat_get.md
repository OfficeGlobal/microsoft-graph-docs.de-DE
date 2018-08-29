# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="5dd54-101">plannerBucketTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="5dd54-101">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="5dd54-102">Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5dd54-102">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5dd54-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5dd54-103">Permissions</span></span>
<span data-ttu-id="5dd54-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5dd54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5dd54-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5dd54-106">Permission type</span></span>      | <span data-ttu-id="5dd54-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5dd54-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dd54-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5dd54-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5dd54-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dd54-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5dd54-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5dd54-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dd54-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5dd54-111">Not supported.</span></span>    |
|<span data-ttu-id="5dd54-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5dd54-112">Application</span></span> | <span data-ttu-id="5dd54-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5dd54-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dd54-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5dd54-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="5dd54-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5dd54-115">Request headers</span></span>
| <span data-ttu-id="5dd54-116">Name</span><span class="sxs-lookup"><span data-stu-id="5dd54-116">Name</span></span>      |<span data-ttu-id="5dd54-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5dd54-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5dd54-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5dd54-118">Authorization</span></span>  | <span data-ttu-id="5dd54-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5dd54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dd54-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5dd54-121">Request body</span></span>
<span data-ttu-id="5dd54-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5dd54-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dd54-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="5dd54-123">Response</span></span>

<span data-ttu-id="5dd54-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5dd54-124">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="5dd54-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="5dd54-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5dd54-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5dd54-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dd54-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5dd54-129">Request</span></span>
<span data-ttu-id="5dd54-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5dd54-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="5dd54-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5dd54-131">Response</span></span>
<span data-ttu-id="5dd54-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5dd54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->