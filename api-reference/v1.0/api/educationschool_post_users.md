# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="9dd13-101">EducationUser zu einer educationSchool hinzufügen</span><span class="sxs-lookup"><span data-stu-id="9dd13-101">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="9dd13-102">Hinzufügen eines Benutzers zu einer Schule.</span><span class="sxs-lookup"><span data-stu-id="9dd13-102">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dd13-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9dd13-103">Permissions</span></span>
<span data-ttu-id="9dd13-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9dd13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9dd13-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9dd13-106">Permission type</span></span>      | <span data-ttu-id="9dd13-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9dd13-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dd13-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9dd13-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9dd13-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9dd13-109">Not supported.</span></span>  |
|<span data-ttu-id="9dd13-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9dd13-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9dd13-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9dd13-111">Not supported.</span></span>  |
|<span data-ttu-id="9dd13-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9dd13-112">Application</span></span> | <span data-ttu-id="9dd13-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd13-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9dd13-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dd13-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9dd13-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9dd13-115">Request headers</span></span>
| <span data-ttu-id="9dd13-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9dd13-116">Header</span></span>       | <span data-ttu-id="9dd13-117">Wert</span><span class="sxs-lookup"><span data-stu-id="9dd13-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9dd13-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9dd13-118">Authorization</span></span>  | <span data-ttu-id="9dd13-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dd13-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9dd13-121">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="9dd13-121">Content-Type</span></span>  | <span data-ttu-id="9dd13-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9dd13-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9dd13-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9dd13-123">Request body</span></span>
<span data-ttu-id="9dd13-124">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9dd13-124">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9dd13-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dd13-125">Response</span></span>
<span data-ttu-id="9dd13-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9dd13-126">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd13-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9dd13-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dd13-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dd13-128">Request</span></span>
<span data-ttu-id="9dd13-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9dd13-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="9dd13-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dd13-130">Response</span></span>
<span data-ttu-id="9dd13-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9dd13-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->