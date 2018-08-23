# <a name="delete-mailfolder"></a><span data-ttu-id="5c9da-101">mailFolder löschen</span><span class="sxs-lookup"><span data-stu-id="5c9da-101">Delete mailFolder</span></span>

<span data-ttu-id="5c9da-102">Löschen Sie den angegebenen [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5c9da-102">Delete the specified mailFolder object.</span></span>

<span data-ttu-id="5c9da-103">Sie können einen E-Mail-Oder durch seine Ordner-ID oder durch seinen [bekannten Ordnernamen](../resources/mailfolder.md), falls dieser existiert, angeben.</span><span class="sxs-lookup"><span data-stu-id="5c9da-103">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="5c9da-104">**Hinweis** Eventuell können Sie Elemente im Ordner "wiederhergestellte Elemente" (mit dem bekannten Ordnernamen `recoverableitemsdeletions`) nicht löschen.</span><span class="sxs-lookup"><span data-stu-id="5c9da-104">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="5c9da-105">Weitere Informationen finden Sie unter [Aufbewahrung gelöschter Elemente](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Aufräumen gelöschter Elemente](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items).</span><span class="sxs-lookup"><span data-stu-id="5c9da-105">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c9da-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5c9da-106">Permissions</span></span>
<span data-ttu-id="5c9da-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c9da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5c9da-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c9da-109">Permission type</span></span>      | <span data-ttu-id="5c9da-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c9da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c9da-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c9da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c9da-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c9da-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c9da-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c9da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c9da-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c9da-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c9da-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c9da-115">Application</span></span> | <span data-ttu-id="5c9da-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c9da-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c9da-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c9da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5c9da-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c9da-118">Request headers</span></span>
| <span data-ttu-id="5c9da-119">Name</span><span class="sxs-lookup"><span data-stu-id="5c9da-119">Name</span></span>       | <span data-ttu-id="5c9da-120">Typ</span><span class="sxs-lookup"><span data-stu-id="5c9da-120">Type</span></span> | <span data-ttu-id="5c9da-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c9da-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c9da-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5c9da-122">Authorization</span></span>  | <span data-ttu-id="5c9da-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c9da-123">string</span></span>  | <span data-ttu-id="5c9da-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5c9da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c9da-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c9da-126">Request body</span></span>
<span data-ttu-id="5c9da-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5c9da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c9da-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c9da-128">Response</span></span>

<span data-ttu-id="5c9da-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c9da-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c9da-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c9da-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c9da-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c9da-132">Request</span></span>
<span data-ttu-id="5c9da-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c9da-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="5c9da-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c9da-134">Response</span></span>
<span data-ttu-id="5c9da-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5c9da-135">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->