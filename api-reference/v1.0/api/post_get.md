# <a name="get-post"></a><span data-ttu-id="32a94-101">Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="32a94-101">Get post</span></span>

<span data-ttu-id="32a94-p101">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="32a94-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="32a94-104">Da die **post**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **post**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="32a94-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="32a94-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32a94-105">Permissions</span></span>
<span data-ttu-id="32a94-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32a94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32a94-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32a94-108">Permission type</span></span>      | <span data-ttu-id="32a94-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32a94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32a94-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32a94-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32a94-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a94-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="32a94-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32a94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32a94-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32a94-113">Not supported.</span></span>    |
|<span data-ttu-id="32a94-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32a94-114">Application</span></span> | <span data-ttu-id="32a94-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a94-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32a94-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32a94-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32a94-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="32a94-117">Optional query parameters</span></span>
<span data-ttu-id="32a94-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="32a94-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32a94-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32a94-119">Request headers</span></span>
| <span data-ttu-id="32a94-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32a94-120">Header</span></span>       | <span data-ttu-id="32a94-121">Wert</span><span class="sxs-lookup"><span data-stu-id="32a94-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32a94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32a94-122">Authorization</span></span>  | <span data-ttu-id="32a94-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32a94-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32a94-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32a94-125">Request body</span></span>
<span data-ttu-id="32a94-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="32a94-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32a94-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="32a94-127">Response</span></span>

<span data-ttu-id="32a94-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/post.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32a94-128">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32a94-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32a94-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32a94-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32a94-130">Request</span></span>
<span data-ttu-id="32a94-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32a94-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="32a94-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="32a94-132">Response</span></span>
<span data-ttu-id="32a94-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32a94-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="32a94-136">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="32a94-136">See also</span></span>

- [<span data-ttu-id="32a94-137">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="32a94-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="32a94-138">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="32a94-138">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
