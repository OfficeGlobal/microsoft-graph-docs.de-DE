# <a name="get-eventmessage"></a><span data-ttu-id="76558-101">eventMessage abrufen</span><span class="sxs-lookup"><span data-stu-id="76558-101">Get eventMessage</span></span>

<span data-ttu-id="76558-102">Dient zum Abrufen der Eigenschaften und Beziehungen eines [eventmessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="76558-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="76558-103">Zurzeit gibt dieser Vorgang Ereignisnachrichtentext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="76558-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76558-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="76558-104">Prerequisites</span></span>
<span data-ttu-id="76558-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="76558-105">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="76558-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76558-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="76558-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="76558-107">Optional query parameters</span></span>
<span data-ttu-id="76558-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="76558-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="76558-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76558-109">Request headers</span></span>
| <span data-ttu-id="76558-110">Name</span><span class="sxs-lookup"><span data-stu-id="76558-110">Name</span></span>       | <span data-ttu-id="76558-111">Typ</span><span class="sxs-lookup"><span data-stu-id="76558-111">Type</span></span> | <span data-ttu-id="76558-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76558-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="76558-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="76558-113">Authorization</span></span>  | <span data-ttu-id="76558-114">string</span><span class="sxs-lookup"><span data-stu-id="76558-114">string</span></span>  | <span data-ttu-id="76558-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="76558-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76558-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76558-117">Request body</span></span>
<span data-ttu-id="76558-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="76558-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76558-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="76558-119">Response</span></span>

<span data-ttu-id="76558-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76558-120">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76558-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76558-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76558-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76558-122">Request</span></span>
<span data-ttu-id="76558-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76558-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="76558-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="76558-124">Response</span></span>
<span data-ttu-id="76558-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76558-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
