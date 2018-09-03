# <a name="add-attachment"></a><span data-ttu-id="ea9a6-101">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ea9a6-101">Add attachment</span></span>

<span data-ttu-id="ea9a6-p101">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Beitrag. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="ea9a6-104">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="ea9a6-104">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="ea9a6-105">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-105">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="ea9a6-106">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-106">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="ea9a6-107">Link zu einer Datei ([referenceAttachment](../resources/referenceAttachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-107">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="ea9a6-108">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-108">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ea9a6-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ea9a6-109">Permissions</span></span>
<span data-ttu-id="ea9a6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea9a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea9a6-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea9a6-112">Permission type</span></span>      | <span data-ttu-id="ea9a6-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea9a6-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ea9a6-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9a6-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea9a6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea9a6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea9a6-117">Not supported.</span></span>    |
|<span data-ttu-id="ea9a6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea9a6-118">Application</span></span> | <span data-ttu-id="ea9a6-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9a6-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea9a6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea9a6-120">HTTP request</span></span>
<span data-ttu-id="ea9a6-121"><!-- { "blockType": "ignored" } --> Anlagen für einen [Beitrag](../resources/post.md) in einer [Diskussion](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="ea9a6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea9a6-122">Request headers</span></span>
| <span data-ttu-id="ea9a6-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea9a6-123">Header</span></span>       | <span data-ttu-id="ea9a6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ea9a6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea9a6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ea9a6-125">Authorization</span></span>  | <span data-ttu-id="ea9a6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea9a6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea9a6-128">Request body</span></span>
<span data-ttu-id="ea9a6-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-129">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea9a6-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea9a6-130">Response</span></span>

<span data-ttu-id="ea9a6-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-131">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="ea9a6-132">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-132">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="ea9a6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea9a6-133">Request</span></span>
<span data-ttu-id="ea9a6-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-134">Here is an example of the request.</span></span>
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
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="ea9a6-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ea9a6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea9a6-136">Response</span></span>
<span data-ttu-id="ea9a6-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="ea9a6-140">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="ea9a6-140">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="ea9a6-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea9a6-141">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="ea9a6-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea9a6-142">Response</span></span>
<span data-ttu-id="ea9a6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea9a6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
