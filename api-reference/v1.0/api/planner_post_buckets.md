# <a name="create-plannerbucket"></a><span data-ttu-id="435ee-101">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="435ee-101">Create plannerBucket</span></span>

<span data-ttu-id="435ee-102">Verwenden Sie diese API zum Erstellen eines neuen **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="435ee-102">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="435ee-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="435ee-103">Permissions</span></span>
<span data-ttu-id="435ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="435ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="435ee-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="435ee-106">Permission type</span></span>      | <span data-ttu-id="435ee-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="435ee-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="435ee-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="435ee-108">Delegated (work or school account)</span></span> | <span data-ttu-id="435ee-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="435ee-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="435ee-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="435ee-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="435ee-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="435ee-111">Not supported.</span></span>    |
|<span data-ttu-id="435ee-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="435ee-112">Application</span></span> | <span data-ttu-id="435ee-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="435ee-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="435ee-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="435ee-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="435ee-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="435ee-115">Request headers</span></span>
| <span data-ttu-id="435ee-116">Name</span><span class="sxs-lookup"><span data-stu-id="435ee-116">Name</span></span>       | <span data-ttu-id="435ee-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="435ee-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="435ee-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="435ee-118">Authorization</span></span>  | <span data-ttu-id="435ee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="435ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="435ee-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="435ee-121">Request body</span></span>
<span data-ttu-id="435ee-122">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerBucket](../resources/plannerbucket.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="435ee-122">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="435ee-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="435ee-123">Response</span></span>

<span data-ttu-id="435ee-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [plannerBucket](../resources/plannerbucket.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="435ee-124">If successful, this method returns `201, Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="435ee-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="435ee-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="435ee-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="435ee-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="435ee-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="435ee-129">Request</span></span>
<span data-ttu-id="435ee-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="435ee-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="435ee-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerBucket](../resources/plannerbucket.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="435ee-131">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="435ee-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="435ee-132">Response</span></span>
<span data-ttu-id="435ee-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="435ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->