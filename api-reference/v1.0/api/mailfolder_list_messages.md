# <a name="list-messages"></a><span data-ttu-id="35139-101">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="35139-101">List messages</span></span>

<span data-ttu-id="35139-102">Mit dieser API können Sie alle Nachrichten im Postfach des angemeldeten Benutzers abrufen oder alle Nachrichten in einem bestimmten Ordner in diesem Postfach.</span><span class="sxs-lookup"><span data-stu-id="35139-102">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="35139-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="35139-103">Permissions</span></span>
<span data-ttu-id="35139-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="35139-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="35139-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35139-106">Permission type</span></span>      | <span data-ttu-id="35139-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35139-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35139-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35139-108">Delegated (work or school account)</span></span> | <span data-ttu-id="35139-109">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35139-109">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35139-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35139-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35139-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35139-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35139-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35139-112">Application</span></span> | <span data-ttu-id="35139-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35139-113">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35139-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35139-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35139-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="35139-115">Optional query parameters</span></span>
<span data-ttu-id="35139-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="35139-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35139-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35139-117">Request headers</span></span>
| <span data-ttu-id="35139-118">Name</span><span class="sxs-lookup"><span data-stu-id="35139-118">Name</span></span>       | <span data-ttu-id="35139-119">Typ</span><span class="sxs-lookup"><span data-stu-id="35139-119">Type</span></span> | <span data-ttu-id="35139-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35139-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="35139-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="35139-121">Authorization</span></span>  | <span data-ttu-id="35139-122">string</span><span class="sxs-lookup"><span data-stu-id="35139-122">string</span></span>  | <span data-ttu-id="35139-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="35139-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35139-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35139-125">Request body</span></span>
<span data-ttu-id="35139-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35139-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35139-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="35139-127">Response</span></span>

<span data-ttu-id="35139-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35139-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35139-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35139-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35139-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35139-130">Request</span></span>
<span data-ttu-id="35139-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35139-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="35139-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="35139-132">Response</span></span>
<span data-ttu-id="35139-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35139-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
