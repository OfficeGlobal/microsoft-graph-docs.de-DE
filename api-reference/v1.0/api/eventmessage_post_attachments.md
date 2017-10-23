# <a name="add-attachment"></a><span data-ttu-id="13c57-101">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="13c57-101">Add attachment</span></span>

<span data-ttu-id="13c57-102">Verwenden Sie diese API, um eine neue Anlage zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="13c57-102">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="13c57-103">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="13c57-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="13c57-104">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="13c57-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="13c57-105">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="13c57-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="13c57-106">Link zu einer Datei ([referenceAttachment](../resources/referenceAttachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="13c57-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="13c57-107">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="13c57-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="13c57-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13c57-108">Permissions</span></span>
<span data-ttu-id="13c57-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="13c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13c57-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13c57-111">Permission type</span></span>      | <span data-ttu-id="13c57-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13c57-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13c57-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13c57-113">Delegated (work or school account)</span></span> | <span data-ttu-id="13c57-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13c57-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13c57-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13c57-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13c57-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13c57-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13c57-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13c57-117">Application</span></span> | <span data-ttu-id="13c57-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13c57-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13c57-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13c57-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="13c57-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13c57-120">Request headers</span></span>
| <span data-ttu-id="13c57-121">Name</span><span class="sxs-lookup"><span data-stu-id="13c57-121">Name</span></span>       | <span data-ttu-id="13c57-122">Typ</span><span class="sxs-lookup"><span data-stu-id="13c57-122">Type</span></span> | <span data-ttu-id="13c57-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13c57-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13c57-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="13c57-124">Authorization</span></span>  | <span data-ttu-id="13c57-125">string</span><span class="sxs-lookup"><span data-stu-id="13c57-125">string</span></span>  | <span data-ttu-id="13c57-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13c57-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13c57-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13c57-128">Content-Type</span></span> | <span data-ttu-id="13c57-129">string</span><span class="sxs-lookup"><span data-stu-id="13c57-129">string</span></span>  | <span data-ttu-id="13c57-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13c57-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13c57-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13c57-132">Request body</span></span>
<span data-ttu-id="13c57-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="13c57-133">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="13c57-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="13c57-134">Response</span></span>

<span data-ttu-id="13c57-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13c57-135">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="13c57-136">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="13c57-136">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="13c57-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13c57-137">Request</span></span>
<span data-ttu-id="13c57-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13c57-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="13c57-139">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="13c57-139">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="13c57-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="13c57-140">Response</span></span>
<span data-ttu-id="13c57-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13c57-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="13c57-144">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="13c57-144">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="13c57-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13c57-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="13c57-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="13c57-146">Response</span></span>
<span data-ttu-id="13c57-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13c57-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
