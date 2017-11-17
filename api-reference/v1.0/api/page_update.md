# <a name="update-page"></a><span data-ttu-id="1f745-101">Seite aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f745-101">Update page</span></span>

<span data-ttu-id="1f745-102">Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="1f745-102">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f745-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f745-103">Permissions</span></span>
<span data-ttu-id="1f745-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f745-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f745-106">Permission type</span></span>      | <span data-ttu-id="1f745-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f745-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f745-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f745-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1f745-109">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f745-109">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f745-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f745-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f745-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f745-111">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1f745-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f745-112">Application</span></span> | <span data-ttu-id="1f745-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f745-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f745-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f745-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="1f745-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f745-115">Request headers</span></span>
| <span data-ttu-id="1f745-116">Name</span><span class="sxs-lookup"><span data-stu-id="1f745-116">Name</span></span>       | <span data-ttu-id="1f745-117">Typ</span><span class="sxs-lookup"><span data-stu-id="1f745-117">Type</span></span> | <span data-ttu-id="1f745-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f745-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f745-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f745-119">Authorization</span></span>  | <span data-ttu-id="1f745-120">string</span><span class="sxs-lookup"><span data-stu-id="1f745-120">string</span></span>  | <span data-ttu-id="1f745-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f745-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f745-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f745-123">Content-Type</span></span> | <span data-ttu-id="1f745-124">string</span><span class="sxs-lookup"><span data-stu-id="1f745-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1f745-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f745-125">Request body</span></span>
<span data-ttu-id="1f745-p103">Geben Sie im Anforderungstext ein Array von [patchContentCommand](../resources/patchcontentcommand.md)-Objekten an, die die Änderungen an der Seite darstellen. Weitere Informationen und Beispiele finden Sie im unter <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote-Seiten aktualisieren</a>.</span><span class="sxs-lookup"><span data-stu-id="1f745-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="1f745-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f745-128">Response</span></span>

<span data-ttu-id="1f745-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.  Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f745-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="1f745-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f745-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f745-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f745-132">Request</span></span>
<span data-ttu-id="1f745-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f745-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="1f745-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f745-134">Response</span></span>
<span data-ttu-id="1f745-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f745-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
