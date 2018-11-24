# <a name="get-page"></a><span data-ttu-id="5648d-101">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="5648d-101">Get page</span></span>

<span data-ttu-id="5648d-102">Dient zum Abrufen der Eigenschaften und Beziehungen eines [page](../resources/page.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5648d-102">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="5648d-103">**Seiteninformationen abrufen**</span><span class="sxs-lookup"><span data-stu-id="5648d-103">**Getting page information**</span></span>

<span data-ttu-id="5648d-104">Greifen Sie über den Seitenbezeichner auf die Metadaten einer Seite zu:</span><span class="sxs-lookup"><span data-stu-id="5648d-104">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="5648d-105">**Seiteninhalt abrufen**</span><span class="sxs-lookup"><span data-stu-id="5648d-105">**Getting page content**</span></span>

<span data-ttu-id="5648d-106">Sie können den `content`-Endpunkt der Seite verwenden, um den HTML-Inhalt einer Seite abzurufen:</span><span class="sxs-lookup"><span data-stu-id="5648d-106">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="5648d-107">Die Abfrageoption `includeIDs=true` wird verwendet, um [Seiten zu aktualisieren](../api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="5648d-107">The `includeIDs=true` query option is used to [update pages](../api/page_update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5648d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5648d-108">Permissions</span></span>
<span data-ttu-id="5648d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5648d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5648d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5648d-111">Permission type</span></span>      | <span data-ttu-id="5648d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5648d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5648d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5648d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5648d-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5648d-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5648d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5648d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5648d-116">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5648d-116">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5648d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5648d-117">Application</span></span> | <span data-ttu-id="5648d-118">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5648d-118">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5648d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5648d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5648d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5648d-120">Optional query parameters</span></span>
<span data-ttu-id="5648d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5648d-121">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5648d-p102">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="5648d-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5648d-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5648d-124">Request headers</span></span>
| <span data-ttu-id="5648d-125">Name</span><span class="sxs-lookup"><span data-stu-id="5648d-125">Name</span></span>       | <span data-ttu-id="5648d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="5648d-126">Type</span></span> | <span data-ttu-id="5648d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5648d-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5648d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5648d-128">Authorization</span></span>  | <span data-ttu-id="5648d-129">string</span><span class="sxs-lookup"><span data-stu-id="5648d-129">string</span></span>  | <span data-ttu-id="5648d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5648d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5648d-132">Accept</span><span class="sxs-lookup"><span data-stu-id="5648d-132">Accept</span></span> | <span data-ttu-id="5648d-133">string</span><span class="sxs-lookup"><span data-stu-id="5648d-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5648d-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5648d-134">Request body</span></span>
<span data-ttu-id="5648d-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5648d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5648d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5648d-136">Response</span></span>

<span data-ttu-id="5648d-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5648d-137">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5648d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5648d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5648d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5648d-139">Request</span></span>
<span data-ttu-id="5648d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5648d-140">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="5648d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5648d-141">Response</span></span>
<span data-ttu-id="5648d-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5648d-142">Here is an example of the response.</span></span> <span data-ttu-id="5648d-143">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="5648d-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="5648d-144">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5648d-144">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
