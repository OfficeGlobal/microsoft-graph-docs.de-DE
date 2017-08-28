# <a name="delete-photo"></a><span data-ttu-id="3fd07-101">Foto löschen</span><span class="sxs-lookup"><span data-stu-id="3fd07-101">Delete photo</span></span>

<span data-ttu-id="3fd07-102">Mit dieser API können Sie Fotos löschen.</span><span class="sxs-lookup"><span data-stu-id="3fd07-102">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="3fd07-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3fd07-103">Permissions</span></span>
<span data-ttu-id="3fd07-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fd07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3fd07-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3fd07-106">Permission type</span></span>      | <span data-ttu-id="3fd07-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3fd07-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fd07-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3fd07-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3fd07-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fd07-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3fd07-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3fd07-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fd07-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fd07-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3fd07-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3fd07-112">Application</span></span> | <span data-ttu-id="3fd07-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fd07-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fd07-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fd07-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="3fd07-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3fd07-115">Request headers</span></span>
| <span data-ttu-id="3fd07-116">Name</span><span class="sxs-lookup"><span data-stu-id="3fd07-116">Name</span></span>       | <span data-ttu-id="3fd07-117">Typ</span><span class="sxs-lookup"><span data-stu-id="3fd07-117">Type</span></span> | <span data-ttu-id="3fd07-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3fd07-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3fd07-119">if-match</span><span class="sxs-lookup"><span data-stu-id="3fd07-119">if-match</span></span>  | <span data-ttu-id="3fd07-120">string</span><span class="sxs-lookup"><span data-stu-id="3fd07-120">string</span></span>  | <span data-ttu-id="3fd07-121">Wenn dieser Anforderungsheader enthalten ist und das angegebene Etag (oder CTag) nicht mit dem aktuellen Etag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="3fd07-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="3fd07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fd07-122">Authorization</span></span>  | <span data-ttu-id="3fd07-123">string</span><span class="sxs-lookup"><span data-stu-id="3fd07-123">string</span></span>  | <span data-ttu-id="3fd07-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3fd07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fd07-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3fd07-126">Request body</span></span>
<span data-ttu-id="3fd07-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3fd07-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fd07-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fd07-128">Response</span></span>

<span data-ttu-id="3fd07-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3fd07-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fd07-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3fd07-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fd07-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fd07-132">Request</span></span>
<span data-ttu-id="3fd07-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3fd07-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="3fd07-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fd07-134">Response</span></span>
<span data-ttu-id="3fd07-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3fd07-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
