# <a name="delete-group"></a><span data-ttu-id="b88ba-101">Gruppe löschen</span><span class="sxs-lookup"><span data-stu-id="b88ba-101">Delete group</span></span>

<span data-ttu-id="b88ba-102">Mit dieser API können Sie Gruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="b88ba-102">Delete group.</span></span>
## <a name="permissions"></a><span data-ttu-id="b88ba-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b88ba-103">Permissions</span></span>
<span data-ttu-id="b88ba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b88ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b88ba-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b88ba-106">Permission type</span></span>      | <span data-ttu-id="b88ba-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b88ba-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b88ba-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b88ba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b88ba-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b88ba-109">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b88ba-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b88ba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b88ba-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b88ba-111">Not supported.</span></span>    | 
|<span data-ttu-id="b88ba-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b88ba-112">Application</span></span> | <span data-ttu-id="b88ba-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b88ba-113">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b88ba-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b88ba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b88ba-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b88ba-115">Request headers</span></span>
| <span data-ttu-id="b88ba-116">Name</span><span class="sxs-lookup"><span data-stu-id="b88ba-116">Name</span></span>       | <span data-ttu-id="b88ba-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b88ba-117">Type</span></span> | <span data-ttu-id="b88ba-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b88ba-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b88ba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b88ba-119">Authorization</span></span>  | <span data-ttu-id="b88ba-120">string</span><span class="sxs-lookup"><span data-stu-id="b88ba-120">string</span></span>  | <span data-ttu-id="b88ba-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b88ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b88ba-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b88ba-123">Request body</span></span>
<span data-ttu-id="b88ba-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b88ba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b88ba-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="b88ba-125">Response</span></span>

<span data-ttu-id="b88ba-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b88ba-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b88ba-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b88ba-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b88ba-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b88ba-129">Request</span></span>
<span data-ttu-id="b88ba-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b88ba-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
##### <a name="response"></a><span data-ttu-id="b88ba-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b88ba-131">Response</span></span>
<span data-ttu-id="b88ba-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b88ba-132">Here is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->