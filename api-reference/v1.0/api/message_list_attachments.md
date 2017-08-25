# <a name="list-attachments"></a><span data-ttu-id="f9e83-101">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="f9e83-101">List attachments</span></span>

<span data-ttu-id="f9e83-102">Mit dieser API können Sie eine Liste der einer Nachricht angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="f9e83-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9e83-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f9e83-103">Permissions</span></span>
<span data-ttu-id="f9e83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9e83-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9e83-106">Permission type</span></span>      | <span data-ttu-id="f9e83-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9e83-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f9e83-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9e83-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f9e83-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f9e83-109">Mail.Read</span></span>    | 
|<span data-ttu-id="f9e83-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9e83-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9e83-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f9e83-111">Mail.Read</span></span>    | 
|<span data-ttu-id="f9e83-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9e83-112">Application</span></span> | <span data-ttu-id="f9e83-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f9e83-113">Mail.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f9e83-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9e83-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f9e83-115">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f9e83-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="f9e83-116">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f9e83-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="f9e83-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="f9e83-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9e83-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f9e83-119">Optional query parameters</span></span>
<span data-ttu-id="f9e83-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9e83-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f9e83-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9e83-121">Request headers</span></span>
| <span data-ttu-id="f9e83-122">Name</span><span class="sxs-lookup"><span data-stu-id="f9e83-122">Name</span></span>       | <span data-ttu-id="f9e83-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f9e83-123">Type</span></span> | <span data-ttu-id="f9e83-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9e83-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9e83-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9e83-125">Authorization</span></span>  | <span data-ttu-id="f9e83-126">string</span><span class="sxs-lookup"><span data-stu-id="f9e83-126">string</span></span>  | <span data-ttu-id="f9e83-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9e83-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9e83-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9e83-129">Request body</span></span>
<span data-ttu-id="f9e83-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f9e83-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9e83-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9e83-131">Response</span></span>

<span data-ttu-id="f9e83-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9e83-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9e83-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9e83-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9e83-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9e83-134">Request</span></span>
<span data-ttu-id="f9e83-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9e83-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="f9e83-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9e83-136">Response</span></span>
<span data-ttu-id="f9e83-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9e83-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->