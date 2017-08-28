# <a name="get-message"></a><span data-ttu-id="c0060-101">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="c0060-101">Get message</span></span>

<span data-ttu-id="c0060-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines [message](../resources/message.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="c0060-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c0060-103">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **message**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="c0060-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="c0060-104">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="c0060-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0060-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0060-105">Permissions</span></span>
<span data-ttu-id="c0060-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c0060-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0060-108">Permission type</span></span>      | <span data-ttu-id="c0060-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0060-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0060-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0060-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0060-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c0060-111">Mail.Read</span></span>    |
|<span data-ttu-id="c0060-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0060-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0060-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c0060-113">Mail.Read</span></span>    |
|<span data-ttu-id="c0060-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0060-114">Application</span></span> | <span data-ttu-id="c0060-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c0060-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0060-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0060-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0060-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c0060-117">Optional query parameters</span></span>
<span data-ttu-id="c0060-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c0060-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0060-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0060-119">Request headers</span></span>
| <span data-ttu-id="c0060-120">Name</span><span class="sxs-lookup"><span data-stu-id="c0060-120">Name</span></span>       | <span data-ttu-id="c0060-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c0060-121">Type</span></span> | <span data-ttu-id="c0060-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0060-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0060-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0060-123">Authorization</span></span>  | <span data-ttu-id="c0060-124">string</span><span class="sxs-lookup"><span data-stu-id="c0060-124">string</span></span>  | <span data-ttu-id="c0060-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0060-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0060-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0060-127">Request body</span></span>
<span data-ttu-id="c0060-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0060-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0060-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0060-129">Response</span></span>

<span data-ttu-id="c0060-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0060-130">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0060-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0060-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0060-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0060-132">Request</span></span>
<span data-ttu-id="c0060-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0060-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="c0060-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0060-134">Response</span></span>
<span data-ttu-id="c0060-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0060-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c0060-138">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="c0060-138">See also</span></span>

- [<span data-ttu-id="c0060-139">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="c0060-139">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c0060-140">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="c0060-140">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
