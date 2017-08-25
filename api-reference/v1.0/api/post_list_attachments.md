# <a name="list-attachments"></a><span data-ttu-id="756d3-101">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="756d3-101">List attachments</span></span>

<span data-ttu-id="756d3-102">Mit dieser API können Sie eine Liste aller Objekte des Typs [attachment](../resources/attachment.md) abrufen, die einem Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="756d3-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="756d3-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="756d3-103">Permissions</span></span>
<span data-ttu-id="756d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="756d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="756d3-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="756d3-106">Permission type</span></span>      | <span data-ttu-id="756d3-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="756d3-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="756d3-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="756d3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="756d3-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="756d3-109">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="756d3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="756d3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="756d3-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="756d3-111">Not supported.</span></span>    | 
|<span data-ttu-id="756d3-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="756d3-112">Application</span></span> | <span data-ttu-id="756d3-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="756d3-113">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="756d3-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="756d3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="756d3-115">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="756d3-115">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="756d3-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="756d3-116">Optional query parameters</span></span>
<span data-ttu-id="756d3-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="756d3-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="756d3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="756d3-118">Request headers</span></span>
| <span data-ttu-id="756d3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="756d3-119">Header</span></span>       | <span data-ttu-id="756d3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="756d3-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="756d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="756d3-121">Authorization</span></span>  | <span data-ttu-id="756d3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="756d3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="756d3-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="756d3-124">Request body</span></span>
<span data-ttu-id="756d3-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="756d3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="756d3-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="756d3-126">Response</span></span>

<span data-ttu-id="756d3-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="756d3-127">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="756d3-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="756d3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="756d3-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="756d3-129">Request</span></span>
<span data-ttu-id="756d3-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="756d3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="756d3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="756d3-131">Response</span></span>
<span data-ttu-id="756d3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="756d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
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
