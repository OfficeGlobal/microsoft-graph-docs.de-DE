# <a name="list-attachments"></a><span data-ttu-id="f1775-101">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="f1775-101">List attachments</span></span>

<span data-ttu-id="f1775-102">Dient zum Abrufen einer Liste von [attachment](../resources/attachment.md)-Objekten, die an einen Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="f1775-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1775-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1775-103">Prerequisites</span></span>
<span data-ttu-id="f1775-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="f1775-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="f1775-105">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1775-105">Group.Read.All</span></span>
* <span data-ttu-id="f1775-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1775-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f1775-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1775-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f1775-108">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="f1775-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1775-109">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f1775-109">Optional query parameters</span></span>
<span data-ttu-id="f1775-110">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f1775-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1775-111">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1775-111">Request headers</span></span>
| <span data-ttu-id="f1775-112">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1775-112">Header</span></span>       | <span data-ttu-id="f1775-113">Wert</span><span class="sxs-lookup"><span data-stu-id="f1775-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1775-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1775-114">Authorization</span></span>  | <span data-ttu-id="f1775-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1775-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1775-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1775-117">Request body</span></span>
<span data-ttu-id="f1775-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1775-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1775-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1775-119">Response</span></span>

<span data-ttu-id="f1775-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1775-120">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1775-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1775-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1775-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1775-122">Request</span></span>
<span data-ttu-id="f1775-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1775-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="f1775-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1775-124">Response</span></span>
<span data-ttu-id="f1775-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1775-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
