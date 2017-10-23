# <a name="create-plannerplan"></a><span data-ttu-id="e1481-101">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="e1481-101">Create plannerPlan</span></span>

<span data-ttu-id="e1481-102">Verwenden Sie diese API zum Erstellen eines neuen **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1481-102">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1481-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e1481-103">Permissions</span></span>
<span data-ttu-id="e1481-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1481-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1481-106">Permission type</span></span>      | <span data-ttu-id="e1481-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1481-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1481-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1481-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e1481-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1481-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1481-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1481-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1481-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1481-111">Not supported.</span></span>    |
|<span data-ttu-id="e1481-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1481-112">Application</span></span> | <span data-ttu-id="e1481-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1481-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1481-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1481-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/plans

```
## <a name="request-headers"></a><span data-ttu-id="e1481-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1481-115">Request headers</span></span>
| <span data-ttu-id="e1481-116">Name</span><span class="sxs-lookup"><span data-stu-id="e1481-116">Name</span></span>       | <span data-ttu-id="e1481-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1481-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1481-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1481-118">Authorization</span></span>  | <span data-ttu-id="e1481-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1481-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1481-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1481-121">Request body</span></span>
<span data-ttu-id="e1481-p103">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerPlan](../resources/plannerplan.md)-Objekts an. Die Eigenschaft „owner“ des **plannerPlan**-Objekts muss auf die ID eines [group](../resources/group.md)-Objekts festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="e1481-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1481-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1481-124">Response</span></span>

<span data-ttu-id="e1481-125">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1481-125">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="e1481-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e1481-p104">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e1481-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1481-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1481-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1481-130">Request</span></span>
<span data-ttu-id="e1481-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1481-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
<span data-ttu-id="e1481-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerPlan](../resources/plannerplan.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e1481-132">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1481-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1481-133">Response</span></span>
<span data-ttu-id="e1481-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1481-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->