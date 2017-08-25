# <a name="add-attachment"></a><span data-ttu-id="561ca-101">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="561ca-101">Add attachment</span></span>

<span data-ttu-id="561ca-102">Mit dieser API können Sie neue Anlagen erstellen.</span><span class="sxs-lookup"><span data-stu-id="561ca-102">Use this API to create a new Attachment.</span></span>
## <a name="permissions"></a><span data-ttu-id="561ca-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="561ca-103">Permissions</span></span>
<span data-ttu-id="561ca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="561ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="561ca-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="561ca-106">Permission type</span></span>      | <span data-ttu-id="561ca-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="561ca-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="561ca-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="561ca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="561ca-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="561ca-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="561ca-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="561ca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="561ca-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="561ca-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="561ca-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="561ca-112">Application</span></span> | <span data-ttu-id="561ca-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="561ca-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="561ca-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="561ca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="561ca-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="561ca-115">Request headers</span></span>
| <span data-ttu-id="561ca-116">Name</span><span class="sxs-lookup"><span data-stu-id="561ca-116">Name</span></span>       | <span data-ttu-id="561ca-117">Typ</span><span class="sxs-lookup"><span data-stu-id="561ca-117">Type</span></span> | <span data-ttu-id="561ca-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="561ca-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="561ca-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="561ca-119">Authorization</span></span>  | <span data-ttu-id="561ca-120">string</span><span class="sxs-lookup"><span data-stu-id="561ca-120">string</span></span>  | <span data-ttu-id="561ca-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="561ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="561ca-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="561ca-123">Content-Type</span></span> | <span data-ttu-id="561ca-124">string</span><span class="sxs-lookup"><span data-stu-id="561ca-124">string</span></span>  | <span data-ttu-id="561ca-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="561ca-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="561ca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="561ca-127">Request body</span></span>
<span data-ttu-id="561ca-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="561ca-128">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="561ca-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="561ca-129">Response</span></span>

<span data-ttu-id="561ca-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="561ca-130">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="561ca-131">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="561ca-131">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="561ca-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="561ca-132">Request</span></span>
<span data-ttu-id="561ca-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="561ca-133">Here is an example of the request.</span></span>
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

<span data-ttu-id="561ca-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="561ca-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="561ca-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="561ca-135">Response</span></span>
<span data-ttu-id="561ca-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="561ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="561ca-139">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="561ca-139">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="561ca-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="561ca-140">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="561ca-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="561ca-141">Response</span></span>
<span data-ttu-id="561ca-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="561ca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
