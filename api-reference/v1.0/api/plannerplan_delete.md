# <a name="delete-plannerplan"></a><span data-ttu-id="ff01e-101">plannerPlan löschen</span><span class="sxs-lookup"><span data-stu-id="ff01e-101">Delete plannerPlan</span></span>

<span data-ttu-id="ff01e-102">Dient zum Löschen eines **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff01e-102">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff01e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ff01e-103">Permissions</span></span>
<span data-ttu-id="ff01e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff01e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff01e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff01e-106">Permission type</span></span>      | <span data-ttu-id="ff01e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff01e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff01e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff01e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ff01e-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff01e-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff01e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff01e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff01e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff01e-111">Not supported.</span></span>    |
|<span data-ttu-id="ff01e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff01e-112">Application</span></span> | <span data-ttu-id="ff01e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff01e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff01e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff01e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ff01e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff01e-115">Request headers</span></span>
| <span data-ttu-id="ff01e-116">Name</span><span class="sxs-lookup"><span data-stu-id="ff01e-116">Name</span></span>       | <span data-ttu-id="ff01e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff01e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff01e-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ff01e-118">Authorization</span></span>  | <span data-ttu-id="ff01e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff01e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff01e-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="ff01e-121">If-Match</span></span>  | <span data-ttu-id="ff01e-p103">Letzter bekannter ETag-Wert für den zu löschenden **plannerPlan**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff01e-p103">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff01e-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff01e-124">Request body</span></span>
<span data-ttu-id="ff01e-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff01e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff01e-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff01e-126">Response</span></span>

<span data-ttu-id="ff01e-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff01e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ff01e-p105">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ff01e-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ff01e-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff01e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff01e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff01e-133">Request</span></span>
<span data-ttu-id="ff01e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff01e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/plans/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="ff01e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff01e-135">Response</span></span>
<span data-ttu-id="ff01e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff01e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->