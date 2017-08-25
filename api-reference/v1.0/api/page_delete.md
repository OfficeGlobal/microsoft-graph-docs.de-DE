# <a name="delete-page"></a><span data-ttu-id="5f350-101">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="5f350-101">Delete page</span></span>

<span data-ttu-id="5f350-102">Mit dieser API können Sie OneNote-Seiten löschen.</span><span class="sxs-lookup"><span data-stu-id="5f350-102">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f350-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5f350-103">Permissions</span></span>
<span data-ttu-id="5f350-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f350-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f350-106">Permission type</span></span>      | <span data-ttu-id="5f350-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f350-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="5f350-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f350-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5f350-109">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f350-109">Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="5f350-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f350-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f350-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f350-111">Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="5f350-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f350-112">Application</span></span> | <span data-ttu-id="5f350-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f350-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5f350-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f350-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5f350-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f350-115">Request headers</span></span>
| <span data-ttu-id="5f350-116">Name</span><span class="sxs-lookup"><span data-stu-id="5f350-116">Name</span></span>       | <span data-ttu-id="5f350-117">Typ</span><span class="sxs-lookup"><span data-stu-id="5f350-117">Type</span></span> | <span data-ttu-id="5f350-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f350-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f350-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f350-119">Authorization</span></span>  | <span data-ttu-id="5f350-120">string</span><span class="sxs-lookup"><span data-stu-id="5f350-120">string</span></span>  | <span data-ttu-id="5f350-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f350-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5f350-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f350-123">Response</span></span>

<span data-ttu-id="5f350-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f350-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f350-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f350-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f350-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f350-127">Request</span></span>
<span data-ttu-id="5f350-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f350-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="5f350-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f350-129">Response</span></span>
<span data-ttu-id="5f350-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5f350-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->