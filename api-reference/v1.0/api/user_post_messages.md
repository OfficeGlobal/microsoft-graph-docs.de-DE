# <a name="create-message"></a><span data-ttu-id="80f73-101">Nachricht erstellen</span><span class="sxs-lookup"><span data-stu-id="80f73-101">Create Message</span></span>

<span data-ttu-id="80f73-p101">Verwenden Sie diese API zum Erstellen eines Entwurfs einer neuen Nachricht. Entwürfe können in einem beliebigen Ordner erstellt und optional vor dem Senden aktualisiert werden. Verwenden Sie die Verknüpfung „/messages“, um den Entwurf im Ordner „Entwürfe“ zu speichern.</span><span class="sxs-lookup"><span data-stu-id="80f73-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="80f73-105">Beim Erstellen des Entwurfs im selben **POST**-Aufruf können Sie eine [Anlage](../resources/attachment.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="80f73-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80f73-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="80f73-106">Permissions</span></span>
<span data-ttu-id="80f73-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="80f73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80f73-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80f73-109">Permission type</span></span>      | <span data-ttu-id="80f73-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80f73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80f73-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80f73-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80f73-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f73-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="80f73-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80f73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80f73-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f73-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="80f73-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80f73-115">Application</span></span> | <span data-ttu-id="80f73-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f73-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="80f73-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="80f73-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80f73-118">Request headers</span></span>
| <span data-ttu-id="80f73-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="80f73-119">Header</span></span>       | <span data-ttu-id="80f73-120">Wert</span><span class="sxs-lookup"><span data-stu-id="80f73-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80f73-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80f73-121">Authorization</span></span>  | <span data-ttu-id="80f73-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80f73-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="80f73-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80f73-124">Content-Type</span></span>  | <span data-ttu-id="80f73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80f73-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80f73-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80f73-126">Request body</span></span>
<span data-ttu-id="80f73-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="80f73-127">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="80f73-128">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie den `POST`-Vorgang verwenden und während der Erstellung der Nachricht benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="80f73-128">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="80f73-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f73-129">Response</span></span>

<span data-ttu-id="80f73-130">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80f73-130">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f73-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80f73-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="80f73-132">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="80f73-132">Request 1</span></span>
<span data-ttu-id="80f73-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80f73-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json
Content-length: 248

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
```
<span data-ttu-id="80f73-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [message](../resources/message.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="80f73-134">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="80f73-135">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="80f73-135">Response 1</span></span>
<span data-ttu-id="80f73-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80f73-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 248

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
```

## <a name="see-also"></a><span data-ttu-id="80f73-139">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="80f73-139">See also</span></span>

- [<span data-ttu-id="80f73-140">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="80f73-140">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="80f73-141">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="80f73-141">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
