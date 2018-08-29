# <a name="get-plannertaskdetails"></a><span data-ttu-id="c1057-101">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="c1057-101">Get plannerTaskDetails</span></span>

<span data-ttu-id="c1057-102">Dient zum Abrufen der Eigenschaften und Beziehungen des **plannertaskdetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1057-102">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1057-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1057-103">Permissions</span></span>
<span data-ttu-id="c1057-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1057-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1057-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1057-106">Permission type</span></span>      | <span data-ttu-id="c1057-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1057-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1057-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1057-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c1057-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1057-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1057-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1057-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1057-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1057-111">Not supported.</span></span>    |
|<span data-ttu-id="c1057-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1057-112">Application</span></span> | <span data-ttu-id="c1057-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1057-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1057-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1057-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="c1057-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1057-115">Request headers</span></span>
| <span data-ttu-id="c1057-116">Name</span><span class="sxs-lookup"><span data-stu-id="c1057-116">Name</span></span>      |<span data-ttu-id="c1057-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1057-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1057-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c1057-118">Authorization</span></span>  | <span data-ttu-id="c1057-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1057-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1057-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1057-121">Request body</span></span>
<span data-ttu-id="c1057-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1057-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1057-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1057-123">Response</span></span>

<span data-ttu-id="c1057-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [plannerTaskDetails](../resources/plannertaskdetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1057-124">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="c1057-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c1057-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c1057-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1057-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1057-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1057-129">Request</span></span>
<span data-ttu-id="c1057-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1057-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
```
##### <a name="response"></a><span data-ttu-id="c1057-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1057-131">Response</span></span>
<span data-ttu-id="c1057-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1057-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->