# <a name="delete-a-user"></a><span data-ttu-id="8ae66-101">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="8ae66-101">Delete a user</span></span>

<span data-ttu-id="8ae66-102">Mit dieser API können Sie Benutzer löschen.</span><span class="sxs-lookup"><span data-stu-id="8ae66-102">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ae66-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ae66-103">Permissions</span></span>
<span data-ttu-id="8ae66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ae66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ae66-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ae66-106">Permission type</span></span>      | <span data-ttu-id="8ae66-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ae66-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="8ae66-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ae66-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8ae66-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ae66-109">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="8ae66-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ae66-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ae66-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ae66-111">Not supported.</span></span>    | 
|<span data-ttu-id="8ae66-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ae66-112">Application</span></span> | <span data-ttu-id="8ae66-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ae66-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8ae66-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ae66-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="8ae66-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ae66-115">Request headers</span></span>
| <span data-ttu-id="8ae66-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8ae66-116">Header</span></span>       | <span data-ttu-id="8ae66-117">Wert</span><span class="sxs-lookup"><span data-stu-id="8ae66-117">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="8ae66-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae66-118">Authorization</span></span>  | <span data-ttu-id="8ae66-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ae66-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ae66-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ae66-121">Request body</span></span>
<span data-ttu-id="8ae66-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ae66-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ae66-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ae66-123">Response</span></span>

<span data-ttu-id="8ae66-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ae66-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae66-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ae66-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ae66-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ae66-127">Request</span></span>
<span data-ttu-id="8ae66-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ae66-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/mba9a3254-9f18-4209-aeb3-9e42a35b5be4
```
##### <a name="response"></a><span data-ttu-id="8ae66-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ae66-129">Response</span></span>
<span data-ttu-id="8ae66-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ae66-130">Here is an example of the response.</span></span> 
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