# <a name="get-outlook-category"></a><span data-ttu-id="5b922-101">Abrufen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="5b922-101">Get Outlook category</span></span>


<span data-ttu-id="5b922-102">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [outlookCategory](../resources/outlookCategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b922-102">Get the properties and relationships of the specified [event](../resources/outlookCategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b922-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b922-103">Permissions</span></span>
<span data-ttu-id="5b922-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5b922-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b922-106">Permission type</span></span>      | <span data-ttu-id="5b922-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b922-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b922-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b922-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5b922-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5b922-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="5b922-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b922-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b922-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5b922-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="5b922-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b922-112">Application</span></span> | <span data-ttu-id="5b922-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5b922-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b922-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b922-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b922-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5b922-115">Optional query parameters</span></span>
<span data-ttu-id="5b922-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b922-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b922-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b922-117">Request headers</span></span>
| <span data-ttu-id="5b922-118">Name</span><span class="sxs-lookup"><span data-stu-id="5b922-118">Name</span></span>      |<span data-ttu-id="5b922-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b922-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b922-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b922-120">Authorization</span></span>  | <span data-ttu-id="5b922-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b922-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b922-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b922-123">Request body</span></span>
<span data-ttu-id="5b922-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b922-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b922-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b922-125">Response</span></span>

<span data-ttu-id="5b922-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [outlookCategory](../resources/outlookCategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b922-126">If successful, this method returns a `200 OK` response code and a [section](../resources/outlookCategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b922-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b922-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b922-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b922-128">Request</span></span>
<span data-ttu-id="5b922-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b922-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories('de912e4d-c790-4da9-949c-ccd933aaa0f7')
```
##### <a name="response"></a><span data-ttu-id="5b922-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b922-130">Response</span></span>
<span data-ttu-id="5b922-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b922-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->