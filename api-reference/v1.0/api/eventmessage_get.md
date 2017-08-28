# <a name="get-eventmessage"></a><span data-ttu-id="7bbca-101">eventMessage abrufen</span><span class="sxs-lookup"><span data-stu-id="7bbca-101">Get eventMessage</span></span>

<span data-ttu-id="7bbca-102">Dient zum Abrufen der Eigenschaften und Beziehungen eines [eventmessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7bbca-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="7bbca-103">Zurzeit gibt dieser Vorgang Ereignisnachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="7bbca-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bbca-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7bbca-104">Permissions</span></span>
<span data-ttu-id="7bbca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bbca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7bbca-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7bbca-107">Permission type</span></span>      | <span data-ttu-id="7bbca-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7bbca-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bbca-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7bbca-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7bbca-110">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7bbca-110">Mail.Read</span></span>    |
|<span data-ttu-id="7bbca-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7bbca-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bbca-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7bbca-112">Mail.Read</span></span>    |
|<span data-ttu-id="7bbca-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7bbca-113">Application</span></span> | <span data-ttu-id="7bbca-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7bbca-114">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bbca-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bbca-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7bbca-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7bbca-116">Optional query parameters</span></span>
<span data-ttu-id="7bbca-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7bbca-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7bbca-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7bbca-118">Request headers</span></span>
| <span data-ttu-id="7bbca-119">Name</span><span class="sxs-lookup"><span data-stu-id="7bbca-119">Name</span></span>       | <span data-ttu-id="7bbca-120">Typ</span><span class="sxs-lookup"><span data-stu-id="7bbca-120">Type</span></span> | <span data-ttu-id="7bbca-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bbca-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7bbca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bbca-122">Authorization</span></span>  | <span data-ttu-id="7bbca-123">string</span><span class="sxs-lookup"><span data-stu-id="7bbca-123">string</span></span>  | <span data-ttu-id="7bbca-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7bbca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bbca-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7bbca-126">Request body</span></span>
<span data-ttu-id="7bbca-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7bbca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bbca-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bbca-128">Response</span></span>

<span data-ttu-id="7bbca-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bbca-129">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bbca-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7bbca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bbca-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bbca-131">Request</span></span>
<span data-ttu-id="7bbca-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7bbca-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="7bbca-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bbca-133">Response</span></span>
<span data-ttu-id="7bbca-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bbca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
