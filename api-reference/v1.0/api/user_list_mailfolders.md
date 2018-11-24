# <a name="list-mailfolders"></a><span data-ttu-id="9c578-101">mailFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="9c578-101">List mailFolders</span></span>

<span data-ttu-id="9c578-102">Mit dieser API können Sie die E-Mail-Ordner-Sammlung im Stammordner des angemeldeten Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="9c578-102">Get the mail folder collection under the root folder of the signed-in user.</span></span> 
## <a name="permissions"></a><span data-ttu-id="9c578-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c578-103">Permissions</span></span>
<span data-ttu-id="9c578-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9c578-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c578-106">Permission type</span></span>      | <span data-ttu-id="9c578-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c578-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c578-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c578-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9c578-109">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c578-109">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9c578-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c578-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c578-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c578-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9c578-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c578-112">Application</span></span> | <span data-ttu-id="9c578-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c578-113">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c578-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c578-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c578-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9c578-115">Optional query parameters</span></span>
<span data-ttu-id="9c578-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c578-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9c578-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c578-117">Request headers</span></span>
| <span data-ttu-id="9c578-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c578-118">Header</span></span>       | <span data-ttu-id="9c578-119">Wert</span><span class="sxs-lookup"><span data-stu-id="9c578-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c578-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c578-120">Authorization</span></span>  | <span data-ttu-id="9c578-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c578-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9c578-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c578-123">Content-Type</span></span>   | <span data-ttu-id="9c578-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9c578-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c578-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c578-125">Request body</span></span>
<span data-ttu-id="9c578-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c578-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c578-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c578-127">Response</span></span>

<span data-ttu-id="9c578-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c578-128">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c578-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c578-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c578-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c578-130">Request</span></span>
<span data-ttu-id="9c578-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c578-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="9c578-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c578-132">Response</span></span>
<span data-ttu-id="9c578-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c578-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
