# <a name="list-pages"></a><span data-ttu-id="159fb-101">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="159fb-101">List pages</span></span>

<span data-ttu-id="159fb-102">Mit dieser API können Sie eine Liste von Objekten des Typs [page](../resources/page.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="159fb-102">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="159fb-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="159fb-103">Permissions</span></span>
<span data-ttu-id="159fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="159fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="159fb-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="159fb-106">Permission type</span></span>      | <span data-ttu-id="159fb-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="159fb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="159fb-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="159fb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="159fb-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="159fb-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="159fb-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="159fb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="159fb-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="159fb-111">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="159fb-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="159fb-112">Application</span></span> | <span data-ttu-id="159fb-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="159fb-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="159fb-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="159fb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="159fb-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="159fb-115">Optional query parameters</span></span>
<span data-ttu-id="159fb-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="159fb-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="159fb-p102">Die Standardabfrage für Seiten gibt die ersten 20 Seiten sortiert nach `lastModifiedTime desc` zurück. Wenn die Standardabfrage mehr als 20 Seiten zurückgibt, enthält die Antwort ein `@odata.nextLink`-Objekt, mit dem Sie seitenweise durch das Resultset blättern können. Die maximale Anzahl von Seiten, die für eine `top`-Anforderung zurückgegeben werden, beträgt 100.</span><span class="sxs-lookup"><span data-stu-id="159fb-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="159fb-p103">Die Standardantwort erweitert `parentSection` und wählt die Eigenschaften `id`, `displayName` und `self` des Abschnitts aus. Gültige `expand`-Werte für Seiten sind `parentNotebook` und `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="159fb-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="159fb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="159fb-122">Request headers</span></span>
| <span data-ttu-id="159fb-123">Name</span><span class="sxs-lookup"><span data-stu-id="159fb-123">Name</span></span>       | <span data-ttu-id="159fb-124">Typ</span><span class="sxs-lookup"><span data-stu-id="159fb-124">Type</span></span> | <span data-ttu-id="159fb-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="159fb-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="159fb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="159fb-126">Authorization</span></span>  | <span data-ttu-id="159fb-127">string</span><span class="sxs-lookup"><span data-stu-id="159fb-127">string</span></span>  | <span data-ttu-id="159fb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="159fb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="159fb-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="159fb-130">Accept</span></span> | <span data-ttu-id="159fb-131">string</span><span class="sxs-lookup"><span data-stu-id="159fb-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="159fb-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="159fb-132">Request body</span></span>
<span data-ttu-id="159fb-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="159fb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="159fb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="159fb-134">Response</span></span>

<span data-ttu-id="159fb-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [page](../resources/page.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="159fb-135">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="159fb-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="159fb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="159fb-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="159fb-137">Request</span></span>
<span data-ttu-id="159fb-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="159fb-138">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="159fb-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="159fb-139">Response</span></span>
<span data-ttu-id="159fb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="159fb-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->