# <a name="delete-educationclass"></a><span data-ttu-id="8917c-101">EducationClass löschen</span><span class="sxs-lookup"><span data-stu-id="8917c-101">Delete educationClass</span></span>

<span data-ttu-id="8917c-102">Löschen einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="8917c-102">Delete a class.</span></span> <span data-ttu-id="8917c-103">Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8917c-103">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8917c-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8917c-104">Permissions</span></span>
<span data-ttu-id="8917c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8917c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8917c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8917c-107">Permission type</span></span>      | <span data-ttu-id="8917c-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8917c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8917c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8917c-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="8917c-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8917c-110">Not supported.</span></span>  |
|<span data-ttu-id="8917c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8917c-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8917c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8917c-112">Not supported.</span></span>  |
|<span data-ttu-id="8917c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8917c-113">Application</span></span> | <span data-ttu-id="8917c-114">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8917c-114">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8917c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8917c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8917c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8917c-116">Request headers</span></span>
| <span data-ttu-id="8917c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8917c-117">Header</span></span>       | <span data-ttu-id="8917c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8917c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8917c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8917c-119">Authorization</span></span>  | <span data-ttu-id="8917c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8917c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8917c-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8917c-122">Request body</span></span>
<span data-ttu-id="8917c-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8917c-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8917c-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="8917c-124">Response</span></span>
<span data-ttu-id="8917c-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8917c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8917c-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8917c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8917c-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8917c-128">Request</span></span>
<span data-ttu-id="8917c-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8917c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="8917c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8917c-130">Response</span></span>
<span data-ttu-id="8917c-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8917c-131">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->