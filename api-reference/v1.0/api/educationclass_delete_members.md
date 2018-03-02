# <a name="remove-a-student"></a><span data-ttu-id="5aad5-101">Entfernen eines Kursteilnehmers</span><span class="sxs-lookup"><span data-stu-id="5aad5-101">Remove a student</span></span>

<span data-ttu-id="5aad5-102">Entfernt einen [EducationUser](../resources/educationuser.md) aus einer [EducationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="5aad5-102">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="5aad5-103">**Hinweis:** Lehrkräfte _und_ Kursteilnehmer sind in der **members**-Sammlung der Klasse enthalten.</span><span class="sxs-lookup"><span data-stu-id="5aad5-103">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="5aad5-104">Vergewissern Sie sich vor dem Aufrufen dieser API, dass der zu entfernende **educationUser** kein Lehrer ist.</span><span class="sxs-lookup"><span data-stu-id="5aad5-104">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="5aad5-105">Rufen Sie die Liste der Lehrer mit einem Aufruf von [educationclass_list_teachers](educationclass_list_teachers.md) ab, und stellen Sie sicher, dass die Benutzers-ID des zu entfernenden Benutzers nicht in der zurückgegebenen Lehrerliste enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="5aad5-105">Get the list of teachers by calling [educationclass_list_teachers](educationclass_list_teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aad5-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5aad5-106">Permissions</span></span>
<span data-ttu-id="5aad5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5aad5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5aad5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5aad5-109">Permission type</span></span>      | <span data-ttu-id="5aad5-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5aad5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5aad5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5aad5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5aad5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5aad5-112">Not supported.</span></span>  |
|<span data-ttu-id="5aad5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5aad5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5aad5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5aad5-114">Not supported.</span></span>  |
|<span data-ttu-id="5aad5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5aad5-115">Application</span></span> | <span data-ttu-id="5aad5-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aad5-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5aad5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5aad5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5aad5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5aad5-118">Request headers</span></span>
| <span data-ttu-id="5aad5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5aad5-119">Header</span></span>       | <span data-ttu-id="5aad5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5aad5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5aad5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aad5-121">Authorization</span></span>  | <span data-ttu-id="5aad5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5aad5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5aad5-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5aad5-124">Request body</span></span>
<span data-ttu-id="5aad5-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5aad5-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5aad5-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="5aad5-126">Response</span></span>
<span data-ttu-id="5aad5-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5aad5-127">If successful, this method returns a `204 No Content` response code and an event object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aad5-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5aad5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5aad5-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5aad5-129">Request</span></span>
<span data-ttu-id="5aad5-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5aad5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="5aad5-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5aad5-131">Response</span></span>
<span data-ttu-id="5aad5-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5aad5-132">The following is an example of the response.</span></span> 
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
