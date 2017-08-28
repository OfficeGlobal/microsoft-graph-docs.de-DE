# <a name="get-section"></a><span data-ttu-id="0be80-101">Abschnitt abrufen</span><span class="sxs-lookup"><span data-stu-id="0be80-101">Get section</span></span>

<span data-ttu-id="0be80-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [section](../resources/section.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="0be80-102">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0be80-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0be80-103">Permissions</span></span>
<span data-ttu-id="0be80-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0be80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0be80-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0be80-106">Permission type</span></span>      | <span data-ttu-id="0be80-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0be80-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0be80-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0be80-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0be80-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be80-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0be80-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0be80-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0be80-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0be80-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0be80-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0be80-112">Application</span></span> | <span data-ttu-id="0be80-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be80-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0be80-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be80-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0be80-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0be80-115">Optional query parameters</span></span>
<span data-ttu-id="0be80-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) `select` und `expand` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0be80-116">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="0be80-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnitte sind `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="0be80-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0be80-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0be80-119">Request headers</span></span>
| <span data-ttu-id="0be80-120">Name</span><span class="sxs-lookup"><span data-stu-id="0be80-120">Name</span></span>       | <span data-ttu-id="0be80-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0be80-121">Type</span></span> | <span data-ttu-id="0be80-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0be80-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0be80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0be80-123">Authorization</span></span>  | <span data-ttu-id="0be80-124">string</span><span class="sxs-lookup"><span data-stu-id="0be80-124">string</span></span>  | <span data-ttu-id="0be80-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0be80-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0be80-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0be80-127">Accept</span></span> | <span data-ttu-id="0be80-128">string</span><span class="sxs-lookup"><span data-stu-id="0be80-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0be80-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0be80-129">Request body</span></span>
<span data-ttu-id="0be80-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0be80-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0be80-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be80-131">Response</span></span>

<span data-ttu-id="0be80-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [section](../resources/section.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0be80-132">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0be80-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0be80-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0be80-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be80-134">Request</span></span>
<span data-ttu-id="0be80-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0be80-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="0be80-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be80-136">Response</span></span>
<span data-ttu-id="0be80-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0be80-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->