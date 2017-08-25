# <a name="list-attachments"></a><span data-ttu-id="20279-101">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="20279-101">List attachments</span></span>

<span data-ttu-id="20279-102">Mit dieser API können Sie eine Liste von Anlagenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="20279-102">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="20279-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="20279-103">Permissions</span></span>
<span data-ttu-id="20279-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20279-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20279-106">Permission type</span></span>      | <span data-ttu-id="20279-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20279-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="20279-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20279-108">Delegated (work or school account)</span></span> | <span data-ttu-id="20279-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20279-109">Mail.Read</span></span>    | 
|<span data-ttu-id="20279-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20279-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20279-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20279-111">Mail.Read</span></span>    | 
|<span data-ttu-id="20279-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20279-112">Application</span></span> | <span data-ttu-id="20279-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20279-113">Mail.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="20279-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20279-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20279-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="20279-115">Optional query parameters</span></span>
<span data-ttu-id="20279-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="20279-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20279-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20279-117">Request headers</span></span>
| <span data-ttu-id="20279-118">Name</span><span class="sxs-lookup"><span data-stu-id="20279-118">Name</span></span>       | <span data-ttu-id="20279-119">Typ</span><span class="sxs-lookup"><span data-stu-id="20279-119">Type</span></span> | <span data-ttu-id="20279-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20279-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20279-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20279-121">Authorization</span></span>  | <span data-ttu-id="20279-122">string</span><span class="sxs-lookup"><span data-stu-id="20279-122">string</span></span>  | <span data-ttu-id="20279-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="20279-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20279-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20279-125">Request body</span></span>
<span data-ttu-id="20279-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="20279-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20279-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="20279-127">Response</span></span>

<span data-ttu-id="20279-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20279-128">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20279-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20279-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20279-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20279-130">Request</span></span>
<span data-ttu-id="20279-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20279-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="20279-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="20279-132">Response</span></span>
<span data-ttu-id="20279-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20279-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
