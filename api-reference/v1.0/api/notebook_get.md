# <a name="get-notebook"></a><span data-ttu-id="c5a71-101">Notizbuch abrufen</span><span class="sxs-lookup"><span data-stu-id="c5a71-101">Get notebook</span></span>

<span data-ttu-id="c5a71-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="c5a71-102">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5a71-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c5a71-103">Permissions</span></span>
<span data-ttu-id="c5a71-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5a71-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5a71-106">Permission type</span></span>      | <span data-ttu-id="c5a71-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5a71-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5a71-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5a71-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c5a71-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a71-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5a71-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5a71-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5a71-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5a71-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c5a71-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5a71-112">Application</span></span> | <span data-ttu-id="c5a71-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a71-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5a71-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a71-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5a71-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c5a71-115">Optional query parameters</span></span>
<span data-ttu-id="c5a71-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5a71-116">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c5a71-117">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="c5a71-117">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5a71-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5a71-118">Request headers</span></span>
| <span data-ttu-id="c5a71-119">Name</span><span class="sxs-lookup"><span data-stu-id="c5a71-119">Name</span></span>       | <span data-ttu-id="c5a71-120">Typ</span><span class="sxs-lookup"><span data-stu-id="c5a71-120">Type</span></span> | <span data-ttu-id="c5a71-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5a71-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5a71-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a71-122">Authorization</span></span>  | <span data-ttu-id="c5a71-123">string</span><span class="sxs-lookup"><span data-stu-id="c5a71-123">string</span></span>  | <span data-ttu-id="c5a71-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5a71-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5a71-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5a71-126">Accept</span></span> | <span data-ttu-id="c5a71-127">string</span><span class="sxs-lookup"><span data-stu-id="c5a71-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c5a71-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5a71-128">Request body</span></span>
<span data-ttu-id="c5a71-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c5a71-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5a71-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a71-130">Response</span></span>

<span data-ttu-id="c5a71-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5a71-131">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5a71-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5a71-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5a71-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a71-133">Request</span></span>
<span data-ttu-id="c5a71-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5a71-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="c5a71-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a71-135">Response</span></span>
<span data-ttu-id="c5a71-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5a71-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
