# <a name="page-copytosection"></a><span data-ttu-id="c87fb-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="c87fb-101">page: copyToSection</span></span>
<span data-ttu-id="c87fb-102">Kopiert eine Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="c87fb-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="c87fb-103">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Aktion „Copy“ auf, und fragen Sie dann das Ergebnis vom Vorgangsendpunkt ab.</span><span class="sxs-lookup"><span data-stu-id="c87fb-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="c87fb-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c87fb-104">Permissions</span></span>
<span data-ttu-id="c87fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c87fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c87fb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c87fb-107">Permission type</span></span>      | <span data-ttu-id="c87fb-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c87fb-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c87fb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c87fb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c87fb-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87fb-110">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c87fb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c87fb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87fb-112">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c87fb-112">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c87fb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c87fb-113">Application</span></span> | <span data-ttu-id="c87fb-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87fb-114">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c87fb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c87fb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="c87fb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c87fb-116">Request headers</span></span>
| <span data-ttu-id="c87fb-117">Name</span><span class="sxs-lookup"><span data-stu-id="c87fb-117">Name</span></span>       | <span data-ttu-id="c87fb-118">Typ</span><span class="sxs-lookup"><span data-stu-id="c87fb-118">Type</span></span> | <span data-ttu-id="c87fb-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c87fb-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c87fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c87fb-120">Authorization</span></span>  | <span data-ttu-id="c87fb-121">string</span><span class="sxs-lookup"><span data-stu-id="c87fb-121">string</span></span>  | <span data-ttu-id="c87fb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c87fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c87fb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c87fb-124">Content-Type</span></span> | <span data-ttu-id="c87fb-125">string</span><span class="sxs-lookup"><span data-stu-id="c87fb-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c87fb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c87fb-126">Request body</span></span>
<span data-ttu-id="c87fb-127">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="c87fb-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="c87fb-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="c87fb-128">Parameter</span></span>    | <span data-ttu-id="c87fb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c87fb-129">Type</span></span>   |<span data-ttu-id="c87fb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c87fb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c87fb-131">groupId</span><span class="sxs-lookup"><span data-stu-id="c87fb-131">groupId</span></span>|<span data-ttu-id="c87fb-132">String</span><span class="sxs-lookup"><span data-stu-id="c87fb-132">String</span></span>|<span data-ttu-id="c87fb-p103">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c87fb-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="c87fb-135">id</span><span class="sxs-lookup"><span data-stu-id="c87fb-135">id</span></span>|<span data-ttu-id="c87fb-136">String</span><span class="sxs-lookup"><span data-stu-id="c87fb-136">String</span></span>|<span data-ttu-id="c87fb-p104">Erforderlich. Die ID des Zielabschnitts.</span><span class="sxs-lookup"><span data-stu-id="c87fb-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="c87fb-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c87fb-139">Response</span></span>

<span data-ttu-id="c87fb-p105">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="c87fb-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="c87fb-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c87fb-142">Example</span></span>
<span data-ttu-id="c87fb-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c87fb-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c87fb-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c87fb-144">Request</span></span>
<span data-ttu-id="c87fb-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c87fb-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="c87fb-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c87fb-146">Response</span></span>
<span data-ttu-id="c87fb-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c87fb-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->