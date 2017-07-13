<span data-ttu-id="71be8-p101">Dient zum Abrufen der Eigenschaften und der Beziehungen einer [Drive](../resources/drive.md)-Ressource. Ein Laufwerk ist der Container auf oberster Ebene für ein Dateisystem. Mit der Graph-API können Sie auf die Drive-Ressource für OneDrive oder OneDrive for Business eines Benutzers oder auf SharePoint-Dokumentbibliotheken zugreifen.</span><span class="sxs-lookup"><span data-stu-id="71be8-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

Dient zum Abrufen der Eigenschaften und der Beziehungen einer [Drive](../resources/drive.md)-Ressource. Ein Laufwerk ist der Container auf oberster Ebene für ein Dateisystem. Mit der Graph-API können Sie auf die Drive-Ressource für OneDrive oder OneDrive for Business eines Benutzers oder auf SharePoint-Dokumentbibliotheken zugreifen.

## <span data-ttu-id="71be8-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71be8-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>

<span data-ttu-id="71be8-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="71be8-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="71be8-107">Files.Read</span><span class="sxs-lookup"><span data-stu-id="71be8-107">Files.Read</span></span>
* <span data-ttu-id="71be8-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71be8-108">Files.ReadWrite</span></span>
* <span data-ttu-id="71be8-109">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="71be8-109">Files.Read.All</span></span>
* <span data-ttu-id="71be8-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71be8-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="71be8-111">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="71be8-111">Sites.Read.All</span></span>
* <span data-ttu-id="71be8-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71be8-112">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="71be8-113">Abrufen von OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="71be8-113">Get a user's OneDrive</span></span>
<a id="get-a-users-onedrive" class="xliff"></a>

<span data-ttu-id="71be8-114">Damit Sie auf OneDrive oder OneDrive for Business eines Benutzers zugreifen können, muss Ihre App die **drive**-Beziehung in der [User](../resources/user.md)-Ressource anfordern.</span><span class="sxs-lookup"><span data-stu-id="71be8-114">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

### <span data-ttu-id="71be8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71be8-115">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <span data-ttu-id="71be8-116">Dient zum Abrufen der Dokumentbibliothek, die einer Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="71be8-116">Get the document library associated with a group</span></span>
<a id="get-the-document-library-associated-with-a-group" class="xliff"></a>

<span data-ttu-id="71be8-117">Für den Zugriff auf die Standarddokumentbibliothek einer [Gruppe](../resources/group.md) fordert Ihre App die **drive**-Beziehung in der Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="71be8-117">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

### <span data-ttu-id="71be8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71be8-118">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <span data-ttu-id="71be8-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="71be8-119">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>

<span data-ttu-id="71be8-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71be8-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="71be8-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71be8-121">Request body</span></span>
<a id="request-body" class="xliff"></a>

<span data-ttu-id="71be8-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71be8-122">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="71be8-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="71be8-123">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="71be8-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [Drive](../resources/drive.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71be8-124">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <span data-ttu-id="71be8-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71be8-125">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="71be8-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71be8-126">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="71be8-127">Nachfolgend finden Sie ein Beispiel für die Anforderung zum Abrufen  von OneDrive oder OneDrive for Business des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="71be8-127">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <span data-ttu-id="71be8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="71be8-128">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="71be8-129">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71be8-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",    
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
