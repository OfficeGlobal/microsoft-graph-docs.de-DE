# <a name="list-childfolders"></a><span data-ttu-id="7e4c9-101">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="7e4c9-101">List childFolders</span></span>

<span data-ttu-id="7e4c9-p101">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`-Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e4c9-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="7e4c9-104">Prerequisites</span></span>
<span data-ttu-id="7e4c9-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Read; Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="7e4c9-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="7e4c9-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e4c9-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7e4c9-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7e4c9-107">Optional query parameters</span></span>
<span data-ttu-id="7e4c9-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7e4c9-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e4c9-109">Request headers</span></span>
| <span data-ttu-id="7e4c9-110">Name</span><span class="sxs-lookup"><span data-stu-id="7e4c9-110">Name</span></span>       | <span data-ttu-id="7e4c9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7e4c9-111">Type</span></span> | <span data-ttu-id="7e4c9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e4c9-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e4c9-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e4c9-113">Authorization</span></span>  | <span data-ttu-id="7e4c9-114">string</span><span class="sxs-lookup"><span data-stu-id="7e4c9-114">string</span></span>  | <span data-ttu-id="7e4c9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e4c9-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e4c9-117">Request body</span></span>
<span data-ttu-id="7e4c9-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e4c9-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e4c9-119">Response</span></span>

<span data-ttu-id="7e4c9-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-120">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e4c9-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e4c9-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e4c9-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e4c9-122">Request</span></span>
<span data-ttu-id="7e4c9-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="7e4c9-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e4c9-124">Response</span></span>
<span data-ttu-id="7e4c9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e4c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
