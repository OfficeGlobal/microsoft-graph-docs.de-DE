# <a name="list-messages"></a><span data-ttu-id="fda88-101">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="fda88-101">List messages</span></span>

<span data-ttu-id="fda88-102">Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“).</span><span class="sxs-lookup"><span data-stu-id="fda88-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="fda88-103">Zurzeit gibt diesen Vorgang Nachrichtentext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="fda88-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fda88-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="fda88-104">Prerequisites</span></span>
<span data-ttu-id="fda88-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Read; Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="fda88-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="fda88-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fda88-106">HTTP request</span></span>

<span data-ttu-id="fda88-107">So rufen Sie alle Nachrichten in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="fda88-107">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="fda88-108">So rufen Sie Nachrichten in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="fda88-108">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fda88-109">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fda88-109">Optional query parameters</span></span>
<span data-ttu-id="fda88-110">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fda88-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fda88-111">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fda88-111">Request headers</span></span>
| <span data-ttu-id="fda88-112">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fda88-112">Header</span></span>       | <span data-ttu-id="fda88-113">Wert</span><span class="sxs-lookup"><span data-stu-id="fda88-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fda88-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda88-114">Authorization</span></span>  | <span data-ttu-id="fda88-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fda88-p101">Bearer {token}. Required.</span></span>  |
 

## <a name="request-body"></a><span data-ttu-id="fda88-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fda88-117">Request body</span></span>
<span data-ttu-id="fda88-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fda88-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fda88-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="fda88-119">Response</span></span>

<span data-ttu-id="fda88-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fda88-120">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="fda88-121">Die Standardseitengröße für diese Anforderung liegt bei 10 Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="fda88-121">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="fda88-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fda88-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fda88-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fda88-123">Request</span></span>
<span data-ttu-id="fda88-124">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fda88-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="fda88-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="fda88-125">Response</span></span>
<span data-ttu-id="fda88-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fda88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
