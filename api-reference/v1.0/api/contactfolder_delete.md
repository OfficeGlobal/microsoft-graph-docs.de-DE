# <a name="delete-contactfolder"></a><span data-ttu-id="a2b56-101">contactFolder löschen</span><span class="sxs-lookup"><span data-stu-id="a2b56-101">Delete contactFolder</span></span>

<span data-ttu-id="a2b56-102">Mit dieser API können Sie Ressourcen des Typs „contactFolder“ löschen (nicht jedoch die als Standardordner festgelegte Ressource des Typs „contactFolder“).</span><span class="sxs-lookup"><span data-stu-id="a2b56-102">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2b56-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a2b56-103">Permissions</span></span>
<span data-ttu-id="a2b56-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2b56-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2b56-106">Permission type</span></span>      | <span data-ttu-id="a2b56-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2b56-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2b56-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2b56-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a2b56-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b56-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a2b56-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2b56-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2b56-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b56-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a2b56-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2b56-112">Application</span></span> | <span data-ttu-id="a2b56-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b56-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2b56-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2b56-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a2b56-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2b56-115">Request headers</span></span>
| <span data-ttu-id="a2b56-116">Name</span><span class="sxs-lookup"><span data-stu-id="a2b56-116">Name</span></span>       | <span data-ttu-id="a2b56-117">Typ</span><span class="sxs-lookup"><span data-stu-id="a2b56-117">Type</span></span> | <span data-ttu-id="a2b56-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2b56-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2b56-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b56-119">Authorization</span></span>  | <span data-ttu-id="a2b56-120">string</span><span class="sxs-lookup"><span data-stu-id="a2b56-120">string</span></span>  | <span data-ttu-id="a2b56-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2b56-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2b56-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2b56-123">Request body</span></span>
<span data-ttu-id="a2b56-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a2b56-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2b56-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2b56-125">Response</span></span>

<span data-ttu-id="a2b56-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2b56-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b56-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2b56-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2b56-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2b56-129">Request</span></span>
<span data-ttu-id="a2b56-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2b56-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="a2b56-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2b56-131">Response</span></span>
<span data-ttu-id="a2b56-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2b56-132">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
