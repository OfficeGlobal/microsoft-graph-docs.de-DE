# <a name="list-childfolders"></a><span data-ttu-id="89736-101">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="89736-101">List childFolders</span></span>

<span data-ttu-id="89736-p101">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`-Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="89736-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="89736-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="89736-104">Permissions</span></span>
<span data-ttu-id="89736-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="89736-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89736-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89736-107">Permission type</span></span>      | <span data-ttu-id="89736-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89736-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89736-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89736-109">Delegated (work or school account)</span></span> | <span data-ttu-id="89736-110">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89736-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="89736-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89736-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89736-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89736-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="89736-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89736-113">Application</span></span> | <span data-ttu-id="89736-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89736-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="89736-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89736-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89736-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="89736-116">Optional query parameters</span></span>
<span data-ttu-id="89736-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89736-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="89736-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89736-118">Request headers</span></span>
| <span data-ttu-id="89736-119">Name</span><span class="sxs-lookup"><span data-stu-id="89736-119">Name</span></span>       | <span data-ttu-id="89736-120">Typ</span><span class="sxs-lookup"><span data-stu-id="89736-120">Type</span></span> | <span data-ttu-id="89736-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89736-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89736-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89736-122">Authorization</span></span>  | <span data-ttu-id="89736-123">string</span><span class="sxs-lookup"><span data-stu-id="89736-123">string</span></span>  | <span data-ttu-id="89736-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89736-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89736-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89736-126">Request body</span></span>
<span data-ttu-id="89736-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="89736-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89736-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="89736-128">Response</span></span>

<span data-ttu-id="89736-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89736-129">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89736-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89736-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89736-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89736-131">Request</span></span>
<span data-ttu-id="89736-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89736-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="89736-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="89736-133">Response</span></span>
<span data-ttu-id="89736-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89736-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
