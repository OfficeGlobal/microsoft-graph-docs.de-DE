# <a name="delete-outlook-category"></a><span data-ttu-id="592e8-101">Löschen der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="592e8-101">Delete Outlook category</span></span>


<span data-ttu-id="592e8-102">Löscht das angegebene [outlookCategory](../resources/outlookCategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="592e8-102">Delete the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="592e8-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="592e8-103">Permissions</span></span>
<span data-ttu-id="592e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="592e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="592e8-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="592e8-106">Permission type</span></span>      | <span data-ttu-id="592e8-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="592e8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="592e8-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="592e8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="592e8-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592e8-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="592e8-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="592e8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="592e8-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592e8-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="592e8-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="592e8-112">Application</span></span> | <span data-ttu-id="592e8-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="592e8-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="592e8-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="592e8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="592e8-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="592e8-115">Optional query parameters</span></span>
<span data-ttu-id="592e8-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="592e8-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="592e8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="592e8-117">Request headers</span></span>
| <span data-ttu-id="592e8-118">Name</span><span class="sxs-lookup"><span data-stu-id="592e8-118">Name</span></span>      |<span data-ttu-id="592e8-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="592e8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="592e8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="592e8-120">Authorization</span></span>  | <span data-ttu-id="592e8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="592e8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="592e8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="592e8-123">Request body</span></span>
<span data-ttu-id="592e8-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="592e8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="592e8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="592e8-125">Response</span></span>

<span data-ttu-id="592e8-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="592e8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="592e8-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="592e8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="592e8-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="592e8-129">Request</span></span>
<span data-ttu-id="592e8-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="592e8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="592e8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="592e8-131">Response</span></span>
<span data-ttu-id="592e8-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="592e8-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->