# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="19699-101">EducationUser aus einer educationSchool entfernen</span><span class="sxs-lookup"><span data-stu-id="19699-101">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="19699-102">Löschen eines Benutzers aus einer Schule.</span><span class="sxs-lookup"><span data-stu-id="19699-102">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="19699-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19699-103">Permissions</span></span>
<span data-ttu-id="19699-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19699-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19699-106">Permission type</span></span>      | <span data-ttu-id="19699-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19699-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19699-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19699-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="19699-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19699-109">Not supported.</span></span>  |
|<span data-ttu-id="19699-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19699-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="19699-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19699-111">Not supported.</span></span>  |
|<span data-ttu-id="19699-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19699-112">Application</span></span> | <span data-ttu-id="19699-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19699-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="19699-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19699-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="19699-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19699-115">Request headers</span></span>
| <span data-ttu-id="19699-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="19699-116">Header</span></span>       | <span data-ttu-id="19699-117">Wert</span><span class="sxs-lookup"><span data-stu-id="19699-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19699-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="19699-118">Authorization</span></span>  | <span data-ttu-id="19699-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19699-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19699-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19699-121">Request body</span></span>
<span data-ttu-id="19699-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="19699-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="19699-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="19699-123">Response</span></span>
<span data-ttu-id="19699-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19699-124">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="19699-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19699-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19699-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19699-126">Request</span></span>
<span data-ttu-id="19699-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19699-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="19699-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="19699-128">Response</span></span>
<span data-ttu-id="19699-129">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19699-129">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->