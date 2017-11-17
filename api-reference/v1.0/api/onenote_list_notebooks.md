# <a name="list-notebooks"></a><span data-ttu-id="04dca-101">Notizbücher auflisten</span><span class="sxs-lookup"><span data-stu-id="04dca-101">List notebooks</span></span>

<span data-ttu-id="04dca-102">Mit dieser API können Sie eine Liste von Objekten des Typs [notebook](../resources/notebook.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="04dca-102">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="04dca-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04dca-103">Permissions</span></span>
<span data-ttu-id="04dca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04dca-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04dca-106">Permission type</span></span>      | <span data-ttu-id="04dca-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04dca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04dca-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04dca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="04dca-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04dca-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="04dca-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04dca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04dca-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04dca-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="04dca-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04dca-112">Application</span></span> | <span data-ttu-id="04dca-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04dca-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04dca-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04dca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04dca-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04dca-115">Optional query parameters</span></span>
<span data-ttu-id="04dca-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04dca-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="04dca-117">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="04dca-117">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="04dca-118">Gültige `expand`-Werte für Notizbücher sind `sections` und `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="04dca-118">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04dca-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04dca-119">Request headers</span></span>
| <span data-ttu-id="04dca-120">Name</span><span class="sxs-lookup"><span data-stu-id="04dca-120">Name</span></span>       | <span data-ttu-id="04dca-121">Typ</span><span class="sxs-lookup"><span data-stu-id="04dca-121">Type</span></span> | <span data-ttu-id="04dca-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04dca-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04dca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04dca-123">Authorization</span></span>  | <span data-ttu-id="04dca-124">string</span><span class="sxs-lookup"><span data-stu-id="04dca-124">string</span></span>  | <span data-ttu-id="04dca-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04dca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04dca-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="04dca-127">Accept</span></span> | <span data-ttu-id="04dca-128">string</span><span class="sxs-lookup"><span data-stu-id="04dca-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="04dca-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04dca-129">Request body</span></span>
<span data-ttu-id="04dca-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04dca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04dca-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="04dca-131">Response</span></span>

<span data-ttu-id="04dca-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [notebook](../resources/notebook.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04dca-132">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04dca-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04dca-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04dca-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04dca-134">Request</span></span>
<span data-ttu-id="04dca-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04dca-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="04dca-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="04dca-136">Response</span></span>
<span data-ttu-id="04dca-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04dca-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->