# <a name="get-drive"></a><span data-ttu-id="673a9-101">Laufwerk abrufen</span><span class="sxs-lookup"><span data-stu-id="673a9-101">Get Drive</span></span>

<span data-ttu-id="673a9-p101">Dient zum Abrufen der Eigenschaften und der Beziehungen einer [Drive](../resources/drive.md)-Ressource. Ein Laufwerk ist der Container auf oberster Ebene für ein Dateisystem. Mit der Graph-API können Sie auf die Drive-Ressource für OneDrive oder OneDrive for Business eines Benutzers oder auf SharePoint-Dokumentbibliotheken zugreifen.</span><span class="sxs-lookup"><span data-stu-id="673a9-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="673a9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="673a9-105">Permissions</span></span>

<span data-ttu-id="673a9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="673a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="673a9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="673a9-108">Permission type</span></span>      | <span data-ttu-id="673a9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="673a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="673a9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="673a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="673a9-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673a9-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="673a9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="673a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="673a9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673a9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="673a9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="673a9-114">Application</span></span> | <span data-ttu-id="673a9-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673a9-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-a-users-onedrive"></a><span data-ttu-id="673a9-116">Abrufen des OneDrive eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="673a9-116">Get a user's OneDrive</span></span>

<span data-ttu-id="673a9-117">Damit Sie auf OneDrive oder OneDrive for Business eines Benutzers zugreifen können, muss Ihre App die **drive**-Beziehung in der [User](../resources/user.md)-Ressource anfordern.</span><span class="sxs-lookup"><span data-stu-id="673a9-117">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="673a9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="673a9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="673a9-119">Dient zum Abrufen der Dokumentbibliothek, die einer Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="673a9-119">Get the document library associated with a group</span></span>

<span data-ttu-id="673a9-120">Für den Zugriff auf die Standarddokumentbibliothek einer [Gruppe](../resources/group.md) fordert Ihre App die **drive**-Beziehung in der Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="673a9-120">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="673a9-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="673a9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="673a9-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="673a9-122">Optional query parameters</span></span>

<span data-ttu-id="673a9-123">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) von `$expand` und `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="673a9-123">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="673a9-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="673a9-124">Request body</span></span>

<span data-ttu-id="673a9-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="673a9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="673a9-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="673a9-126">Response</span></span>

<span data-ttu-id="673a9-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [Drive](../resources/drive.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="673a9-127">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="673a9-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="673a9-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="673a9-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="673a9-129">Request</span></span>

<span data-ttu-id="673a9-130">Nachfolgend finden Sie ein Beispiel für die Anforderung zum Abrufen  von OneDrive oder OneDrive for Business des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="673a9-130">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="673a9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="673a9-131">Response</span></span>

<span data-ttu-id="673a9-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="673a9-132">Here is an example of the response.</span></span>

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
