# <a name="create-notebook"></a><span data-ttu-id="73c89-101">Notizbuch erstellen</span><span class="sxs-lookup"><span data-stu-id="73c89-101">Create notebook</span></span>

<span data-ttu-id="73c89-102">Mit dieser API können Sie eine neue OneNote-Ressource des Typs [notebook](../resources/notebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="73c89-102">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="73c89-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="73c89-103">Permissions</span></span>
<span data-ttu-id="73c89-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73c89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73c89-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73c89-106">Permission type</span></span>      | <span data-ttu-id="73c89-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73c89-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="73c89-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73c89-108">Delegated (work or school account)</span></span> | <span data-ttu-id="73c89-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c89-109">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="73c89-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73c89-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73c89-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c89-111">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="73c89-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73c89-112">Application</span></span> | <span data-ttu-id="73c89-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c89-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="73c89-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73c89-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="73c89-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73c89-115">Request headers</span></span>
| <span data-ttu-id="73c89-116">Name</span><span class="sxs-lookup"><span data-stu-id="73c89-116">Name</span></span>       | <span data-ttu-id="73c89-117">Typ</span><span class="sxs-lookup"><span data-stu-id="73c89-117">Type</span></span> | <span data-ttu-id="73c89-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73c89-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73c89-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="73c89-119">Authorization</span></span>  | <span data-ttu-id="73c89-120">string</span><span class="sxs-lookup"><span data-stu-id="73c89-120">string</span></span>  | <span data-ttu-id="73c89-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73c89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73c89-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73c89-123">Content-Type</span></span> | <span data-ttu-id="73c89-124">string</span><span class="sxs-lookup"><span data-stu-id="73c89-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="73c89-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73c89-125">Request body</span></span>
<span data-ttu-id="73c89-126">Geben Sie im Anforderungstext einen Namen für das Notizbuch an.</span><span class="sxs-lookup"><span data-stu-id="73c89-126">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="73c89-p103">Notizbuchnamen müssen eindeutig sein. Der Name darf nicht mehr als 128 Zeichen und keines der folgenden Zeichen enthalten: ?*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="73c89-p103">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="73c89-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="73c89-129">Response</span></span>

<span data-ttu-id="73c89-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das neue [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73c89-130">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73c89-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73c89-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73c89-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73c89-132">Request</span></span>
<span data-ttu-id="73c89-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73c89-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="73c89-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="73c89-134">Response</span></span>
<span data-ttu-id="73c89-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73c89-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->