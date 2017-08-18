# <a name="get-message"></a><span data-ttu-id="cf8fd-101">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="cf8fd-101">Get message</span></span>

<span data-ttu-id="cf8fd-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines [message](../resources/message.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="cf8fd-103">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **message**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="cf8fd-104">Zurzeit gibt dieser Vorgang Nachrichtentext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf8fd-105">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="cf8fd-105">Prerequisites</span></span>
<span data-ttu-id="cf8fd-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="cf8fd-106">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>  
## <a name="http-request"></a><span data-ttu-id="cf8fd-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf8fd-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf8fd-108">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf8fd-108">Optional query parameters</span></span>
<span data-ttu-id="cf8fd-109">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf8fd-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf8fd-110">Request headers</span></span>
| <span data-ttu-id="cf8fd-111">Name</span><span class="sxs-lookup"><span data-stu-id="cf8fd-111">Name</span></span>       | <span data-ttu-id="cf8fd-112">Typ</span><span class="sxs-lookup"><span data-stu-id="cf8fd-112">Type</span></span> | <span data-ttu-id="cf8fd-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf8fd-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cf8fd-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf8fd-114">Authorization</span></span>  | <span data-ttu-id="cf8fd-115">string</span><span class="sxs-lookup"><span data-stu-id="cf8fd-115">string</span></span>  | <span data-ttu-id="cf8fd-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf8fd-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf8fd-118">Request body</span></span>
<span data-ttu-id="cf8fd-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf8fd-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf8fd-120">Response</span></span>

<span data-ttu-id="cf8fd-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-121">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf8fd-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf8fd-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf8fd-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf8fd-123">Request</span></span>
<span data-ttu-id="cf8fd-124">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="cf8fd-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf8fd-125">Response</span></span>
<span data-ttu-id="cf8fd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf8fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
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
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="cf8fd-129">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="cf8fd-129">See also</span></span>

- [<span data-ttu-id="cf8fd-130">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="cf8fd-130">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="cf8fd-131">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="cf8fd-131">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
