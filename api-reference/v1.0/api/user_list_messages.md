# <a name="list-messages"></a><span data-ttu-id="f6524-101">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="f6524-101">List messages</span></span>

<span data-ttu-id="f6524-102">Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“).</span><span class="sxs-lookup"><span data-stu-id="f6524-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="f6524-103">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="f6524-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="f6524-104">Es gibt zwei Szenarien, in dem eine app Nachrichten in einen anderen Benutzer e-Mail-Ordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="f6524-104">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="f6524-105">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="f6524-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f6524-106">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen e-Mail-Ordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="f6524-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f6524-107">Finden Sie [ausführliche Informationen und ein Beispiel](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="f6524-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6524-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f6524-108">Permissions</span></span>
<span data-ttu-id="f6524-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6524-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6524-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6524-111">Permission type</span></span>      | <span data-ttu-id="f6524-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6524-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6524-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6524-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f6524-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6524-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6524-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6524-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6524-116">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6524-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6524-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6524-117">Application</span></span> | <span data-ttu-id="f6524-118">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6524-118">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6524-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6524-119">HTTP request</span></span>

<span data-ttu-id="f6524-120">So rufen Sie alle Nachrichten in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="f6524-120">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="f6524-121">So rufen Sie Nachrichten in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="f6524-121">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6524-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f6524-122">Optional query parameters</span></span>
<span data-ttu-id="f6524-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6524-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f6524-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6524-124">Request headers</span></span>
| <span data-ttu-id="f6524-125">Name</span><span class="sxs-lookup"><span data-stu-id="f6524-125">Name</span></span>       | <span data-ttu-id="f6524-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f6524-126">Type</span></span> | <span data-ttu-id="f6524-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6524-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6524-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6524-128">Authorization</span></span>  | <span data-ttu-id="f6524-129">string</span><span class="sxs-lookup"><span data-stu-id="f6524-129">string</span></span>  | <span data-ttu-id="f6524-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6524-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6524-132">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f6524-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f6524-133">string</span><span class="sxs-lookup"><span data-stu-id="f6524-133">string</span></span> | <span data-ttu-id="f6524-134">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f6524-134">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="f6524-135">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="f6524-135">Values can be "text" or "html".</span></span> <span data-ttu-id="f6524-136">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6524-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="f6524-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="f6524-137">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f6524-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6524-138">Request body</span></span>
<span data-ttu-id="f6524-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6524-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6524-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6524-140">Response</span></span>

<span data-ttu-id="f6524-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6524-141">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="f6524-142">Die Standardseitengröße für diese Anforderung liegt bei 10 Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="f6524-142">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="f6524-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6524-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6524-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6524-144">Request</span></span>
<span data-ttu-id="f6524-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6524-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="f6524-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6524-146">Response</span></span>
<span data-ttu-id="f6524-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6524-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
