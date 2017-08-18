# <a name="add-attachment"></a><span data-ttu-id="9f223-101">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="9f223-101">Add attachment</span></span>

<span data-ttu-id="9f223-p101">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Beitrag. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="9f223-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f223-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f223-104">Prerequisites</span></span>
<span data-ttu-id="9f223-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="9f223-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="9f223-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f223-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9f223-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f223-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9f223-108">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="9f223-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="9f223-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f223-109">Request headers</span></span>
| <span data-ttu-id="9f223-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f223-110">Header</span></span>       | <span data-ttu-id="9f223-111">Wert</span><span class="sxs-lookup"><span data-stu-id="9f223-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f223-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f223-112">Authorization</span></span>  | <span data-ttu-id="9f223-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f223-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f223-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f223-115">Request body</span></span>
<span data-ttu-id="9f223-116">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9f223-116">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f223-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f223-117">Response</span></span>

<span data-ttu-id="9f223-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f223-118">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="9f223-119">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="9f223-119">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9f223-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f223-120">Request</span></span>
<span data-ttu-id="9f223-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f223-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="9f223-122">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9f223-122">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="9f223-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f223-123">Response</span></span>
<span data-ttu-id="9f223-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f223-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="9f223-127">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="9f223-127">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9f223-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f223-128">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="9f223-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f223-129">Response</span></span>
<span data-ttu-id="9f223-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f223-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
