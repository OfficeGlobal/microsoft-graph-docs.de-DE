# <a name="get-post"></a><span data-ttu-id="1b6e0-101">Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="1b6e0-101">Get post</span></span>

<span data-ttu-id="1b6e0-p101">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="1b6e0-104">Da die **post**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **post**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b6e0-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b6e0-105">Prerequisites</span></span>
<span data-ttu-id="1b6e0-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="1b6e0-106">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="1b6e0-107">*Group.Read.All*, *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="1b6e0-107">*Group.Read.All*, *Group.Readwrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="1b6e0-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b6e0-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b6e0-109">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1b6e0-109">Optional query parameters</span></span>
<span data-ttu-id="1b6e0-110">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1b6e0-111">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b6e0-111">Request headers</span></span>
| <span data-ttu-id="1b6e0-112">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1b6e0-112">Header</span></span>       | <span data-ttu-id="1b6e0-113">Wert</span><span class="sxs-lookup"><span data-stu-id="1b6e0-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b6e0-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b6e0-114">Authorization</span></span>  | <span data-ttu-id="1b6e0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b6e0-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b6e0-117">Request body</span></span>
<span data-ttu-id="1b6e0-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b6e0-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b6e0-119">Response</span></span>

<span data-ttu-id="1b6e0-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/post.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-120">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b6e0-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b6e0-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b6e0-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b6e0-122">Request</span></span>
<span data-ttu-id="1b6e0-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="1b6e0-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b6e0-124">Response</span></span>
<span data-ttu-id="1b6e0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b6e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

{
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "receivedDateTime": "datetime-value",
  "hasAttachments": true,
  "from": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  },
  "sender": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="1b6e0-128">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="1b6e0-128">See also</span></span>

- [<span data-ttu-id="1b6e0-129">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1b6e0-129">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="1b6e0-130">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="1b6e0-130">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
