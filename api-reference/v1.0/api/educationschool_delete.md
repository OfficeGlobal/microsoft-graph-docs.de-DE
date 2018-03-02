# <a name="delete-educationschool"></a><span data-ttu-id="e6ece-101">EducationSchool löschen</span><span class="sxs-lookup"><span data-stu-id="e6ece-101">Delete educationSchool</span></span>

<span data-ttu-id="e6ece-102">Löschen einer Schule.</span><span class="sxs-lookup"><span data-stu-id="e6ece-102">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ece-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6ece-103">Permissions</span></span>
<span data-ttu-id="e6ece-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6ece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6ece-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6ece-106">Permission type</span></span>      | <span data-ttu-id="e6ece-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6ece-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6ece-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6ece-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6ece-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6ece-109">Not supported.</span></span>  |
|<span data-ttu-id="e6ece-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6ece-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6ece-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6ece-111">Not supported.</span></span>  |
|<span data-ttu-id="e6ece-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6ece-112">Application</span></span> | <span data-ttu-id="e6ece-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ece-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e6ece-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6ece-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e6ece-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6ece-115">Request headers</span></span>
| <span data-ttu-id="e6ece-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e6ece-116">Header</span></span>       | <span data-ttu-id="e6ece-117">Wert</span><span class="sxs-lookup"><span data-stu-id="e6ece-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6ece-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ece-118">Authorization</span></span>  | <span data-ttu-id="e6ece-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6ece-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6ece-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6ece-121">Request body</span></span>
<span data-ttu-id="e6ece-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6ece-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e6ece-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6ece-123">Response</span></span>
<span data-ttu-id="e6ece-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6ece-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ece-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6ece-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6ece-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6ece-127">Request</span></span>
<span data-ttu-id="e6ece-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6ece-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="e6ece-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6ece-129">Response</span></span>
<span data-ttu-id="e6ece-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6ece-130">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->