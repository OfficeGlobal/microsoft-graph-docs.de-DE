# <a name="page-copytosection"></a><span data-ttu-id="f48eb-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="f48eb-101">page: copyToSection</span></span>
<span data-ttu-id="f48eb-102">Kopiert eine Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="f48eb-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="f48eb-103">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="f48eb-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f48eb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f48eb-104">Prerequisites</span></span>
<span data-ttu-id="f48eb-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="f48eb-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="f48eb-106">Notes.Create, Notes.ReadWrite oder Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48eb-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>  

## <a name="http-request"></a><span data-ttu-id="f48eb-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f48eb-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="f48eb-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f48eb-108">Request headers</span></span>
| <span data-ttu-id="f48eb-109">Name</span><span class="sxs-lookup"><span data-stu-id="f48eb-109">Name</span></span>       | <span data-ttu-id="f48eb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f48eb-110">Type</span></span> | <span data-ttu-id="f48eb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f48eb-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f48eb-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="f48eb-112">Authorization</span></span>  | <span data-ttu-id="f48eb-113">string</span><span class="sxs-lookup"><span data-stu-id="f48eb-113">string</span></span>  | <span data-ttu-id="f48eb-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f48eb-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f48eb-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f48eb-116">Content-Type</span></span> | <span data-ttu-id="f48eb-117">string</span><span class="sxs-lookup"><span data-stu-id="f48eb-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f48eb-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f48eb-118">Request body</span></span>
<span data-ttu-id="f48eb-119">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="f48eb-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="f48eb-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="f48eb-120">Parameter</span></span>    | <span data-ttu-id="f48eb-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f48eb-121">Type</span></span>   |<span data-ttu-id="f48eb-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f48eb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f48eb-123">groupId</span><span class="sxs-lookup"><span data-stu-id="f48eb-123">groupId</span></span>|<span data-ttu-id="f48eb-124">String</span><span class="sxs-lookup"><span data-stu-id="f48eb-124">String</span></span>|<span data-ttu-id="f48eb-p102">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f48eb-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="f48eb-127">id</span><span class="sxs-lookup"><span data-stu-id="f48eb-127">id</span></span>|<span data-ttu-id="f48eb-128">String</span><span class="sxs-lookup"><span data-stu-id="f48eb-128">String</span></span>|<span data-ttu-id="f48eb-p103">Erforderlich. Die ID des Zielabschnitts.</span><span class="sxs-lookup"><span data-stu-id="f48eb-p103">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="f48eb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f48eb-131">Response</span></span>

<span data-ttu-id="f48eb-p104">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="f48eb-p104">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="f48eb-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f48eb-134">Example</span></span>
<span data-ttu-id="f48eb-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f48eb-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f48eb-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f48eb-136">Request</span></span>
<span data-ttu-id="f48eb-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f48eb-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f48eb-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f48eb-138">Response</span></span>
<span data-ttu-id="f48eb-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f48eb-139">Here is an example of the response.</span></span>
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