# <a name="delete-message"></a><span data-ttu-id="17f05-101">Nachricht löschen</span><span class="sxs-lookup"><span data-stu-id="17f05-101">Delete message</span></span>

<span data-ttu-id="17f05-102">Löschen Sie eine Nachricht im Postfach des jeweiligen Benutzers, oder löschen Sie eine Beziehung zur Nachricht.</span><span class="sxs-lookup"><span data-stu-id="17f05-102">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="17f05-103">**Hinweis** Eventuell können Sie Elemente im Ordner "wiederherstellbare Elemente" (unter dem [altbekannten Ordnernamen ](../resources/mailfolder.md)`recoverableitemsdeletions`) nicht löschen.</span><span class="sxs-lookup"><span data-stu-id="17f05-103">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="17f05-104">Weitere Informationen finden Sie unter [Aufbewahrung gelöschter Elemente](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Aufräumen gelöschter Elemente](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items).</span><span class="sxs-lookup"><span data-stu-id="17f05-104">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="17f05-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="17f05-105">Permissions</span></span>
<span data-ttu-id="17f05-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="17f05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17f05-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17f05-108">Permission type</span></span>      | <span data-ttu-id="17f05-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17f05-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17f05-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17f05-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17f05-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17f05-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="17f05-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17f05-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17f05-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17f05-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="17f05-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17f05-114">Application</span></span> | <span data-ttu-id="17f05-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17f05-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="17f05-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17f05-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="17f05-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17f05-117">Request headers</span></span>
| <span data-ttu-id="17f05-118">Name</span><span class="sxs-lookup"><span data-stu-id="17f05-118">Name</span></span>       | <span data-ttu-id="17f05-119">Typ</span><span class="sxs-lookup"><span data-stu-id="17f05-119">Type</span></span> | <span data-ttu-id="17f05-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17f05-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17f05-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="17f05-121">Authorization</span></span>  | <span data-ttu-id="17f05-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17f05-122">string</span></span>  | <span data-ttu-id="17f05-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17f05-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17f05-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17f05-125">Request body</span></span>
<span data-ttu-id="17f05-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="17f05-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17f05-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="17f05-127">Response</span></span>

<span data-ttu-id="17f05-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17f05-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f05-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17f05-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17f05-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17f05-131">Request</span></span>
<span data-ttu-id="17f05-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17f05-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="17f05-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="17f05-133">Response</span></span>
<span data-ttu-id="17f05-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="17f05-134">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->