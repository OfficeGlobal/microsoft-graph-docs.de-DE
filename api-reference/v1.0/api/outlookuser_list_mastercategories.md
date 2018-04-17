# <a name="list-outlook-categories"></a><span data-ttu-id="ce8aa-101">Auflisten von Outlook-Kategorien</span><span class="sxs-lookup"><span data-stu-id="ce8aa-101">List Outlook categories</span></span>


<span data-ttu-id="ce8aa-102">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-102">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce8aa-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ce8aa-103">Permissions</span></span>
<span data-ttu-id="ce8aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce8aa-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce8aa-106">Permission type</span></span>      | <span data-ttu-id="ce8aa-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce8aa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce8aa-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce8aa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ce8aa-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ce8aa-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ce8aa-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce8aa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce8aa-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ce8aa-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ce8aa-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce8aa-112">Application</span></span> | <span data-ttu-id="ce8aa-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ce8aa-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce8aa-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce8aa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce8aa-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ce8aa-115">Optional query parameters</span></span>
<span data-ttu-id="ce8aa-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce8aa-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce8aa-117">Request headers</span></span>
| <span data-ttu-id="ce8aa-118">Name</span><span class="sxs-lookup"><span data-stu-id="ce8aa-118">Name</span></span>      |<span data-ttu-id="ce8aa-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce8aa-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce8aa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce8aa-120">Authorization</span></span>  | <span data-ttu-id="ce8aa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce8aa-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce8aa-123">Request body</span></span>
<span data-ttu-id="ce8aa-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce8aa-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce8aa-125">Response</span></span>

<span data-ttu-id="ce8aa-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [outlookCategory](../resources/outlookCategory.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/outlookCategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce8aa-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce8aa-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce8aa-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce8aa-128">Request</span></span>
<span data-ttu-id="ce8aa-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="ce8aa-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce8aa-130">Response</span></span>
<span data-ttu-id="ce8aa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce8aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->