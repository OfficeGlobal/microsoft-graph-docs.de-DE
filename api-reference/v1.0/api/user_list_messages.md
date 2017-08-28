# <a name="list-messages"></a><span data-ttu-id="0d66f-101">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="0d66f-101">List messages</span></span>

<span data-ttu-id="0d66f-102">Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“).</span><span class="sxs-lookup"><span data-stu-id="0d66f-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="0d66f-103">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="0d66f-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d66f-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d66f-104">Permissions</span></span>
<span data-ttu-id="0d66f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d66f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0d66f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d66f-107">Permission type</span></span>      | <span data-ttu-id="0d66f-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d66f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d66f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d66f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0d66f-110">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d66f-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0d66f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d66f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d66f-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d66f-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0d66f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d66f-113">Application</span></span> | <span data-ttu-id="0d66f-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d66f-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d66f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d66f-115">HTTP request</span></span>

<span data-ttu-id="0d66f-116">So rufen Sie alle Nachrichten in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="0d66f-116">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="0d66f-117">So rufen Sie Nachrichten in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="0d66f-117">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d66f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0d66f-118">Optional query parameters</span></span>
<span data-ttu-id="0d66f-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0d66f-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0d66f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d66f-120">Request headers</span></span>
| <span data-ttu-id="0d66f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0d66f-121">Header</span></span>       | <span data-ttu-id="0d66f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0d66f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d66f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d66f-123">Authorization</span></span>  | <span data-ttu-id="0d66f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d66f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d66f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d66f-126">Request body</span></span>
<span data-ttu-id="0d66f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0d66f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d66f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d66f-128">Response</span></span>

<span data-ttu-id="0d66f-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d66f-129">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="0d66f-130">Die Standardseitengröße für diese Anforderung liegt bei 10 Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="0d66f-130">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="0d66f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d66f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d66f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d66f-132">Request</span></span>
<span data-ttu-id="0d66f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d66f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="0d66f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d66f-134">Response</span></span>
<span data-ttu-id="0d66f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d66f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
