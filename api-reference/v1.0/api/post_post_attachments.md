# <a name="add-attachment"></a><span data-ttu-id="9ebf4-101">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="9ebf4-101">Add attachment</span></span>

<span data-ttu-id="9ebf4-p101">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Beitrag. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ebf4-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ebf4-104">Permissions</span></span>
<span data-ttu-id="9ebf4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ebf4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ebf4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ebf4-107">Permission type</span></span>      | <span data-ttu-id="9ebf4-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ebf4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ebf4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ebf4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9ebf4-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ebf4-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ebf4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ebf4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ebf4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ebf4-112">Not supported.</span></span>    |
|<span data-ttu-id="9ebf4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ebf4-113">Application</span></span> | <span data-ttu-id="9ebf4-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ebf4-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ebf4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ebf4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9ebf4-116">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-116">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="9ebf4-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ebf4-117">Request headers</span></span>
| <span data-ttu-id="9ebf4-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ebf4-118">Header</span></span>       | <span data-ttu-id="9ebf4-119">Wert</span><span class="sxs-lookup"><span data-stu-id="9ebf4-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ebf4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ebf4-120">Authorization</span></span>  | <span data-ttu-id="9ebf4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ebf4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ebf4-123">Request body</span></span>
<span data-ttu-id="9ebf4-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-124">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ebf4-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ebf4-125">Response</span></span>

<span data-ttu-id="9ebf4-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-126">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="9ebf4-127">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="9ebf4-127">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9ebf4-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ebf4-128">Request</span></span>
<span data-ttu-id="9ebf4-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-129">Here is an example of the request.</span></span>
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

<span data-ttu-id="9ebf4-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-130">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="9ebf4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ebf4-131">Response</span></span>
<span data-ttu-id="9ebf4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="9ebf4-135">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="9ebf4-135">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9ebf4-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ebf4-136">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="9ebf4-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ebf4-137">Response</span></span>
<span data-ttu-id="9ebf4-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ebf4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
