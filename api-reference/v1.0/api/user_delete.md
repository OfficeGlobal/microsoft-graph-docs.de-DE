# <a name="delete-a-user"></a><span data-ttu-id="48c8a-101">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="48c8a-101">Delete a user</span></span>

<span data-ttu-id="48c8a-102">Mit dieser API können Sie Benutzer löschen.</span><span class="sxs-lookup"><span data-stu-id="48c8a-102">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="48c8a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48c8a-103">Permissions</span></span>
<span data-ttu-id="48c8a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48c8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48c8a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48c8a-106">Permission type</span></span>      | <span data-ttu-id="48c8a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48c8a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48c8a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48c8a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="48c8a-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48c8a-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48c8a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48c8a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48c8a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48c8a-111">Not supported.</span></span>    |
|<span data-ttu-id="48c8a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48c8a-112">Application</span></span> | <span data-ttu-id="48c8a-113">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48c8a-113">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48c8a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48c8a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="48c8a-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48c8a-115">Request headers</span></span>
| <span data-ttu-id="48c8a-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48c8a-116">Header</span></span>       | <span data-ttu-id="48c8a-117">Wert</span><span class="sxs-lookup"><span data-stu-id="48c8a-117">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="48c8a-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="48c8a-118">Authorization</span></span>  | <span data-ttu-id="48c8a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48c8a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48c8a-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48c8a-121">Request body</span></span>
<span data-ttu-id="48c8a-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="48c8a-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48c8a-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="48c8a-123">Response</span></span>

<span data-ttu-id="48c8a-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48c8a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48c8a-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48c8a-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48c8a-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48c8a-127">Request</span></span>
<span data-ttu-id="48c8a-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48c8a-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="48c8a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="48c8a-129">Response</span></span>
<span data-ttu-id="48c8a-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48c8a-130">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->